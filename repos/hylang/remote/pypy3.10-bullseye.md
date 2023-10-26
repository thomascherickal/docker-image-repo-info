## `hylang:pypy3.10-bullseye`

```console
$ docker pull hylang@sha256:e5ef037fe91aec1302888afcae8eb1bd08c9931e485d4e4d666006229601ab7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.10-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:8611f7718b0197458969fcb0164bfc5d3d75aa68db7028da79e47191a4df4271
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.9 MB (77906788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8973942027f775d0cec9422ac2a586cdeb62417608cd01cb0bcf0a658d9daad`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 Oct 2023 18:35:13 GMT
ADD file:cb13581b8e7a9de4396639e5ca2f3817763435c0563232f85e3d899f6388a1b3 in / 
# Wed, 11 Oct 2023 18:35:13 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 02:53:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 02:53:57 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 02:53:57 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 02:57:07 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 26 Oct 2023 01:29:24 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux64.tar.bz2'; 			sha256='54936eeafd9350a5ea0375b036272a260871b9bca82e1b0bb3201deea9f5a442'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-aarch64.tar.bz2'; 			sha256='ac476f01c9653358404f2e4b52f62307b2f64ccdb8c96dadcbfe355824d81a63'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux32.tar.bz2'; 			sha256='bfba57eb1f859dd0ad0d6fe841bb12e1256f1f023c7fbca083b536cccbc1233b'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-s390x.tar.bz2'; 			sha256='3c813c7efa6a026b281313b299c186c585155fc164c7538e65d41efdabff87c9'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 26 Oct 2023 01:29:25 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 26 Oct 2023 01:29:25 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 26 Oct 2023 01:29:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 26 Oct 2023 01:29:37 GMT
CMD ["pypy3"]
# Thu, 26 Oct 2023 01:54:29 GMT
ENV HY_VERSION=0.27.0
# Thu, 26 Oct 2023 01:54:29 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 26 Oct 2023 01:54:59 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 26 Oct 2023 01:54:59 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:e67fdae3559346105027c63e7fb032bba57e62b1fe9f2da23e6fdfb56384e00b`  
		Last Modified: Wed, 11 Oct 2023 18:40:17 GMT  
		Size: 31.4 MB (31417862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb2029872e7d96806f6e6a1654ba712b38f740f0f9f61f0d4c0e530ac465e03`  
		Last Modified: Thu, 12 Oct 2023 02:59:06 GMT  
		Size: 1.1 MB (1068490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637c5c7fbb3edc21eb1577cb05f70f8bdc13fab8be60412a63bf1545d542ebf8`  
		Last Modified: Thu, 26 Oct 2023 01:35:07 GMT  
		Size: 35.6 MB (35588214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847eba2735dc73ce18552f2a6b99cf86a3184b7377cc70cf7d37fb2ac83eeee3`  
		Last Modified: Thu, 26 Oct 2023 01:35:02 GMT  
		Size: 3.5 MB (3518630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d155159fa391ca2b49472db3fda7821453e2de7a7c0c4a08e1a47853d43c1695`  
		Last Modified: Thu, 26 Oct 2023 01:58:39 GMT  
		Size: 6.3 MB (6313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.10-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:5aea0729a8099a0f076af8a66e4e582fcec4e27abb14e16cd2dc6990ef23dc17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.2 MB (74159442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335ff410085b30e17082692a32c51cc2b577857c041ec63b5d976d245733e463`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 Oct 2023 18:25:06 GMT
ADD file:2c3e5451390c62f0b85f20139d2c88011cc54d649cdda5567084c050ad373372 in / 
# Wed, 11 Oct 2023 18:25:06 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 03:41:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 03:41:21 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 03:41:21 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 03:51:05 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 26 Oct 2023 01:09:40 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux64.tar.bz2'; 			sha256='54936eeafd9350a5ea0375b036272a260871b9bca82e1b0bb3201deea9f5a442'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-aarch64.tar.bz2'; 			sha256='ac476f01c9653358404f2e4b52f62307b2f64ccdb8c96dadcbfe355824d81a63'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux32.tar.bz2'; 			sha256='bfba57eb1f859dd0ad0d6fe841bb12e1256f1f023c7fbca083b536cccbc1233b'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-s390x.tar.bz2'; 			sha256='3c813c7efa6a026b281313b299c186c585155fc164c7538e65d41efdabff87c9'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 26 Oct 2023 01:09:41 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 26 Oct 2023 01:09:41 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 26 Oct 2023 01:09:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 26 Oct 2023 01:09:53 GMT
CMD ["pypy3"]
# Thu, 26 Oct 2023 01:34:01 GMT
ENV HY_VERSION=0.27.0
# Thu, 26 Oct 2023 01:34:01 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 26 Oct 2023 01:34:32 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 26 Oct 2023 01:34:32 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:85e50d2242ceaba78c3726e059dbd2fa06f5c18e265554bd43a482d19b256d20`  
		Last Modified: Wed, 11 Oct 2023 18:29:07 GMT  
		Size: 30.1 MB (30064086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57dc7cfd0da8b117b3b58b70d8224fd60be57225a72b008ecafe35bc71feaff8`  
		Last Modified: Thu, 12 Oct 2023 03:53:45 GMT  
		Size: 1.1 MB (1055757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2ef5fb9c2bbe7a2b417bf21fb45379a5ab5c2d407377ec60a300fd53c19481`  
		Last Modified: Thu, 26 Oct 2023 01:15:05 GMT  
		Size: 33.2 MB (33207617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbe1067abf3cf54e701dda546e00fe5b8a091de8b32faa3e2f5d5769b18ff7e`  
		Last Modified: Thu, 26 Oct 2023 01:15:01 GMT  
		Size: 3.5 MB (3518384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c964077ff7cbe27ee9a4fad13e36868a131ba3cd39381d8a699abe5b9699b1c`  
		Last Modified: Thu, 26 Oct 2023 01:37:51 GMT  
		Size: 6.3 MB (6313598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.10-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:394af60d68ab0917b4f2e02e7ee523d679fb61dc3a182a3ccd72dede41d2f48a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.3 MB (77271952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82084670b6e4c73721643c920fffa2ad5c2674730977163217891ae5c6a05730`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 Oct 2023 17:41:03 GMT
ADD file:ec6d51df021532be6c52d882f60a33d5cce8c3bff039efe8b98e923f2658ba45 in / 
# Wed, 11 Oct 2023 17:41:03 GMT
CMD ["bash"]
# Thu, 12 Oct 2023 13:16:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Oct 2023 13:16:04 GMT
ENV LANG=C.UTF-8
# Thu, 12 Oct 2023 13:16:04 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 Oct 2023 13:22:29 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 26 Oct 2023 00:44:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux64.tar.bz2'; 			sha256='54936eeafd9350a5ea0375b036272a260871b9bca82e1b0bb3201deea9f5a442'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-aarch64.tar.bz2'; 			sha256='ac476f01c9653358404f2e4b52f62307b2f64ccdb8c96dadcbfe355824d81a63'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-linux32.tar.bz2'; 			sha256='bfba57eb1f859dd0ad0d6fe841bb12e1256f1f023c7fbca083b536cccbc1233b'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.10-v7.3.13-s390x.tar.bz2'; 			sha256='3c813c7efa6a026b281313b299c186c585155fc164c7538e65d41efdabff87c9'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.10; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 26 Oct 2023 00:44:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 26 Oct 2023 00:44:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 26 Oct 2023 00:44:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 26 Oct 2023 00:44:26 GMT
CMD ["pypy3"]
# Thu, 26 Oct 2023 01:10:02 GMT
ENV HY_VERSION=0.27.0
# Thu, 26 Oct 2023 01:10:02 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 26 Oct 2023 01:10:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 26 Oct 2023 01:10:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f088164df28359c53d5766709e069e084073984ecf4688687b4c7c529a8926a5`  
		Last Modified: Wed, 11 Oct 2023 17:46:21 GMT  
		Size: 32.4 MB (32402649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28ef4a1ac786e9aeec3953a14ef0eadce3fe4e1fb2b0f4e02d5ed24bdc2b0ce`  
		Last Modified: Thu, 12 Oct 2023 13:25:55 GMT  
		Size: 1.1 MB (1080455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d543a2f169228b6e5b8f8ec88f7742435444ca4824b8f60fc040c9b4346322`  
		Last Modified: Thu, 26 Oct 2023 00:50:47 GMT  
		Size: 34.0 MB (33956841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900b48208f3d8fd1c5b471e12ea7a94a0ac40fa52ffdea12bccc817cb7af3c9b`  
		Last Modified: Thu, 26 Oct 2023 00:50:40 GMT  
		Size: 3.5 MB (3518290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a6fffee2a5840ddeecfbe5179d6a80804ae9ea35e7d04a6b94264110235e23`  
		Last Modified: Thu, 26 Oct 2023 01:15:05 GMT  
		Size: 6.3 MB (6313717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
