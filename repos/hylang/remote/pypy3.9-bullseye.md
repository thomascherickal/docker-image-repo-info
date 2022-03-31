## `hylang:pypy3.9-bullseye`

```console
$ docker pull hylang@sha256:79ad9593eb5319268c498e5b542a0add0370c365b5788295cb962b2693522fac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.9-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:1e2657691badbc868539825a2d48e52ff8ee77a827a48f608f2e37f7810a416b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74153781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bae24f49d4375e50475c65c13715ea3e737f8076e0794ba79e6769f8a7d60b5`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:13:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:13:59 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 18:14:00 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 18:14:00 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 29 Mar 2022 18:14:29 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux64.tar.bz2'; 			sha256='129a055032bba700cd1d0acacab3659cf6b7180e25b1b2f730e792f06d5b3010'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='b7282bc4484bceae5bc4cc04e05ee4faf51cb624c8fc7a69d92e5fdf0d0c96aa'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux32.tar.bz2'; 			sha256='a0d18e4e73cc655eb02354759178b8fb161d3e53b64297d05e2fff91f7cf862d'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-s390x.tar.bz2'; 			sha256='37b596bfe76707ead38ffb565629697e9b6fa24e722acc3c632b41ec624f5d95'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 29 Mar 2022 18:14:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 29 Mar 2022 18:14:30 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 29 Mar 2022 18:14:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 29 Mar 2022 18:14:42 GMT
CMD ["pypy3"]
# Wed, 30 Mar 2022 14:00:40 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 14:00:40 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 14:00:45 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 14:00:45 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c5f06096be7051e1473e3f0a584b8f472d494b7c0a0cddefcbc4e7e8444cc`  
		Last Modified: Tue, 29 Mar 2022 18:26:18 GMT  
		Size: 1.1 MB (1066217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b7095a7d7a4f25ef803fe3755ea30ae396522849fde7afaa31dfe89693cbb1`  
		Last Modified: Tue, 29 Mar 2022 18:26:25 GMT  
		Size: 36.2 MB (36235565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb303ab69975f5e55962734b08768eda531a9ad1a8c19bba88357a71b534d6d3`  
		Last Modified: Tue, 29 Mar 2022 18:26:19 GMT  
		Size: 2.6 MB (2639194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e1401828f38c9e41adf273f57abbb4b2cc14a923f77e26a59a3399a3f08dbc`  
		Last Modified: Wed, 30 Mar 2022 14:06:34 GMT  
		Size: 2.8 MB (2834348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:82bc7e75d68fb4436aef8842fdfd2f44eb79cc23567bc15733cae98bd97cfc60
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.7 MB (69725463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b886907192613813a4617a4e85a83249ced39cd6c29532105e6b475a859191e3`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:17 GMT
ADD file:e95289cd39de0f389d09cda9edf8476d5da371bc68d76e820c5e1c310dc54baf in / 
# Tue, 29 Mar 2022 00:43:17 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 04:48:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 04:48:05 GMT
ENV LANG=C.UTF-8
# Wed, 30 Mar 2022 04:48:06 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 04:48:07 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 30 Mar 2022 04:48:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux64.tar.bz2'; 			sha256='129a055032bba700cd1d0acacab3659cf6b7180e25b1b2f730e792f06d5b3010'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-aarch64-portable.tar.bz2'; 			sha256='b7282bc4484bceae5bc4cc04e05ee4faf51cb624c8fc7a69d92e5fdf0d0c96aa'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux32.tar.bz2'; 			sha256='a0d18e4e73cc655eb02354759178b8fb161d3e53b64297d05e2fff91f7cf862d'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-s390x.tar.bz2'; 			sha256='37b596bfe76707ead38ffb565629697e9b6fa24e722acc3c632b41ec624f5d95'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 30 Mar 2022 04:48:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 30 Mar 2022 04:48:48 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 30 Mar 2022 04:49:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 30 Mar 2022 04:49:07 GMT
CMD ["pypy3"]
# Wed, 30 Mar 2022 19:26:05 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 19:26:06 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 19:26:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 19:26:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2203022c5aa978ec114a15a7cdc2c323c65922d3b0a8eab11d50811bb9ae1cfb`  
		Last Modified: Tue, 29 Mar 2022 00:50:04 GMT  
		Size: 30.1 MB (30064311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7648f576816bd0414eaae6bac5eb0e1726477209d4efd73a81c611bf653f5948`  
		Last Modified: Wed, 30 Mar 2022 05:06:52 GMT  
		Size: 849.4 KB (849420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f4d7cabf376a1fde4afff8d55c1732830c4991101c9e08ca09abc90a6405d57`  
		Last Modified: Wed, 30 Mar 2022 05:06:58 GMT  
		Size: 33.6 MB (33553106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d354a5713e0d96118be018a3696aa3a318d18a8d86932af410e003a0cf53f6`  
		Last Modified: Wed, 30 Mar 2022 05:06:53 GMT  
		Size: 2.4 MB (2424377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7559f4cc29719ab6205a207b8acac3a492b287c1b9207db1f62b1aedf105b37`  
		Last Modified: Wed, 30 Mar 2022 19:34:09 GMT  
		Size: 2.8 MB (2834249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:9723937d70ebc02a3157e94db511ed8a9269283b62d85cfe261b99f7c7f2bfe0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.6 MB (75600150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7941d5b516f704baae52620df151e202b19dcb72962133a0b295ec2164acee8c`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:01 GMT
ADD file:d093057c080a13cc4370d0e786857751004b8cd3c93368742512abbee4f1de83 in / 
# Tue, 29 Mar 2022 00:42:01 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:26:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:26:06 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 17:26:07 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 30 Mar 2022 17:41:05 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 30 Mar 2022 17:41:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux64.tar.bz2'; 			sha256='46818cb3d74b96b34787548343d266e2562b531ddbaf330383ba930ff1930ed5'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-aarch64.tar.bz2'; 			sha256='2e1ae193d98bc51439642a7618d521ea019f45b8fb226940f7e334c548d2b4b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux32.tar.bz2'; 			sha256='0de4b9501cf28524cdedcff5052deee9ea4630176a512bdc408edfa30914bae7'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-s390x.tar.bz2'; 			sha256='774dca83bcb4403fb99b3d155e7bd572ef8c52b9fe87a657109f64e75ad71732'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 30 Mar 2022 17:41:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 30 Mar 2022 17:41:40 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 30 Mar 2022 17:41:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 30 Mar 2022 17:41:55 GMT
CMD ["pypy3"]
# Wed, 30 Mar 2022 19:02:07 GMT
ENV HY_VERSION=1.0a4
# Wed, 30 Mar 2022 19:02:08 GMT
ENV HYRULE_VERSION=0.1
# Wed, 30 Mar 2022 19:02:14 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 30 Mar 2022 19:02:15 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:fec59da75229f638ca2878278d3859a1a8b73a20d5c0c043354eb37129ebb8bf`  
		Last Modified: Tue, 29 Mar 2022 00:49:10 GMT  
		Size: 32.4 MB (32389518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bbda215d1a060cee485119134b79bed9bab91b0e247f757fa5b3f8a1248118`  
		Last Modified: Tue, 29 Mar 2022 17:43:18 GMT  
		Size: 873.8 KB (873843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93ef981784180d385844dddfb0760c7f72aca13af4bf03fe2b8739b3a68daeb`  
		Last Modified: Wed, 30 Mar 2022 17:58:22 GMT  
		Size: 36.1 MB (36149013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459b60b08dca8b11ae7ec3a96c3bc1aa70190a73a04b9937a93083aa6f5e7193`  
		Last Modified: Wed, 30 Mar 2022 17:58:17 GMT  
		Size: 3.0 MB (2951402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22a557d616b171c088759e9e3c1c91d90b8646019664ba2296a49d265082560`  
		Last Modified: Wed, 30 Mar 2022 19:06:49 GMT  
		Size: 3.2 MB (3236374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
