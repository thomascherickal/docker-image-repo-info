## `hylang:pypy3.7-buster`

```console
$ docker pull hylang@sha256:6603900735e82fedb046cc30f7c120aeb0f46ec986b61dd55a94062658a8fc41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `hylang:pypy3.7-buster` - linux; amd64

```console
$ docker pull hylang@sha256:b3e9f2dd29227dc96591dd053f578f2b2cd219c67b4c576fd5ec3c944e109e17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.7 MB (71664627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629b1387037202a1fe0053b0047fdbb284185196478b580096f6e9dc04aa44c8`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 21 Dec 2021 01:23:04 GMT
ADD file:bd5c9e0e0145fe33beee9d73615cc89b5c5459bb84ea164cb1bbd8c999f0c2e4 in / 
# Tue, 21 Dec 2021 01:23:04 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 03:08:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:08:35 GMT
ENV LANG=C.UTF-8
# Tue, 21 Dec 2021 03:08:35 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 03:08:35 GMT
ENV PYPY_VERSION=7.3.7
# Tue, 21 Dec 2021 03:12:50 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux64.tar.bz2'; 			sha256='8332f923755441fedfe4767a84601c94f4d6f8475384406cb5f259ad8d0b2002'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-aarch64.tar.bz2'; 			sha256='a1a84882525dd574c4b051b66e9b7ef0e132392acc2f729420d7825f96835216'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux32.tar.bz2'; 			sha256='0ab9e2e8ae1ac463bb811b9d3ba24d138f41f7378c17ca9e2d8dee51bf151d19'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-s390x.tar.bz2'; 			sha256='7f91efc65a69e727519cc885ca6351f4bfdd6b90580dced2fdcc9ae1bf10013b'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 21 Dec 2021 03:12:50 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 21 Dec 2021 03:12:51 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 21 Dec 2021 03:13:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 21 Dec 2021 03:13:03 GMT
CMD ["pypy3"]
# Tue, 11 Jan 2022 00:22:08 GMT
ENV HY_VERSION=1.0a4
# Tue, 11 Jan 2022 00:22:08 GMT
ENV HYRULE_VERSION=0.1
# Tue, 11 Jan 2022 00:22:13 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 11 Jan 2022 00:22:14 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:72a69066d2febc34d8f3dbcb645f7b851a57e9681322ece7ad8007503b783c19`  
		Last Modified: Tue, 21 Dec 2021 01:28:32 GMT  
		Size: 27.2 MB (27153723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9042c4fc606d343774abe31f261f6cc338214f41a992f15ef03e2cd915decfdb`  
		Last Modified: Tue, 21 Dec 2021 03:19:41 GMT  
		Size: 2.8 MB (2757916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40668b105069d1d95ea395aeeec9998fb8d5a2e539d1781771722c4ceeb354a9`  
		Last Modified: Tue, 21 Dec 2021 03:22:25 GMT  
		Size: 36.9 MB (36852776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762b3ff0af940345222bf423da0eb487c2de7ac548556e035c4d687de56f944f`  
		Last Modified: Tue, 21 Dec 2021 03:22:18 GMT  
		Size: 2.4 MB (2367097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3e19a84be7dec4743cb588f57b14783b140d0433c1774da3e7f2b0df66ac526`  
		Last Modified: Tue, 11 Jan 2022 00:29:25 GMT  
		Size: 2.5 MB (2533115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:50d44ed8a57dd4529f51ae75cc8d9187da0ca40bc7944efa10d1c755d81169d0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66342448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31f106884f6229be12c53e449d09b1ca23ce442d009b228e2a4e57293b399b25`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:56 GMT
ADD file:796bc43a948899ba53bddebf7f613769fe96e8ea3a27eb7143d079c7a166ab01 in / 
# Wed, 26 Jan 2022 01:42:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 07:18:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 07:18:25 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 07:18:26 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 07:18:27 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 26 Jan 2022 07:22:15 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux64.tar.bz2'; 			sha256='8332f923755441fedfe4767a84601c94f4d6f8475384406cb5f259ad8d0b2002'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-aarch64.tar.bz2'; 			sha256='a1a84882525dd574c4b051b66e9b7ef0e132392acc2f729420d7825f96835216'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux32.tar.bz2'; 			sha256='0ab9e2e8ae1ac463bb811b9d3ba24d138f41f7378c17ca9e2d8dee51bf151d19'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-s390x.tar.bz2'; 			sha256='7f91efc65a69e727519cc885ca6351f4bfdd6b90580dced2fdcc9ae1bf10013b'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 26 Jan 2022 07:22:15 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 26 Jan 2022 07:22:16 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 26 Jan 2022 07:22:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Jan 2022 07:22:34 GMT
CMD ["pypy3"]
# Thu, 27 Jan 2022 01:40:55 GMT
ENV HY_VERSION=1.0a4
# Thu, 27 Jan 2022 01:40:56 GMT
ENV HYRULE_VERSION=0.1
# Thu, 27 Jan 2022 01:41:02 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 27 Jan 2022 01:41:03 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4c7c9f6f1115fd4f35807a2f6c1375759365a991748aee0111873e55255f150b`  
		Last Modified: Wed, 26 Jan 2022 01:49:55 GMT  
		Size: 25.9 MB (25923216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb9bd4618813bb4cc63b8b9568068380b3faffa783988a338e688fd67defdee`  
		Last Modified: Wed, 26 Jan 2022 07:30:10 GMT  
		Size: 2.6 MB (2626740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fe215c7b57b6dae4e8c1ce2b8d948d368ff0386c97236d3bf6b720599c6715`  
		Last Modified: Wed, 26 Jan 2022 07:32:55 GMT  
		Size: 33.1 MB (33104151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7af1fc377228dfc3ae58238cccb34f50479f8a7d5d11779c481f7c4e00904d`  
		Last Modified: Wed, 26 Jan 2022 07:32:49 GMT  
		Size: 2.2 MB (2154828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdebe979f292e9097e295f744d4b95c27face0b2741826c78a0ff31676707a34`  
		Last Modified: Thu, 27 Jan 2022 01:46:22 GMT  
		Size: 2.5 MB (2533513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; 386

```console
$ docker pull hylang@sha256:13047cd1a0b866ca85a46a7a4327368ad11dcf1a9d4dae28f277208e7ec235fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74225672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f19f4e2eb1550a9df88bbbbcca4558dab1d6be74102312c2e84944ba29201e`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:30 GMT
ADD file:0d3811120feb1258b2cbe48be0a91ae3389643fb759b10b83b6534ebca8cf795 in / 
# Wed, 26 Jan 2022 01:40:31 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 21:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 21:18:09 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 21:18:09 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 21:18:10 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 26 Jan 2022 21:22:25 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux64.tar.bz2'; 			sha256='8332f923755441fedfe4767a84601c94f4d6f8475384406cb5f259ad8d0b2002'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-aarch64.tar.bz2'; 			sha256='a1a84882525dd574c4b051b66e9b7ef0e132392acc2f729420d7825f96835216'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux32.tar.bz2'; 			sha256='0ab9e2e8ae1ac463bb811b9d3ba24d138f41f7378c17ca9e2d8dee51bf151d19'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-s390x.tar.bz2'; 			sha256='7f91efc65a69e727519cc885ca6351f4bfdd6b90580dced2fdcc9ae1bf10013b'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 26 Jan 2022 21:22:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 26 Jan 2022 21:22:26 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 26 Jan 2022 21:22:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Jan 2022 21:22:46 GMT
CMD ["pypy3"]
# Thu, 27 Jan 2022 12:28:32 GMT
ENV HY_VERSION=1.0a4
# Thu, 27 Jan 2022 12:28:33 GMT
ENV HYRULE_VERSION=0.1
# Thu, 27 Jan 2022 12:28:38 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 27 Jan 2022 12:28:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:79e14f2e0ab2370ab81617ee0b4757c6c2e55d326ad5c7b5290a5068e50176df`  
		Last Modified: Wed, 26 Jan 2022 01:50:05 GMT  
		Size: 27.8 MB (27804600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cb884b98f263b1de2aced2aed126582e71db9d6a378fa06c40f9feda03e727`  
		Last Modified: Wed, 26 Jan 2022 21:32:40 GMT  
		Size: 2.8 MB (2769426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85316641ceb1ca67ab3e1de5bc1311e47f2ef0d01c6569f03f206ca3f8088a1a`  
		Last Modified: Wed, 26 Jan 2022 21:36:19 GMT  
		Size: 38.8 MB (38751607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b237490ef4e0f21d044b89ef1366f638aa8a1093ad28651504c2e01121f572e`  
		Last Modified: Wed, 26 Jan 2022 21:36:09 GMT  
		Size: 2.4 MB (2366878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c85232d2ca81c616d1deb3cd0ac6560a4b83c60bb75bee5b139eef8a0ebd83f`  
		Last Modified: Thu, 27 Jan 2022 12:35:07 GMT  
		Size: 2.5 MB (2533161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.7-buster` - linux; s390x

```console
$ docker pull hylang@sha256:21e31e229cbd50dac7e45c6403840c4067f83811d7b1dcdbade741de38c05970
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67561842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd29096bf2ea05e55bdb88889b94272c823b73a9434dff0369df823c2849b3c7`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:43 GMT
ADD file:27d2ddf8a67fd6bce8ec2eb1a83419b88265bc9b1640c3055d6b36b44586b03a in / 
# Wed, 26 Jan 2022 01:41:44 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 10:38:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 10:38:41 GMT
ENV LANG=C.UTF-8
# Wed, 26 Jan 2022 10:38:41 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Jan 2022 10:38:42 GMT
ENV PYPY_VERSION=7.3.7
# Wed, 26 Jan 2022 10:40:17 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux64.tar.bz2'; 			sha256='8332f923755441fedfe4767a84601c94f4d6f8475384406cb5f259ad8d0b2002'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-aarch64.tar.bz2'; 			sha256='a1a84882525dd574c4b051b66e9b7ef0e132392acc2f729420d7825f96835216'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-linux32.tar.bz2'; 			sha256='0ab9e2e8ae1ac463bb811b9d3ba24d138f41f7378c17ca9e2d8dee51bf151d19'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.7-s390x.tar.bz2'; 			sha256='7f91efc65a69e727519cc885ca6351f4bfdd6b90580dced2fdcc9ae1bf10013b'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 26 Jan 2022 10:40:19 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 26 Jan 2022 10:40:19 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 26 Jan 2022 10:40:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 26 Jan 2022 10:40:28 GMT
CMD ["pypy3"]
# Wed, 26 Jan 2022 22:44:48 GMT
ENV HY_VERSION=1.0a4
# Wed, 26 Jan 2022 22:44:48 GMT
ENV HYRULE_VERSION=0.1
# Wed, 26 Jan 2022 22:44:52 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 26 Jan 2022 22:44:52 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:72d32cf8184f85de685e3d4f0354385b1ef6ed1ff7ce95a31b81ad20d6ae77c1`  
		Last Modified: Wed, 26 Jan 2022 01:47:30 GMT  
		Size: 25.8 MB (25769120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2142db46bdaa54bac36d940e1cd37c842bab09c0fab19e55feec6f116da56cc1`  
		Last Modified: Wed, 26 Jan 2022 10:41:42 GMT  
		Size: 2.5 MB (2452749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35c2623cc1b76a2d54ec995ea39576b7d281465466f1268b37de628e2897f65`  
		Last Modified: Wed, 26 Jan 2022 10:42:29 GMT  
		Size: 34.4 MB (34439680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2868f10635d3651d42d15fe576f1413a6c43cb81ac3bb1474a0d928bbaae308`  
		Last Modified: Wed, 26 Jan 2022 10:42:23 GMT  
		Size: 2.4 MB (2367417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb9d07c8ca129d2b729713ca2dc89d31b6369a535625319cac3041d761132d5`  
		Last Modified: Wed, 26 Jan 2022 22:48:57 GMT  
		Size: 2.5 MB (2532876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
