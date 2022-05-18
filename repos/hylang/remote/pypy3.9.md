## `hylang:pypy3.9`

```console
$ docker pull hylang@sha256:cfe8af34194400105bb56ab0315a3ae8521c5af0a63a73e8d9e7be3153d0640e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.707; amd64
	-	windows version 10.0.17763.2928; amd64

### `hylang:pypy3.9` - linux; amd64

```console
$ docker pull hylang@sha256:a3c82c8bc2b02304c4470df7da7b49bce451f64ad9ecafa4e03bb8870d63817b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75895708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86b9accb74722531e73ff9093c688ecbb7bbb13512c2941fcc5c828ed49a9271`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:56:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:56:37 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 14:56:37 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 14:56:37 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 14:57:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux64.tar.bz2'; 			sha256='46818cb3d74b96b34787548343d266e2562b531ddbaf330383ba930ff1930ed5'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-aarch64.tar.bz2'; 			sha256='2e1ae193d98bc51439642a7618d521ea019f45b8fb226940f7e334c548d2b4b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux32.tar.bz2'; 			sha256='0de4b9501cf28524cdedcff5052deee9ea4630176a512bdc408edfa30914bae7'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-s390x.tar.bz2'; 			sha256='774dca83bcb4403fb99b3d155e7bd572ef8c52b9fe87a657109f64e75ad71732'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 11 May 2022 14:57:10 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 14:57:10 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 14:57:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 May 2022 14:57:23 GMT
CMD ["pypy3"]
# Thu, 12 May 2022 02:08:33 GMT
ENV HY_VERSION=1.0a4
# Thu, 12 May 2022 02:08:33 GMT
ENV HYRULE_VERSION=0.1
# Thu, 12 May 2022 02:08:39 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 12 May 2022 02:08:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5c63018a4470ab46343e549f63fb48115ea86ff959c6648bd44dbafbc02ddfe`  
		Last Modified: Wed, 11 May 2022 15:09:04 GMT  
		Size: 1.1 MB (1066234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feae7adabb438770214b7fa72f91300cf7e1a5d3647eee83653d1e94ada7ba0e`  
		Last Modified: Wed, 11 May 2022 15:09:11 GMT  
		Size: 37.0 MB (37040825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec8b9e0584e37f0469661b5ba9c5b98d834127a95ea6e70f07b25c2d681dba`  
		Last Modified: Wed, 11 May 2022 15:09:05 GMT  
		Size: 3.2 MB (3170790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea37e406e7f56de490eb1dcc78fe90c08db5e0a79fb6cc12dab3233e976f8e2c`  
		Last Modified: Thu, 12 May 2022 02:12:36 GMT  
		Size: 3.2 MB (3238383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:512bd5adfed187719316649462bd63f8101e7b55bb407536ed273913d6e5aa88
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.5 MB (71456624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db1a28c3a6ddb3688ccafcdd6ebd0991bbe329a4aea265afb5fdfe80d718ded8`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 08:22:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 08:22:38 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 08:22:39 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 08:22:40 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 08:23:10 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux64.tar.bz2'; 			sha256='46818cb3d74b96b34787548343d266e2562b531ddbaf330383ba930ff1930ed5'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-aarch64.tar.bz2'; 			sha256='2e1ae193d98bc51439642a7618d521ea019f45b8fb226940f7e334c548d2b4b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux32.tar.bz2'; 			sha256='0de4b9501cf28524cdedcff5052deee9ea4630176a512bdc408edfa30914bae7'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-s390x.tar.bz2'; 			sha256='774dca83bcb4403fb99b3d155e7bd572ef8c52b9fe87a657109f64e75ad71732'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 11 May 2022 08:23:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 08:23:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 08:23:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 May 2022 08:23:27 GMT
CMD ["pypy3"]
# Thu, 12 May 2022 00:04:03 GMT
ENV HY_VERSION=1.0a4
# Thu, 12 May 2022 00:04:03 GMT
ENV HYRULE_VERSION=0.1
# Thu, 12 May 2022 00:04:10 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 12 May 2022 00:04:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfaefd81ac55b34ce9901ddc18cf199396659fbe9aa9e9d3ab150d457b5d8238`  
		Last Modified: Wed, 11 May 2022 08:39:14 GMT  
		Size: 849.5 KB (849467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0075579f80f1de60c37be2c96c041743eb230710504eff9d6dc9e4ad75610d80`  
		Last Modified: Wed, 11 May 2022 08:39:20 GMT  
		Size: 34.4 MB (34352954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44fb6b00c455b1aedc4f0089c443e995c88631b2e8ec41980c229e14071bd34f`  
		Last Modified: Wed, 11 May 2022 08:39:14 GMT  
		Size: 3.0 MB (2951540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ef082ac5e9bf0088651a7c3d6a3bfa5c607008495be86f9c1f60093609c591`  
		Last Modified: Thu, 12 May 2022 00:09:55 GMT  
		Size: 3.2 MB (3236970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - linux; 386

```console
$ docker pull hylang@sha256:a24e6dee80369c132da05bd248150a11703ee21804d0b61d8ec600083f18a947
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75601259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb531a74e681bc2c6fadada787437d0378ca33d8b4cdd82d17799c03a7421fc3`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 10:42:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 10:42:10 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 10:42:11 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 10:42:12 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 10:42:46 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux64.tar.bz2'; 			sha256='46818cb3d74b96b34787548343d266e2562b531ddbaf330383ba930ff1930ed5'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-aarch64.tar.bz2'; 			sha256='2e1ae193d98bc51439642a7618d521ea019f45b8fb226940f7e334c548d2b4b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux32.tar.bz2'; 			sha256='0de4b9501cf28524cdedcff5052deee9ea4630176a512bdc408edfa30914bae7'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-s390x.tar.bz2'; 			sha256='774dca83bcb4403fb99b3d155e7bd572ef8c52b9fe87a657109f64e75ad71732'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 11 May 2022 10:42:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 10:42:47 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 10:43:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 May 2022 10:43:02 GMT
CMD ["pypy3"]
# Wed, 11 May 2022 19:57:34 GMT
ENV HY_VERSION=1.0a4
# Wed, 11 May 2022 19:57:35 GMT
ENV HYRULE_VERSION=0.1
# Wed, 11 May 2022 19:57:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 11 May 2022 19:57:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e43e2675131b3496a5f30db378ca53620a532d814a5fea2e9e5824ba6a3e1e1`  
		Last Modified: Wed, 11 May 2022 10:59:50 GMT  
		Size: 873.8 KB (873842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1669595f49239feb3801ad0b6e6b5c3f042d6fba95161ff52cdef936c91b26c1`  
		Last Modified: Wed, 11 May 2022 10:59:56 GMT  
		Size: 36.1 MB (36149340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9421ccddb58779dda5b9e6a29fa1f579774820ead25a0d31a037c75e4587f27`  
		Last Modified: Wed, 11 May 2022 10:59:51 GMT  
		Size: 3.0 MB (2951385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:539c46b608c806612732419291d322da7d8c846a31a30922ea93faaa7a286a56`  
		Last Modified: Wed, 11 May 2022 20:03:39 GMT  
		Size: 3.2 MB (3236916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - windows version 10.0.20348.707; amd64

```console
$ docker pull hylang@sha256:41e2ff75c1bb969ca8297c38fdac39af8cd30b5cae6113de7740620dc5067bd8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2287494304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c3d8971014df8037d9214dc465e757cbc20656acb947bd18642ff2055a9a85`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 05 May 2022 03:02:27 GMT
RUN Install update 10.0.20348.707
# Tue, 10 May 2022 17:36:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 12:04:19 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 11 May 2022 12:04:48 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:04:49 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 12:05:43 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = 'be48ab42f95c402543a7042c999c9433b17e55477c847612c8733a583ca6dff5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:05:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 12:05:46 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 12:07:00 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:07:01 GMT
CMD ["pypy"]
# Wed, 18 May 2022 12:29:13 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 12:29:14 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 12:30:05 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 18 May 2022 12:30:07 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:12fb50a031bdc8d2b65d86d694a4ed20e937852ed1bd3c433d8f2f60279cecc7`  
		Size: 800.7 MB (800671635 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e88d40042c6dc2d74dace22d66dfa64aeebe4cd3eec90e5081400debd9281a35`  
		Last Modified: Tue, 10 May 2022 18:16:13 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9856212015d3344ddeccfb9bc86716cbb73e023f931ec57f649eba5f92bfe3ba`  
		Last Modified: Wed, 18 May 2022 12:06:29 GMT  
		Size: 604.4 KB (604405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f806e77cf758e99e339f11b825191b78ac074c0e15df57c95ffa35234212c710`  
		Last Modified: Wed, 18 May 2022 12:06:44 GMT  
		Size: 15.7 MB (15727162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b939be8ce96ba83671598e7fbe27585667afa6663b3f00274620dbe8bc53f82e`  
		Last Modified: Wed, 18 May 2022 12:06:28 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407543b3efcf7d8911e75254ea58a66808670289151e11ff1ea4d54ca3843358`  
		Last Modified: Wed, 18 May 2022 12:06:36 GMT  
		Size: 26.6 MB (26582183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350f39fe407028ac6eb87456b7e01934258abea006dda522307037f79e25f11a`  
		Last Modified: Wed, 18 May 2022 12:06:24 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf16f4b08e106fded0f27bead695f7f6ffa52bbf6484379f49a6d4a9325e47c2`  
		Last Modified: Wed, 18 May 2022 12:06:24 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33833c97512f3520ddd1e5c8f712ac1c30fbe905b2e40344b29092dc8ca73ea2`  
		Last Modified: Wed, 18 May 2022 12:06:28 GMT  
		Size: 3.2 MB (3206853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4f3d65a093b4c0e81aab03304610a1524c06faed031eb20138c04c91b13179`  
		Last Modified: Wed, 18 May 2022 12:06:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9116b334e0af3e54bc91341b3996bb9c709104c3692dcdbd227277904daba439`  
		Last Modified: Wed, 18 May 2022 12:36:36 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e05c754f46dc6308bd333cdf28ebd3099596a16dbd4a10c6360819f62adf81cb`  
		Last Modified: Wed, 18 May 2022 12:36:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85558a3b25e9575d15750a2cbd5fb871094f42f53bb6fd5f541453ed310f794`  
		Last Modified: Wed, 18 May 2022 12:36:37 GMT  
		Size: 3.8 MB (3827176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d178d97dfaafe5c94c6a4c7a227550bf5acbdb8a3551366599ebcf28c058147f`  
		Last Modified: Wed, 18 May 2022 12:36:36 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - windows version 10.0.17763.2928; amd64

```console
$ docker pull hylang@sha256:5a4909c47e2ada46321c773837f973aa16ae369ff98dad01e43b4483825258f2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2553019790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b94520994d3a95323ed08174358ff7377f29fed8be2a9d8cedb951ff17a2255`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 12:08:19 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 11 May 2022 12:09:16 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:09:17 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 11 May 2022 12:10:41 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = 'be48ab42f95c402543a7042c999c9433b17e55477c847612c8733a583ca6dff5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:10:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 May 2022 12:10:44 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 May 2022 12:12:12 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 11 May 2022 12:12:14 GMT
CMD ["pypy"]
# Wed, 18 May 2022 12:30:15 GMT
ENV HY_VERSION=1.0a4
# Wed, 18 May 2022 12:30:15 GMT
ENV HYRULE_VERSION=0.1
# Wed, 18 May 2022 12:31:28 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 18 May 2022 12:31:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d2387a2c2f291aa6063bfd517e16a53cf5edf957859e74eee166038705a109`  
		Last Modified: Wed, 18 May 2022 12:07:02 GMT  
		Size: 486.1 KB (486116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d60b357cba6426f215b9ba70764743afe3d54199a19271133a07e58873f0586`  
		Last Modified: Wed, 18 May 2022 12:07:05 GMT  
		Size: 15.5 MB (15495601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11d7014821b4c2a807d4879721798652cbfb821be75a3e58f40ebdd1a637aa58`  
		Last Modified: Wed, 18 May 2022 12:07:01 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77194bc8ff6dbe3ea0fd1978797df82485b5d7f4d66785cc74123910dd55c1e5`  
		Last Modified: Wed, 18 May 2022 12:07:29 GMT  
		Size: 26.4 MB (26365348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f9debfd3eff6122e1c748a3c3d21de7a7790f0d7ef53e5441db0cb49c174bd`  
		Last Modified: Wed, 18 May 2022 12:06:59 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b954dbecc3f9dabb3f05876da11ea6a4904358977003713b41b5d45a95cfb8b`  
		Last Modified: Wed, 18 May 2022 12:06:59 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cab2ab43cce2d0b190f7de2e7b867436db0a41068bab1d7037fabf1b6b68f52`  
		Last Modified: Wed, 18 May 2022 12:07:02 GMT  
		Size: 3.0 MB (2985169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0195e871b9184b400a8c98450dbafed679562b1aa53990f9e3a738b477bc274`  
		Last Modified: Wed, 18 May 2022 12:06:59 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39ad61e77e740752d89d4ab371d4fd2cc7738edca6359eb335a6fb8752ad21b`  
		Last Modified: Wed, 18 May 2022 12:36:49 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d7b275fe5b495417dd408d581e62c450fbb5989ba5e42ffea6dd4aded2ff31`  
		Last Modified: Wed, 18 May 2022 12:36:49 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fbff08da09b3627d8700fd63337b4539a175c06db8efb2a9446ce6ad1c771d`  
		Last Modified: Wed, 18 May 2022 12:36:50 GMT  
		Size: 3.6 MB (3620561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cabd24118271e29c827aa6ae11af9590c4fb3a202e8eff5230d84010754635d8`  
		Last Modified: Wed, 18 May 2022 12:36:49 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
