## `hylang:pypy3.8-bullseye`

```console
$ docker pull hylang@sha256:590ba9237389d129d09122addf4e5596c5818c97f6270862ac69f06411db1ad7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.8-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:78ecf1d03e2f65f3fddf8682b064099828f5e9a7dfcafd47cf87ec073fbd8c28
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75721392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cddb61fb315dc5baf060f0776ef46d08f7837b3f37203d585e8d50f8f11cab6`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 15:07:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 15:07:00 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 15:07:00 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 15:07:00 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 23 Mar 2023 15:10:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 23 Mar 2023 15:10:34 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 23 Mar 2023 15:10:34 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 23 Mar 2023 15:10:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 23 Mar 2023 15:10:46 GMT
CMD ["pypy3"]
# Thu, 23 Mar 2023 18:10:27 GMT
ENV HY_VERSION=0.26.0
# Thu, 23 Mar 2023 18:10:27 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 23 Mar 2023 18:11:01 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Mar 2023 18:11:02 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b89d363cc686e059b8581126fd0f2bb2f4cf606ee302b20cbc37f300263846a`  
		Last Modified: Thu, 23 Mar 2023 15:15:12 GMT  
		Size: 1.1 MB (1066500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a02a1cac48f7c5f86600916544b1b2495c1ea7c613d16b34fdf85425de7190`  
		Last Modified: Thu, 23 Mar 2023 15:17:09 GMT  
		Size: 35.9 MB (35891413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6c1c47dd7508e19f69e265ef4514d53ffde4e1360bc074072245204fdb5b51`  
		Last Modified: Thu, 23 Mar 2023 15:17:03 GMT  
		Size: 3.2 MB (3194792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f96ba0ce8a999300db99038e078abbddfc532b08d77b0a05bfc5cfbc50620a1`  
		Last Modified: Thu, 23 Mar 2023 18:19:09 GMT  
		Size: 4.2 MB (4157282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:d53148879acf07c46a656fc53bdf7352a1a42e04e099b0e51c80fe16d8b8aeb6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71897929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a8c1932971ed9268d14a8fffb58886e3129389888b236216acd76a2b98baa8`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 06:02:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 06:02:54 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 06:02:54 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 06:02:54 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 23 Mar 2023 06:04:52 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 23 Mar 2023 06:04:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 23 Mar 2023 06:04:53 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 23 Mar 2023 06:05:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 23 Mar 2023 06:05:03 GMT
CMD ["pypy3"]
# Thu, 23 Mar 2023 15:12:20 GMT
ENV HY_VERSION=0.26.0
# Thu, 23 Mar 2023 15:12:20 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 23 Mar 2023 15:12:54 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Mar 2023 15:12:54 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d1e54406be8d5f44fc875b900ad3f0fcac16df20b38c231eb4ab849a94be046`  
		Last Modified: Thu, 23 Mar 2023 06:07:20 GMT  
		Size: 1.1 MB (1054057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a126d10b97a582885ac3b1bc54624683c6deba3dce6c7836161cc2e23f647980`  
		Last Modified: Thu, 23 Mar 2023 06:08:29 GMT  
		Size: 33.4 MB (33429094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830d81d244b41f6d1b01580487d740e951c3acd538826702eaa78cfb4f715fe4`  
		Last Modified: Thu, 23 Mar 2023 06:08:25 GMT  
		Size: 3.2 MB (3194608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df4aa5d63d3a616cf3d4a8dd800753976455b2adb1a72c5ccf19c49571185c0e`  
		Last Modified: Thu, 23 Mar 2023 15:20:54 GMT  
		Size: 4.2 MB (4157470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:99a81cead465bb3ec1dde0bce6e65b4f79cd77261ad6f7a95a162b109ca1d519
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.0 MB (75030303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa8714bb2320c0cd0d0ed6229c094f4693a5c39e6dcf6247754a719f8bbb6e08`
-	Default Command: `["hy"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 19:28:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 19:28:17 GMT
ENV LANG=C.UTF-8
# Thu, 23 Mar 2023 19:28:17 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Mar 2023 19:28:17 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 23 Mar 2023 19:31:51 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux64.tar.bz2'; 			sha256='470330e58ac105c094041aa07bb05676b06292bc61409e26f5c5593ebb2292d9'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-aarch64.tar.bz2'; 			sha256='9a2fa0b8d92b7830aa31774a9a76129b0ff81afbd22cd5c41fbdd9119e859f55'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-linux32.tar.bz2'; 			sha256='a79b31fce8f5bc1f9940b6777134189a1d3d18bda4b1c830384cda90077c9176'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.11-s390x.tar.bz2'; 			sha256='eab7734d86d96549866f1cba67f4f9c73c989f6a802248beebc504080d4c3fcd'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 23 Mar 2023 19:31:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 23 Mar 2023 19:31:52 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 23 Mar 2023 19:32:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 23 Mar 2023 19:32:05 GMT
CMD ["pypy3"]
# Thu, 23 Mar 2023 23:55:53 GMT
ENV HY_VERSION=0.26.0
# Thu, 23 Mar 2023 23:55:53 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 23 Mar 2023 23:56:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 23 Mar 2023 23:56:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f9901e33609ef3c21f4da83b79637ca7211c193ec5e6e4548b37ce316bf09b`  
		Last Modified: Thu, 23 Mar 2023 19:36:30 GMT  
		Size: 1.1 MB (1078979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9199e8b89f6fa25bf5b3e756fe3df73538120ed032706dba1e613d6e0fe57bc0`  
		Last Modified: Thu, 23 Mar 2023 19:38:37 GMT  
		Size: 34.2 MB (34203642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607d9c8fa6b1eea4f2874c3e6105f9dbfbc7ebb4d2f72f0a7c0de1e4e9ccd893`  
		Last Modified: Thu, 23 Mar 2023 19:38:30 GMT  
		Size: 3.2 MB (3194457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddf1fabf09774fcc074a9ae2cd5b69a8de5aa9d93f16081f1896046a8cd1555`  
		Last Modified: Fri, 24 Mar 2023 00:05:12 GMT  
		Size: 4.2 MB (4156948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
