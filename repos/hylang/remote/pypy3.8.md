## `hylang:pypy3.8`

```console
$ docker pull hylang@sha256:305d37bb764cf271a81d259ec24bf5a984a78e04b60b80c1bbe2777cc185bbdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1249; amd64
	-	windows version 10.0.17763.3650; amd64

### `hylang:pypy3.8` - linux; amd64

```console
$ docker pull hylang@sha256:e367e244fb48bf1eedbc5c7197930f7f3620373c5569ba88cd50dabc8b982f70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76471476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc972040b9a2622b1ef8166a4990042a74bd7b16ee1ddb3a3e08e42eeb76de0a`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:48:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:48:13 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 13:48:13 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 13:48:14 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 15 Nov 2022 13:51:50 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux64.tar.bz2'; 			sha256='08be25ec82fc5d23b78563eda144923517daba481a90af0ace7a047c9c9a3c34'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-aarch64.tar.bz2'; 			sha256='5e124455e207425e80731dff317f0432fa0aba1f025845ffca813770e2447e32'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux32.tar.bz2'; 			sha256='4b261516c6c59078ab0c8bd7207327a1b97057b4ec1714ed5e79a026f9efd492'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-s390x.tar.bz2'; 			sha256='c6177a0016c9145c7b99fddb5d74cc2e518ccdb216a6deb51ef6a377510cc930'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Nov 2022 13:51:51 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 15 Nov 2022 13:51:51 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 15 Nov 2022 13:52:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Nov 2022 13:52:04 GMT
CMD ["pypy3"]
# Tue, 15 Nov 2022 23:10:09 GMT
ENV HY_VERSION=0.25.0
# Tue, 15 Nov 2022 23:10:09 GMT
ENV HYRULE_VERSION=0.2.1
# Tue, 15 Nov 2022 23:10:45 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 15 Nov 2022 23:10:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84abf685ee57502df7f40681d28caee5a74e20464f11d3dd27a0de46b1bc879d`  
		Last Modified: Tue, 15 Nov 2022 14:00:22 GMT  
		Size: 1.1 MB (1067972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fc8c82d602bff57d3222f3ae5ffdca664a4f556482c6ded808717342a2c93f`  
		Last Modified: Tue, 15 Nov 2022 14:02:02 GMT  
		Size: 36.8 MB (36788197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f099bf599848f9053a713e0cc49c87317fc9b52aa6968462dbe2ed1c06fe14b8`  
		Last Modified: Tue, 15 Nov 2022 14:01:56 GMT  
		Size: 3.2 MB (3171045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b04f9d587f7bf729accbe0272d01013244f2dd417db6042e253b4fc7230b12`  
		Last Modified: Tue, 15 Nov 2022 23:19:00 GMT  
		Size: 4.0 MB (4031632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:f3217414e155bf2e87975d5351929509e4de933e1e80443520a7c175de2d82cb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.6 MB (72634806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d8db6b7f3cbf2d718604ae13a22e8c5a2cae52a307f78f270ea8d4a1125304f`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 07:10:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 07:10:05 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 07:10:06 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 07:10:06 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 15 Nov 2022 07:13:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux64.tar.bz2'; 			sha256='08be25ec82fc5d23b78563eda144923517daba481a90af0ace7a047c9c9a3c34'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-aarch64.tar.bz2'; 			sha256='5e124455e207425e80731dff317f0432fa0aba1f025845ffca813770e2447e32'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux32.tar.bz2'; 			sha256='4b261516c6c59078ab0c8bd7207327a1b97057b4ec1714ed5e79a026f9efd492'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-s390x.tar.bz2'; 			sha256='c6177a0016c9145c7b99fddb5d74cc2e518ccdb216a6deb51ef6a377510cc930'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Nov 2022 07:13:12 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 15 Nov 2022 07:13:12 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 15 Nov 2022 07:13:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Nov 2022 07:13:23 GMT
CMD ["pypy3"]
# Tue, 15 Nov 2022 21:57:25 GMT
ENV HY_VERSION=0.25.0
# Tue, 15 Nov 2022 21:57:25 GMT
ENV HYRULE_VERSION=0.2.1
# Tue, 15 Nov 2022 21:57:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 15 Nov 2022 21:57:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fb81f010c0b597ef25ca37e0837011236f5c374787890796a881c39db41114`  
		Last Modified: Tue, 15 Nov 2022 07:21:05 GMT  
		Size: 1.1 MB (1055297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244e98520375f7cbe2966f441e11647e9ab8aabf17856eac8c90c327fd4ece15`  
		Last Modified: Tue, 15 Nov 2022 07:22:55 GMT  
		Size: 34.3 MB (34316182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1f9d13c38043b2c6cb3c4c3a7c6ac1d36a3dd140a8cd4fe0c93886df5ec255`  
		Last Modified: Tue, 15 Nov 2022 07:22:50 GMT  
		Size: 3.2 MB (3170941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2573b0c1fb0d573cc735c5fe576a8a1a993dcd4a77f4139b2e0925680b5f312`  
		Last Modified: Tue, 15 Nov 2022 22:06:44 GMT  
		Size: 4.0 MB (4031781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - linux; 386

```console
$ docker pull hylang@sha256:7901f8a3c3d4f8e09d282c9d0dce0433868915a568de6ff5cacf120ec08c3369
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76132041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f48cc006348b912f091e5c80ac3f558378e3d09ebad99675adf733ba5145b2f`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:27 GMT
ADD file:608bec4ba3e2543714da4c5158f3c46a168f63ee69ac3f48bff54474ba9a6f27 in / 
# Tue, 15 Nov 2022 01:41:27 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 09:23:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 09:23:43 GMT
ENV LANG=C.UTF-8
# Tue, 15 Nov 2022 09:23:44 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 15 Nov 2022 09:23:45 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 15 Nov 2022 09:28:18 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux64.tar.bz2'; 			sha256='08be25ec82fc5d23b78563eda144923517daba481a90af0ace7a047c9c9a3c34'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-aarch64.tar.bz2'; 			sha256='5e124455e207425e80731dff317f0432fa0aba1f025845ffca813770e2447e32'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-linux32.tar.bz2'; 			sha256='4b261516c6c59078ab0c8bd7207327a1b97057b4ec1714ed5e79a026f9efd492'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.8-v7.3.9-s390x.tar.bz2'; 			sha256='c6177a0016c9145c7b99fddb5d74cc2e518ccdb216a6deb51ef6a377510cc930'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.8; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 15 Nov 2022 09:28:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 15 Nov 2022 09:28:19 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 15 Nov 2022 09:28:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 15 Nov 2022 09:28:35 GMT
CMD ["pypy3"]
# Tue, 15 Nov 2022 19:46:59 GMT
ENV HY_VERSION=0.25.0
# Tue, 15 Nov 2022 19:46:59 GMT
ENV HYRULE_VERSION=0.2.1
# Tue, 15 Nov 2022 19:47:39 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 15 Nov 2022 19:47:40 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f6a1e975b34444ecb7c6a2b537403fd6b94d2ff3225944ac2ac3b292466e4078`  
		Last Modified: Tue, 15 Nov 2022 01:47:05 GMT  
		Size: 32.4 MB (32392982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf5dfac51abcc2a04456bbcd8d9da11fb9490e8812b2573797c298a1be565da`  
		Last Modified: Tue, 15 Nov 2022 09:41:20 GMT  
		Size: 874.9 KB (874940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9de444ef3d01bc614d8ef2ddece41673973538e81e6f864e7240732b4dfe203`  
		Last Modified: Tue, 15 Nov 2022 09:43:14 GMT  
		Size: 35.9 MB (35880632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d1625ddde9461ad9d07198bfd34e8ad1d5b53dc19855bc31ba3f77c4f964d3c`  
		Last Modified: Tue, 15 Nov 2022 09:43:09 GMT  
		Size: 3.0 MB (2951707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0dce7a24dcfd0e87facda61f3afe0bdcb5deb4ef814c4a69333af2631d6915`  
		Last Modified: Tue, 15 Nov 2022 20:01:00 GMT  
		Size: 4.0 MB (4031780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - windows version 10.0.20348.1249; amd64

```console
$ docker pull hylang@sha256:e0772ab30bb179d6f88ffce8f16dda68e58e76ab0f245b4a3e1674c80ca72ca8
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2532424875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:192964a6be8828482a724c7d6b5d70fdd3c06a5650c6fae487123fc5b518c564`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 05 Nov 2022 07:49:25 GMT
RUN Install update 10.0.20348.1249
# Tue, 08 Nov 2022 18:28:39 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:05:47 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 09 Nov 2022 13:06:31 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 09 Nov 2022 13:06:32 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 09 Nov 2022 13:18:05 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '05022baaa55db2b60880f2422312d9e4025e1267303ac57f33e8253559d0be88'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 09 Nov 2022 13:18:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 09 Nov 2022 13:18:07 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 09 Nov 2022 13:19:28 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 09 Nov 2022 13:19:29 GMT
CMD ["pypy3"]
# Wed, 09 Nov 2022 17:50:28 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 17:50:30 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 17:53:05 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 09 Nov 2022 17:53:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e276673195ed11807395b0da51ac20ef31c925ce955c29ad1bab54f14617c25b`  
		Last Modified: Tue, 08 Nov 2022 19:41:53 GMT  
		Size: 1.0 GB (1007770983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3becc14271944025e3fa6c2ef2689bdfbf09bfc54ec339115d3082df315898e4`  
		Last Modified: Tue, 08 Nov 2022 19:38:57 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6541ee836e2e3b5e29906e7ed7d0a85c066f5da32ed5ba70943ad28207a0b4d`  
		Last Modified: Wed, 09 Nov 2022 13:44:33 GMT  
		Size: 612.3 KB (612286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a1d0927d19e4d589be10f89b90edcdea1904fc695340f76f3ba2df2732b632`  
		Last Modified: Wed, 09 Nov 2022 13:44:35 GMT  
		Size: 15.7 MB (15736946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222d93a6fdd6f63528e5cc09a8547e58fb9a0a6e2b14c1070c38bc6d3db47341`  
		Last Modified: Wed, 09 Nov 2022 13:44:32 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f7d4f12ce013b347dc4f60b7fe44d7fa0bf88f572f154283dbba11e56b4822`  
		Last Modified: Wed, 09 Nov 2022 13:45:30 GMT  
		Size: 26.4 MB (26356388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ff6fe54103ce85bf527b3b07accb676f09c1984e201e1d52fdf06417adacf0`  
		Last Modified: Wed, 09 Nov 2022 13:45:21 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eaf3c9b6385255e6c8deadbd2af94c9de63d5bcfe26646d6ae8e6aead0118d0`  
		Last Modified: Wed, 09 Nov 2022 13:45:21 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f306579330600405d650bcc249c646667f64f0ddbe78a284e938db889519a0`  
		Last Modified: Wed, 09 Nov 2022 13:45:23 GMT  
		Size: 3.2 MB (3197952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c8c72c402dbca63f5de875238f8eed61aa575967c971becf2068278912b650`  
		Last Modified: Wed, 09 Nov 2022 13:45:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed13598cdfb500e2c812047ebe11af6f5138d10b0e335a94598c3156957e6302`  
		Last Modified: Wed, 09 Nov 2022 18:05:10 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ddf1f360b1aefcee3205c46c524a989170e4013a91ad8edf062c8bb6cb12697`  
		Last Modified: Wed, 09 Nov 2022 18:05:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0845bb56152f55f08a2234ce02dd3e6ed393d8d9ebde4d72be8cad72c7c59e3`  
		Last Modified: Wed, 09 Nov 2022 18:05:12 GMT  
		Size: 4.7 MB (4741367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b0723c4c8cd30ca2619ed714bdb1f171a97cea79bf40667eef15324bb9214b`  
		Last Modified: Wed, 09 Nov 2022 18:05:10 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.8` - windows version 10.0.17763.3650; amd64

```console
$ docker pull hylang@sha256:b003eed64d5408250acd6fc38796ffa1881658e36fbbc36ed9f37448347ef92d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2827988028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8ef2f53ae550d73f138f3826fc34ba1526740e4d0ebfe86a4c76c73949d5559`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 13:11:04 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 09 Nov 2022 13:12:34 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 09 Nov 2022 13:12:35 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 09 Nov 2022 13:21:42 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.8-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '05022baaa55db2b60880f2422312d9e4025e1267303ac57f33e8253559d0be88'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.8-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 09 Nov 2022 13:21:43 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 09 Nov 2022 13:21:44 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 09 Nov 2022 13:23:59 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 09 Nov 2022 13:24:00 GMT
CMD ["pypy3"]
# Wed, 09 Nov 2022 17:53:20 GMT
ENV HY_VERSION=0.25.0
# Wed, 09 Nov 2022 17:53:22 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 09 Nov 2022 17:56:36 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 09 Nov 2022 17:56:38 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c0b65cd5d45c257f43399d7e53719e953f8e09ef9ce0ff7f32dce0d5377da7`  
		Last Modified: Wed, 09 Nov 2022 13:45:00 GMT  
		Size: 363.0 KB (363039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619c75c2a1ee945b9b550ca5f4af58f087f2435c24b756a3088a8923d8ee3a8c`  
		Last Modified: Wed, 09 Nov 2022 13:45:02 GMT  
		Size: 15.5 MB (15503027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837ad43d5b0f50b8b879a113a848e2bd674fddf50337d5a6c30858a408e19e42`  
		Last Modified: Wed, 09 Nov 2022 13:44:59 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f3139205533bc7c2158752753d4aa595e2c274ebb2c2796c67c884899faa49`  
		Last Modified: Wed, 09 Nov 2022 13:46:09 GMT  
		Size: 26.1 MB (26130819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15679f04b3389f6f436fb4061e24a2a8ceeb481c496f894533a5110206843c2`  
		Last Modified: Wed, 09 Nov 2022 13:46:01 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d14ad68b3f7c3a9c1ab1382ff1e27bc6e97cc05eba0fd0fad143fd91f4afd8b`  
		Last Modified: Wed, 09 Nov 2022 13:46:01 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44943c0a8a27bce3cd7e3d0e3c775dd73c33e14cf10adc9b27b14f8769f98203`  
		Last Modified: Wed, 09 Nov 2022 13:46:02 GMT  
		Size: 3.0 MB (2978016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab93dfac8900a02509bcdf18d895c5835dab202c388c53278e2fe19496a5757`  
		Last Modified: Wed, 09 Nov 2022 13:46:01 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aec7c29dc25269986eccc33c0f2b96f530c80e63c522ae808ba48b27101f9b4`  
		Last Modified: Wed, 09 Nov 2022 18:05:46 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c5ad6cd24d7768363b31a216e4808c14b7d57b2b962a8d1c72fa326a98061`  
		Last Modified: Wed, 09 Nov 2022 18:05:46 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d02d698237ae1b7b0f6780ee4ed8ad862c90d43cde9ea1b2dad5311134138`  
		Last Modified: Wed, 09 Nov 2022 18:05:48 GMT  
		Size: 4.4 MB (4415357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4414c1e4f1c380c95ad2fd40d368394c615bfc2164ebf1f7edc0fc979a6ff03`  
		Last Modified: Wed, 09 Nov 2022 18:05:46 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
