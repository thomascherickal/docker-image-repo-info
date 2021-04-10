## `pypy:2-slim`

```console
$ docker pull pypy@sha256:aa83e195d7153468a6e76a577fa36d1e40249b57c54a754ce83e34b8014f5720
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-slim` - linux; amd64

```console
$ docker pull pypy@sha256:24771591ef344283c79082d02db1686b71c273d9b8b25512464ce2519e4a889b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64941600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9f9cb499f7ee1516cf222eaeb567327a2de6be566e08cf15eeb83e5d7616ed4`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:29 GMT
ADD file:b797b4d60ad7954e98ad71574c4fc90ad3da9a5c250112373e92e2af3056e581 in / 
# Tue, 30 Mar 2021 21:49:30 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:50:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:50:33 GMT
ENV LANG=C.UTF-8
# Tue, 30 Mar 2021 22:50:34 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Apr 2021 20:00:31 GMT
ENV PYPY_VERSION=7.3.4
# Thu, 08 Apr 2021 20:02:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-linux64.tar.bz2'; 			sha256='d3f7b0625e770d9be62201765d7d2316febc463372fba9c93a12969d26ae03dd'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-aarch64.tar.bz2'; 			sha256='9e741162ce486b14fbcf5aa377796d26b0529a9352fb602ee8b66c005f8420d1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-linux32.tar.bz2'; 			sha256='653cc3f0612399e494021027f4463d62639dffa4345736a16d0704f3f8a61d5f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 08 Apr 2021 20:02:01 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Thu, 08 Apr 2021 20:02:02 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 08 Apr 2021 20:02:02 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 08 Apr 2021 20:02:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 08 Apr 2021 20:02:14 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:75646c2fb4101d306585c9b106be1dfa7d82720baabe1c75b64d759ea8adf341`  
		Last Modified: Tue, 30 Mar 2021 21:54:15 GMT  
		Size: 27.1 MB (27139293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326f7a54e58461c3962f5ab9b1da47b2e5f4d723d35580eec0dfeb97f00de3ff`  
		Last Modified: Tue, 30 Mar 2021 22:55:31 GMT  
		Size: 2.8 MB (2757692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b84ad60d4697d775c6140491f088668974b439fc4fe9d7ea223691042e04f7`  
		Last Modified: Thu, 08 Apr 2021 20:05:56 GMT  
		Size: 32.8 MB (32805599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4631a85396d928cc896a97dd79f53e3d33d2505c2467e2c67ab0938397fb04f`  
		Last Modified: Thu, 08 Apr 2021 20:05:48 GMT  
		Size: 2.2 MB (2239016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:669388f6c10c6fa45c1f1b73fe991eb688a1e8a75cadeb816835c28fc3f8a035
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61385714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e924c8176cd3c7b48d370125de22469c6772cdcb857e11cd7de13a09998e127f`
-	Default Command: `["pypy"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 10:59:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 10:59:31 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 10:59:31 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 10:59:32 GMT
ENV PYPY_VERSION=7.3.4
# Sat, 10 Apr 2021 11:03:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-linux64.tar.bz2'; 			sha256='d3f7b0625e770d9be62201765d7d2316febc463372fba9c93a12969d26ae03dd'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-aarch64.tar.bz2'; 			sha256='9e741162ce486b14fbcf5aa377796d26b0529a9352fb602ee8b66c005f8420d1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-linux32.tar.bz2'; 			sha256='653cc3f0612399e494021027f4463d62639dffa4345736a16d0704f3f8a61d5f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 10 Apr 2021 11:03:14 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Sat, 10 Apr 2021 11:03:17 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 10 Apr 2021 11:03:18 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 10 Apr 2021 11:03:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 10 Apr 2021 11:03:48 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33eeb66cbe9658b76a975f836346c35755c240ebca8217427c30173634860e16`  
		Last Modified: Sat, 10 Apr 2021 11:05:15 GMT  
		Size: 2.6 MB (2626374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fc54f0d300d7260d9ebde1c1d399e2f86ae20f64aefc11e5c3b42ef3d5220ea`  
		Last Modified: Sat, 10 Apr 2021 11:06:36 GMT  
		Size: 30.6 MB (30615825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4bda721d50f658f08c8ceadcd5379535125cf4eb312428cc497d0a7755ec33`  
		Last Modified: Sat, 10 Apr 2021 11:06:29 GMT  
		Size: 2.2 MB (2238933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-slim` - linux; 386

```console
$ docker pull pypy@sha256:51b757bd0c6fa61dcb5dbe19c62fcfc0601f353a623386e1d031151f420b0c95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.0 MB (63039995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70d9e909bc8a66cf3372c0f2d73720c76785195506e7e71d8e8476343eab0017`
-	Default Command: `["pypy"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:07:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:07:12 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 01:07:12 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 01:07:12 GMT
ENV PYPY_VERSION=7.3.4
# Sat, 10 Apr 2021 01:08:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-linux64.tar.bz2'; 			sha256='d3f7b0625e770d9be62201765d7d2316febc463372fba9c93a12969d26ae03dd'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-aarch64.tar.bz2'; 			sha256='9e741162ce486b14fbcf5aa377796d26b0529a9352fb602ee8b66c005f8420d1'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.4-linux32.tar.bz2'; 			sha256='653cc3f0612399e494021027f4463d62639dffa4345736a16d0704f3f8a61d5f'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 10 Apr 2021 01:08:44 GMT
ENV PYTHON_PIP_VERSION=20.3.4
# Sat, 10 Apr 2021 01:08:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 10 Apr 2021 01:08:44 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 10 Apr 2021 01:08:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $PYTHON_PIP_VERSION" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 10 Apr 2021 01:08:57 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c61c37f00ee5e12d61f2fa53765dba4639a1276ccfeaa02c264cec3061c35dad`  
		Last Modified: Sat, 10 Apr 2021 01:11:28 GMT  
		Size: 2.8 MB (2769386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea03e1302bd3e3a42c4d7c0fae2d0468e1d3bde81460b6512351ecd570eb6e81`  
		Last Modified: Sat, 10 Apr 2021 01:12:57 GMT  
		Size: 30.2 MB (30242655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699967ed2e86d295df07a366a0440e0c7d1531f8dfb88aa113227cddb5794b0a`  
		Last Modified: Sat, 10 Apr 2021 01:12:49 GMT  
		Size: 2.2 MB (2238967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
