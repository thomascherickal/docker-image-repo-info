## `pypy:slim`

```console
$ docker pull pypy@sha256:26dd9aa3602f3e79868e9d7c3b23d79bdfc22d320ae2b30d37785007b27eb1ce
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `pypy:slim` - linux; amd64

```console
$ docker pull pypy@sha256:558d89718e8d19d0852ee2ef1781389747710243c083c5bfdedebe97c19599e3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.1 MB (71068589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70b70a79fe0c9655da811bc43b3236f333129a96340fc6b1b9641d0b549141e6`
-	Default Command: `["pypy3"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 14:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 14:46:44 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 14:46:44 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 14:46:45 GMT
ENV PYPY_VERSION=7.3.4
# Wed, 12 May 2021 14:47:14 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux64.tar.bz2'; 			sha256='09d7298b44a38648a87995ec06e1e093761644e50f547c8bb0b2d7f4fe433548'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-aarch64.tar.bz2'; 			sha256='a4148fa73b74a091e004e1f378b278c0b8830984cbcb91e10fa31fd915c43efe'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux32.tar.bz2'; 			sha256='04de1a2e80530f3d74abcf133ec046a0fb12d81956bc043dee8ab4799f3b77eb'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-s390x.tar.bz2'; 			sha256='7d6fb180c359a66a158ef6e81eeca88fbabbb62656a1700f425a70db18de2a0f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 12 May 2021 14:47:15 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 12 May 2021 14:47:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 12 May 2021 14:47:15 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 12 May 2021 14:47:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 12 May 2021 14:47:34 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db5028b68bc95cdca0100f5f0112b94faeafb23674980662f8593d974f1d8a0`  
		Last Modified: Wed, 12 May 2021 14:51:08 GMT  
		Size: 2.8 MB (2757664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140131ab92eee6c4de2147d919e5e95a8bba973529b71106087c00cd92651543`  
		Last Modified: Wed, 12 May 2021 14:51:17 GMT  
		Size: 38.6 MB (38598883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1e5e4e46b270d0a4cfeb9aec13899d721adc852f8f6048dc8d206b688dd14b`  
		Last Modified: Wed, 12 May 2021 14:51:09 GMT  
		Size: 2.6 MB (2566127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:slim` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:e414c50017a2c20aeeb0fe6f4b2fb57f752dce7c24a75ec058cc890b77d667d4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66467259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e41ba8fc942fb915affae044a1472f0055eb6a9c0d8d2102e9c9b2a3033eba`
-	Default Command: `["pypy3"]`

```dockerfile
# Wed, 12 May 2021 00:52:19 GMT
ADD file:91ba1791cab3ad29a1469d1e78f21f4c0b5d3d30598683b7104980604c318854 in / 
# Wed, 12 May 2021 00:52:34 GMT
CMD ["bash"]
# Wed, 12 May 2021 13:45:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 13:45:15 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 13:45:16 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 13:45:18 GMT
ENV PYPY_VERSION=7.3.4
# Wed, 12 May 2021 13:46:20 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux64.tar.bz2'; 			sha256='09d7298b44a38648a87995ec06e1e093761644e50f547c8bb0b2d7f4fe433548'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-aarch64.tar.bz2'; 			sha256='a4148fa73b74a091e004e1f378b278c0b8830984cbcb91e10fa31fd915c43efe'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux32.tar.bz2'; 			sha256='04de1a2e80530f3d74abcf133ec046a0fb12d81956bc043dee8ab4799f3b77eb'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-s390x.tar.bz2'; 			sha256='7d6fb180c359a66a158ef6e81eeca88fbabbb62656a1700f425a70db18de2a0f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 12 May 2021 13:46:25 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 12 May 2021 13:46:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 12 May 2021 13:46:35 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 12 May 2021 13:47:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 12 May 2021 13:47:23 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:fcad0c936ea5c12e1c8c4edb81a97c0cde04ee71e7067ee3b246474cf1854d7a`  
		Last Modified: Wed, 12 May 2021 01:02:02 GMT  
		Size: 25.9 MB (25911250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae606e4b598425ee3f0eae7006e8aae45b5faf7662ede98f48398412254a4f73`  
		Last Modified: Wed, 12 May 2021 13:52:04 GMT  
		Size: 2.6 MB (2626299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db94c99213b29a78a31e2ede0db03a9dff2d1a90bf23f2d441a770ece30ff7`  
		Last Modified: Wed, 12 May 2021 13:52:15 GMT  
		Size: 35.4 MB (35363762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9a0e2944bd344909f63a0e568701f8ead1f9a8ddba287831060fa7c3a652d6`  
		Last Modified: Wed, 12 May 2021 13:52:04 GMT  
		Size: 2.6 MB (2565948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:slim` - linux; 386

```console
$ docker pull pypy@sha256:6e676f31106a9a53ac3c38d086b42664a2c878d9c3bb7276b6a19e0259e23ad7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73735439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b94199a0d059c0e1a1ccc8ded13f36b6b53e9e0e79c37d428768b3d56d73b424`
-	Default Command: `["pypy3"]`

```dockerfile
# Wed, 12 May 2021 00:39:52 GMT
ADD file:62173a7456d614031a7b20be741983644d9723c734eee663b099ad6b47af7b35 in / 
# Wed, 12 May 2021 00:39:53 GMT
CMD ["bash"]
# Wed, 12 May 2021 12:38:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 12:38:40 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 12:38:41 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 12:38:41 GMT
ENV PYPY_VERSION=7.3.4
# Wed, 12 May 2021 12:39:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux64.tar.bz2'; 			sha256='09d7298b44a38648a87995ec06e1e093761644e50f547c8bb0b2d7f4fe433548'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-aarch64.tar.bz2'; 			sha256='a4148fa73b74a091e004e1f378b278c0b8830984cbcb91e10fa31fd915c43efe'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux32.tar.bz2'; 			sha256='04de1a2e80530f3d74abcf133ec046a0fb12d81956bc043dee8ab4799f3b77eb'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-s390x.tar.bz2'; 			sha256='7d6fb180c359a66a158ef6e81eeca88fbabbb62656a1700f425a70db18de2a0f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 12 May 2021 12:39:11 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 12 May 2021 12:39:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 12 May 2021 12:39:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 12 May 2021 12:39:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 12 May 2021 12:39:25 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:9b548256784c8e079e5953ec08bd26ce8cbaed0d606a5d350b4bcd12710d2192`  
		Last Modified: Wed, 12 May 2021 00:46:39 GMT  
		Size: 27.8 MB (27795074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb63b37fe34f2cd5f37adaacc9536932e1923c91535448092ffc5ffcc0d19bb`  
		Last Modified: Wed, 12 May 2021 12:44:01 GMT  
		Size: 2.8 MB (2769460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140de4b878d8cf1b24ae54ce98ccf0f9791927177a904b5f66c16b580f4f6559`  
		Last Modified: Wed, 12 May 2021 12:44:16 GMT  
		Size: 40.6 MB (40605139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add89bd2f94ae5e2d48399acafa4c1724f536282ded7bd4c79a46fa098041878`  
		Last Modified: Wed, 12 May 2021 12:44:01 GMT  
		Size: 2.6 MB (2565766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:slim` - linux; s390x

```console
$ docker pull pypy@sha256:6d21b2bd3d6a5e46c3ac92b92744b72606011adde0da6050cab8687edebc07db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66360602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0635c753f0c8aaa922960c9444882860ad333eeb805e6aa7ab5b7450642a0d50`
-	Default Command: `["pypy3"]`

```dockerfile
# Wed, 12 May 2021 00:43:38 GMT
ADD file:77af21d863769b75a5f055b85b2c9d6e878f9d77a4122397ae8dde6b69e945c6 in / 
# Wed, 12 May 2021 00:43:42 GMT
CMD ["bash"]
# Wed, 12 May 2021 06:13:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 06:13:02 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 06:13:02 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 06:13:03 GMT
ENV PYPY_VERSION=7.3.4
# Wed, 12 May 2021 06:13:59 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux64.tar.bz2'; 			sha256='09d7298b44a38648a87995ec06e1e093761644e50f547c8bb0b2d7f4fe433548'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-aarch64.tar.bz2'; 			sha256='a4148fa73b74a091e004e1f378b278c0b8830984cbcb91e10fa31fd915c43efe'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-linux32.tar.bz2'; 			sha256='04de1a2e80530f3d74abcf133ec046a0fb12d81956bc043dee8ab4799f3b77eb'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.4-s390x.tar.bz2'; 			sha256='7d6fb180c359a66a158ef6e81eeca88fbabbb62656a1700f425a70db18de2a0f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 12 May 2021 06:14:04 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Wed, 12 May 2021 06:14:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 12 May 2021 06:14:05 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 12 May 2021 06:14:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 12 May 2021 06:14:31 GMT
CMD ["pypy3"]
```

-	Layers:
	-	`sha256:ba4b99e0e723623b64d4ecb8d74102998d32137ea9bcc88b15fd2e4e34b38df9`  
		Last Modified: Wed, 12 May 2021 00:48:03 GMT  
		Size: 25.8 MB (25760171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edb18f5c9b647c5730f0ed0acea816dc6504113efcc15f2b461b4959b4470bc`  
		Last Modified: Wed, 12 May 2021 06:15:48 GMT  
		Size: 2.5 MB (2452407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4572a6625dfad1d2e1321c81085e284ec00994ea434cfc1f27f78c687c286e`  
		Last Modified: Wed, 12 May 2021 06:15:57 GMT  
		Size: 35.6 MB (35581814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc39c4eacd9dae67c1a3cbe3f612c721538fc86504b57de9ba85f6690fa6a4`  
		Last Modified: Wed, 12 May 2021 06:15:48 GMT  
		Size: 2.6 MB (2566210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
