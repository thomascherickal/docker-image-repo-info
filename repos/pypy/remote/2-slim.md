## `pypy:2-slim`

```console
$ docker pull pypy@sha256:eaaa6d67999461cef28dfc49a3e29dc2827a395311112dc5684a13a3f4852e8d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-slim` - linux; amd64

```console
$ docker pull pypy@sha256:6c0b0a8d4fe46d5c8de1c7013ab0f0000ca3619e2a88d26f99940854a66b958c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66695362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d229c57dfb57bcbf30d71b5e86db924aef390fd4586fba400301d395f383be82`
-	Default Command: `["pypy"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 10:04:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 10:04:03 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 10:04:03 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 10:04:04 GMT
ENV PYPY_VERSION=7.3.9
# Sat, 28 May 2022 10:12:42 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-linux64.tar.bz2'; 			sha256='172a928b0096a7e00b7d58f523f57300c35c3de7f822491e2a7bc845375c23f8'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-aarch64.tar.bz2'; 			sha256='aff4e4dbab53448f662cd01acb2251571d60f836d2f48382a7d8da54ca5b3442'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-linux32.tar.bz2'; 			sha256='bbf4e7343d43c8217099a9bffeed6a1781f4b5a3e186ed1a0befca65e647aeb9'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-s390x.tar.bz2'; 			sha256='62481dd3c6472393ca05eb3a0880c96e4f5921747157607dbaa772a7369cab77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 28 May 2022 10:12:42 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 28 May 2022 10:12:42 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 28 May 2022 10:12:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 28 May 2022 10:12:51 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20adf0d92d7aa80e69b76bc7ecb920a78fe44e9bef4546d5bfebd98c4a7f677b`  
		Last Modified: Sat, 28 May 2022 10:16:04 GMT  
		Size: 1.1 MB (1066435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02897e74838b27ef7a6a1246fddda2fda871fb022851716474f844bd67ef7602`  
		Last Modified: Sat, 28 May 2022 10:22:04 GMT  
		Size: 32.1 MB (32078562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e29fe27b00f874e73920681b584e2ecbdbbaf3db3cf1c5a8918ad550b89c21`  
		Last Modified: Sat, 28 May 2022 10:21:58 GMT  
		Size: 2.2 MB (2171089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:0ae12145e1392b139b47c2c16a741bd589e4ab0ded1c1e453e4847a816ed4497
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.7 MB (62736753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ef468b5c0811307f47a62bdcdd5fa39426dc6a8d1ab834d68aec0d663d8f7ad`
-	Default Command: `["pypy"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:17:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:17:53 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 07:17:54 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 07:17:55 GMT
ENV PYPY_VERSION=7.3.9
# Sat, 28 May 2022 07:25:42 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-linux64.tar.bz2'; 			sha256='172a928b0096a7e00b7d58f523f57300c35c3de7f822491e2a7bc845375c23f8'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-aarch64.tar.bz2'; 			sha256='aff4e4dbab53448f662cd01acb2251571d60f836d2f48382a7d8da54ca5b3442'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-linux32.tar.bz2'; 			sha256='bbf4e7343d43c8217099a9bffeed6a1781f4b5a3e186ed1a0befca65e647aeb9'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-s390x.tar.bz2'; 			sha256='62481dd3c6472393ca05eb3a0880c96e4f5921747157607dbaa772a7369cab77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 28 May 2022 07:25:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 28 May 2022 07:25:44 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 28 May 2022 07:25:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 28 May 2022 07:25:57 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:094ea76c514fbf36df8927cb522e694cf6ac546efee529dc34b9ebde9a7527bc`  
		Last Modified: Sat, 28 May 2022 07:31:07 GMT  
		Size: 849.6 KB (849570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7fa6b0fb7e150236d0269342ccba133e930783f732934eb6218cc830252f93e`  
		Last Modified: Sat, 28 May 2022 07:35:12 GMT  
		Size: 29.9 MB (29866965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66c015fe34a2d9173f96bb90869cabbe0dc5a7ad07cceb7b779e3fd53da111f`  
		Last Modified: Sat, 28 May 2022 07:35:07 GMT  
		Size: 2.0 MB (1954490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim` - linux; 386

```console
$ docker pull pypy@sha256:7ca6683bf8f7ce20603bd09a214d3aae523a4818477b71761e04b2d0ca3fd35b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.4 MB (64361750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea24ec2367a6475faada627867582bad675d03006d0df61c7ee83ce5a014fe12`
-	Default Command: `["pypy"]`

```dockerfile
# Sat, 28 May 2022 00:39:33 GMT
ADD file:8320d7b95b9f68313e086faff974bb38977e0c9da4984afb6382eb0405742bde in / 
# Sat, 28 May 2022 00:39:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 07:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 07:43:56 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 07:43:57 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 07:43:58 GMT
ENV PYPY_VERSION=7.3.9
# Sat, 28 May 2022 07:55:12 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-linux64.tar.bz2'; 			sha256='172a928b0096a7e00b7d58f523f57300c35c3de7f822491e2a7bc845375c23f8'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-aarch64.tar.bz2'; 			sha256='aff4e4dbab53448f662cd01acb2251571d60f836d2f48382a7d8da54ca5b3442'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-linux32.tar.bz2'; 			sha256='bbf4e7343d43c8217099a9bffeed6a1781f4b5a3e186ed1a0befca65e647aeb9'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.9-s390x.tar.bz2'; 			sha256='62481dd3c6472393ca05eb3a0880c96e4f5921747157607dbaa772a7369cab77'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 28 May 2022 07:55:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 28 May 2022 07:55:13 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 28 May 2022 07:55:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 28 May 2022 07:55:25 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:5e7494d2ee6c81c73ce32f8bde3ea8658c6224c2cc22d7bb01df4bc3d42949aa`  
		Last Modified: Sat, 28 May 2022 00:46:43 GMT  
		Size: 32.4 MB (32390321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f14f1fd9051a4db3428f1ff2f17729e8221800012533d47a1c448d3e09ae8d8`  
		Last Modified: Sat, 28 May 2022 08:01:34 GMT  
		Size: 874.0 KB (874032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c469292eac21e7f93785014bcd89953ce61797fa5b7dad6b2f26524bc39fb9e2`  
		Last Modified: Sat, 28 May 2022 08:08:33 GMT  
		Size: 29.1 MB (29143009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb331ab6c6ab8e96bf17ed8a10088c3c307eb3b2ca44d05029b6ec278968528`  
		Last Modified: Sat, 28 May 2022 08:08:28 GMT  
		Size: 2.0 MB (1954388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
