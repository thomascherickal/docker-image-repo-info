## `hylang:pypy-bullseye`

```console
$ docker pull hylang@sha256:82a20e2628662dab623abddd674412f42fae4eae05d3002e5ea7ce643c5c0df0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; 386

### `hylang:pypy-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:074186ac3cdb3e4af4a98b7adeb575f287c2032d1a2d139b538a808872e4ed2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73800036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d977d15eb74e3b26e67f1371643cb45c31c2a592c733fd1b3fb11a6b1da9e1e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:29 GMT
ADD file:d48a85028743f16ed927507322e3e3beee187fbfadd0b781d4b89de197c64b5b in / 
# Tue, 01 Mar 2022 02:13:29 GMT
CMD ["bash"]
# Wed, 02 Mar 2022 01:40:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 02 Mar 2022 01:40:53 GMT
ENV LANG=C.UTF-8
# Wed, 02 Mar 2022 01:40:53 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 02 Mar 2022 01:40:53 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 08 Mar 2022 05:18:45 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-linux64.tar.bz2'; 			sha256='089f8e3e357d6130815964ddd3507c13bd53e4976ccf0a89b5c36a9a6775a188'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='0210536e9f1841ba283c13b04783394050837bb3e6f4091c9f1bd9c7f2b94b55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-linux32.tar.bz2'; 			sha256='bea4b275decd492af6462157d293dd6fcf08a949859f8aec0959537b40afd032'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-s390x.tar.bz2'; 			sha256='ad53d373d6e275a41ca64da7d88afb6a17e48e7bfb2a6fff92daafdc06da6b90'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Mar 2022 05:18:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 08 Mar 2022 05:18:45 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 08 Mar 2022 05:18:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Mar 2022 05:18:57 GMT
CMD ["pypy3"]
# Tue, 08 Mar 2022 09:18:30 GMT
ENV HY_VERSION=1.0a4
# Tue, 08 Mar 2022 09:18:31 GMT
ENV HYRULE_VERSION=0.1
# Tue, 08 Mar 2022 09:18:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 08 Mar 2022 09:18:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f7a1c6dad28192bd417b78079d6ddc03cbca6d5ea46bba12769b235b6353c00c`  
		Last Modified: Tue, 01 Mar 2022 02:19:23 GMT  
		Size: 31.4 MB (31366396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85840658c910f38522200d385220880921e0966db76c8fa51084fb39dfcbb859`  
		Last Modified: Wed, 02 Mar 2022 01:54:42 GMT  
		Size: 1.1 MB (1066001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f328d57be8b5b52631397af12d1bc6753056e05f12e91b6e48253b5f374c9f`  
		Last Modified: Tue, 08 Mar 2022 05:28:56 GMT  
		Size: 35.9 MB (35944869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e92f19ea6b6b328a732cedd32218ba5b6b246e892bed59a218952d95637f21`  
		Last Modified: Tue, 08 Mar 2022 05:28:50 GMT  
		Size: 2.6 MB (2631453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ad4705f8e5cdc577db8e1b8d144be522a980a18d82e5934550db175dd43920`  
		Last Modified: Tue, 08 Mar 2022 11:04:26 GMT  
		Size: 2.8 MB (2791317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:a9a17ef7b29b2333f086bea2ff70230084626a2e65673c46b0c925f1730e1bb2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74172894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa31c8574f65d314ed205bf0e4906e1dea3b16c72359dc9d5dd89cf8086b70e`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:32 GMT
ADD file:e92ab504d4c0d3bd63da83254e6ca400b607c32e0f5037039648559b91770870 in / 
# Tue, 01 Mar 2022 02:07:33 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 21:18:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:18:08 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 21:18:08 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 21:18:08 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 08 Mar 2022 04:00:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-linux64.tar.bz2'; 			sha256='089f8e3e357d6130815964ddd3507c13bd53e4976ccf0a89b5c36a9a6775a188'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='0210536e9f1841ba283c13b04783394050837bb3e6f4091c9f1bd9c7f2b94b55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-linux32.tar.bz2'; 			sha256='bea4b275decd492af6462157d293dd6fcf08a949859f8aec0959537b40afd032'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.8-s390x.tar.bz2'; 			sha256='ad53d373d6e275a41ca64da7d88afb6a17e48e7bfb2a6fff92daafdc06da6b90'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 08 Mar 2022 04:00:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 08 Mar 2022 04:00:02 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 08 Mar 2022 04:00:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 08 Mar 2022 04:00:14 GMT
CMD ["pypy3"]
# Tue, 08 Mar 2022 04:32:31 GMT
ENV HY_VERSION=1.0a4
# Tue, 08 Mar 2022 04:32:31 GMT
ENV HYRULE_VERSION=0.1
# Tue, 08 Mar 2022 04:32:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 08 Mar 2022 04:32:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:04a87e821be7e4b29d48011b7aa4ff884ca57fd36995cb3b99fd2fc24ac562d8`  
		Last Modified: Tue, 01 Mar 2022 02:15:51 GMT  
		Size: 32.4 MB (32377389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644e74815eb3f18f96bfa2e149a7a246bd0c7482f5681e0a9b0929bad87cdbeb`  
		Last Modified: Tue, 01 Mar 2022 21:39:32 GMT  
		Size: 1.1 MB (1078416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be008a69253632f5895c9ccd68821966b19058b691f4c865a9122e68f4e6aab5`  
		Last Modified: Tue, 08 Mar 2022 04:14:36 GMT  
		Size: 35.3 MB (35294616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d2e6ac145cd77ada3277d01c199e695e840bcc7754ead85c87e0a508b9322`  
		Last Modified: Tue, 08 Mar 2022 04:14:28 GMT  
		Size: 2.6 MB (2631196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22c0b4afaf94f54767009d0daeea2348ff26f7da7c3459e9bbad534670e292b`  
		Last Modified: Tue, 08 Mar 2022 04:40:28 GMT  
		Size: 2.8 MB (2791277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
