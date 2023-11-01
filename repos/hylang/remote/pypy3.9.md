## `hylang:pypy3.9`

```console
$ docker pull hylang@sha256:55f4bf6beb6948f11a0a40843cd2207108dcb31fefcb72f08fadfc7409bdd7a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.2031; amd64
	-	windows version 10.0.17763.4974; amd64

### `hylang:pypy3.9` - linux; amd64

```console
$ docker pull hylang@sha256:90bab67fb591d3cfa9186b2a111d49f002d939df5a73137c2cf80f1d96149250
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.2 MB (76181093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c25952a6170dab3abfb8aca9ab0d510d7f9616a15f818a5a4ddca98fad99b3b3`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Nov 2023 00:20:49 GMT
ADD file:fbd8521c24ed758023728505c18d7a0d6d101bc77fd772a4af9b65049b943864 in / 
# Wed, 01 Nov 2023 00:20:49 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 02:57:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 02:57:32 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 02:57:32 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 02:57:32 GMT
ENV PYPY_VERSION=7.3.13
# Wed, 01 Nov 2023 03:00:59 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux64.tar.bz2'; 			sha256='323b05a9f607e932cda1995cbe77a96e4ea35994631aa6d734c8035e8479b74e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-aarch64.tar.bz2'; 			sha256='317d7876c5825a086f854253648b967a432b993ce87695d2895d3ad6ed0d2716'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux32.tar.bz2'; 			sha256='ac695238b4a3635ac6b482e74e04e2ea78b31acca0decd5de601dfd2f4ebf35a'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-s390x.tar.bz2'; 			sha256='213c88f652a99c4dc4e8e00b4b5b58f381c7f7e9ea1a9b65801fc0eb1e50df0a'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 01 Nov 2023 03:00:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 01 Nov 2023 03:00:59 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 01 Nov 2023 03:01:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Nov 2023 03:01:11 GMT
CMD ["pypy3"]
# Wed, 01 Nov 2023 18:25:01 GMT
ENV HY_VERSION=0.27.0
# Wed, 01 Nov 2023 18:25:01 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 01 Nov 2023 18:25:29 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 01 Nov 2023 18:25:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:578acb154839e9d0034432e8f53756d6f53ba62cf8c7ea5218a2476bf5b58fc9`  
		Last Modified: Wed, 01 Nov 2023 00:25:30 GMT  
		Size: 29.1 MB (29149836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09fcacf068736f37733c985132796568df05b156b069b086ab1327cf627dcbd4`  
		Last Modified: Wed, 01 Nov 2023 03:05:52 GMT  
		Size: 3.5 MB (3494652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9114a6bead4c6b388bbf4429caf57d22b66d3161356d3883cb7f9bd9ec69dbc`  
		Last Modified: Wed, 01 Nov 2023 03:07:58 GMT  
		Size: 36.5 MB (36492042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26705f2ca0b470f267b95789d7d9be533e3477e08d3a2bceb21295e34f59284a`  
		Last Modified: Wed, 01 Nov 2023 03:07:53 GMT  
		Size: 3.1 MB (3126164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afda16f93aaa97f2a53576dc224e23e44dbf240108ac60af91a57280ff5b09bb`  
		Last Modified: Wed, 01 Nov 2023 18:31:51 GMT  
		Size: 3.9 MB (3918399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:6a66b7d06c648cdf55c84417040c088640c52eb72964544b9be7f45e05920c05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.4 MB (73364522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bbc3069789e2a78bb6e2ee5528f8cb679eb10e8fc5837d323536fbe09b90262`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Nov 2023 00:39:41 GMT
ADD file:c58f86cd28b3a97f884e2a46f8fe60a2c5c1f443e198bd10e3277b4f3653736a in / 
# Wed, 01 Nov 2023 00:39:41 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 11:31:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 11:31:40 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 11:31:40 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 11:31:40 GMT
ENV PYPY_VERSION=7.3.13
# Wed, 01 Nov 2023 11:34:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux64.tar.bz2'; 			sha256='323b05a9f607e932cda1995cbe77a96e4ea35994631aa6d734c8035e8479b74e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-aarch64.tar.bz2'; 			sha256='317d7876c5825a086f854253648b967a432b993ce87695d2895d3ad6ed0d2716'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux32.tar.bz2'; 			sha256='ac695238b4a3635ac6b482e74e04e2ea78b31acca0decd5de601dfd2f4ebf35a'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-s390x.tar.bz2'; 			sha256='213c88f652a99c4dc4e8e00b4b5b58f381c7f7e9ea1a9b65801fc0eb1e50df0a'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 01 Nov 2023 11:34:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 01 Nov 2023 11:34:40 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 01 Nov 2023 11:34:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Nov 2023 11:34:51 GMT
CMD ["pypy3"]
# Wed, 01 Nov 2023 16:35:42 GMT
ENV HY_VERSION=0.27.0
# Wed, 01 Nov 2023 16:35:42 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 01 Nov 2023 16:36:12 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 01 Nov 2023 16:36:13 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:31ce7ceb6d443e2ab4ae91695fea10e1443417fd94c40a46994d5a96940ea1ca`  
		Last Modified: Wed, 01 Nov 2023 00:43:07 GMT  
		Size: 29.2 MB (29179119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e6a34785e9172f6512acad3a0f8ae05db467e5b7efd00e3f81c7b68fd1f62c`  
		Last Modified: Wed, 01 Nov 2023 11:38:59 GMT  
		Size: 3.3 MB (3317182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fbe43c1498aa684214c8cb636fca02d41566a13dad45cfcfb845a02db3b004`  
		Last Modified: Wed, 01 Nov 2023 11:41:05 GMT  
		Size: 33.8 MB (33823889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779d3c5e7f786aad8e98cf5d84bd5d742d3a51f4d88e5bbaac993c992a9a8a8e`  
		Last Modified: Wed, 01 Nov 2023 11:41:00 GMT  
		Size: 3.1 MB (3126115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383438bfcf2882a57e5642c4cb2b2c22230dff22ec525fe3c9646618bdde007c`  
		Last Modified: Wed, 01 Nov 2023 16:42:20 GMT  
		Size: 3.9 MB (3918217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - linux; 386

```console
$ docker pull hylang@sha256:c617256a68767e225d6d0c8d57dae307d48202609842c512ee0fb861e77f9af9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73213845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:116a281ce22c7b8f5c857205a50e25a0ee4b79532c87996f86d02bcac88a99e8`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Nov 2023 00:38:56 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Wed, 01 Nov 2023 00:38:56 GMT
CMD ["bash"]
# Wed, 01 Nov 2023 13:33:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Nov 2023 13:33:27 GMT
ENV LANG=C.UTF-8
# Wed, 01 Nov 2023 13:33:27 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Nov 2023 13:33:27 GMT
ENV PYPY_VERSION=7.3.13
# Wed, 01 Nov 2023 13:36:23 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux64.tar.bz2'; 			sha256='323b05a9f607e932cda1995cbe77a96e4ea35994631aa6d734c8035e8479b74e'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-aarch64.tar.bz2'; 			sha256='317d7876c5825a086f854253648b967a432b993ce87695d2895d3ad6ed0d2716'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-linux32.tar.bz2'; 			sha256='ac695238b4a3635ac6b482e74e04e2ea78b31acca0decd5de601dfd2f4ebf35a'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.13-s390x.tar.bz2'; 			sha256='213c88f652a99c4dc4e8e00b4b5b58f381c7f7e9ea1a9b65801fc0eb1e50df0a'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 01 Nov 2023 13:36:23 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 01 Nov 2023 13:36:23 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 01 Nov 2023 13:36:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Nov 2023 13:36:37 GMT
CMD ["pypy3"]
# Wed, 01 Nov 2023 17:46:58 GMT
ENV HY_VERSION=0.27.0
# Wed, 01 Nov 2023 17:46:58 GMT
ENV HYRULE_VERSION=0.4.0
# Wed, 01 Nov 2023 17:47:39 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 01 Nov 2023 17:47:39 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b9088195bd5a4382ad9b94ed109d5f0329b0d47a0e12b4e000da68c1f55249`  
		Last Modified: Wed, 01 Nov 2023 13:39:55 GMT  
		Size: 3.5 MB (3499403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8673325669708228359241aaaea8d7cac72ba8769184386274f52b05d359490b`  
		Last Modified: Wed, 01 Nov 2023 13:41:33 GMT  
		Size: 32.5 MB (32506359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34db84f0fb779564449acbde73ad1f6beeb4ddcf0aac2e1d69eca4a7cd2ab372`  
		Last Modified: Wed, 01 Nov 2023 13:41:26 GMT  
		Size: 3.1 MB (3125811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f13afab4cbb3c50bc26f39a616a40a43e3d30818bf67e8a4a13f843729ab52`  
		Last Modified: Wed, 01 Nov 2023 17:54:26 GMT  
		Size: 3.9 MB (3918230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - windows version 10.0.20348.2031; amd64

```console
$ docker pull hylang@sha256:ddba1e19e12c945e4f6eb8a0688641a50343268c94bdb631fd94dcc40d937ecf
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1910286389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b11a8cc68a3a66d49c69388dd71a92d7658119d0d76965f4db9d8b40aa7025c9`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Fri, 06 Oct 2023 21:59:31 GMT
RUN Install update 10.0.20348.2031
# Wed, 11 Oct 2023 01:35:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 06:14:40 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 11 Oct 2023 06:15:05 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:15:09 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 26 Oct 2023 01:21:59 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.13-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '85745a2055c4a8cefac9b6d3f7f305b1edaaf62468c8f640b4511d9dd21d091c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.13-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:22:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 26 Oct 2023 01:22:01 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 26 Oct 2023 01:23:06 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:23:07 GMT
CMD ["pypy"]
# Thu, 26 Oct 2023 01:46:38 GMT
ENV HY_VERSION=0.27.0
# Thu, 26 Oct 2023 01:46:39 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 26 Oct 2023 01:48:59 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 26 Oct 2023 01:49:00 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d2471a50c8ec3ea61c16dd871f7b9167bf779faad2b6e5a6f72a18b88b846b`  
		Last Modified: Tue, 10 Oct 2023 17:55:23 GMT  
		Size: 471.2 MB (471244358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73b90f34f44bbbb354af4f3d4cc6cde597d2f5183641e139f7ca8b76ec3bb9`  
		Last Modified: Wed, 11 Oct 2023 02:45:06 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd18844d7cd91075829793024df5a5d9d615bf17e860c71d9d1ef6b7cbd0dd0`  
		Last Modified: Wed, 11 Oct 2023 06:37:18 GMT  
		Size: 445.5 KB (445470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4050e10e1bb82c108d6c64fa6275e021c24161296f4976b50cc7ddd01032a`  
		Last Modified: Wed, 11 Oct 2023 06:37:20 GMT  
		Size: 15.5 MB (15451502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee80caefaddaede3888ab0418aff530483fdd9fd46c5cac248d9b0f6bdc6318`  
		Last Modified: Thu, 26 Oct 2023 01:28:35 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cbf5ee06e66af0f93b0cc76f62a8882f603bb3f2e22f60fd9067236db43e188`  
		Last Modified: Thu, 26 Oct 2023 01:29:50 GMT  
		Size: 26.5 MB (26524655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2c07a76cdc1112e2988568de337169bed9c9a139c39e006e19564bcbc09789`  
		Last Modified: Thu, 26 Oct 2023 01:29:43 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bbec89da37d2fe4d5d0f70d30849f5663e99fc373e65bc2508ce5f01499045`  
		Last Modified: Thu, 26 Oct 2023 01:29:43 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be717c4074c88027705426f0334a516ab6c0e20da9adeb0efcb03df2845a244`  
		Last Modified: Thu, 26 Oct 2023 01:29:45 GMT  
		Size: 3.5 MB (3451900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad2d9351e7e4f2f9fb0f970b9967194d28958292f49ab82ade472773f37e582`  
		Last Modified: Thu, 26 Oct 2023 01:29:43 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f3b1dfe4ee2af7d85678525fd076b0c39d0fcb0d78d4c0c76f7a7160808ed8`  
		Last Modified: Thu, 26 Oct 2023 01:52:35 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27a1da08ef3ef1444132d5298dc3d1c1dfeddae89e100acdd8c95dcaf5b47a1d`  
		Last Modified: Thu, 26 Oct 2023 01:52:35 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e45bae1e80381153942f9287f2f6c4fa4ead308916363da25ee5504cd69b959`  
		Last Modified: Thu, 26 Oct 2023 01:52:36 GMT  
		Size: 4.6 MB (4558902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6755ff4ff74ef83b04664b43c75faa69114e9ada89c51593d7597eb21110b9`  
		Last Modified: Thu, 26 Oct 2023 01:52:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9` - windows version 10.0.17763.4974; amd64

```console
$ docker pull hylang@sha256:7b52ecbec2059d3abdd852517692a31cc73a8d371a58c95ca69010d267a2fdb4
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2081993142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e38bd7f4adde5b4e6223c203bebd8db526c4d82e604925c0bb03f00600fe201a`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 01:36:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Oct 2023 06:18:14 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 11 Oct 2023 06:19:20 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:17:22 GMT
ENV PYPY_VERSION=7.3.13
# Thu, 26 Oct 2023 01:24:58 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.13-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '85745a2055c4a8cefac9b6d3f7f305b1edaaf62468c8f640b4511d9dd21d091c'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.13-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:24:59 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 26 Oct 2023 01:25:00 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 26 Oct 2023 01:26:59 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 26 Oct 2023 01:27:00 GMT
CMD ["pypy"]
# Thu, 26 Oct 2023 01:49:06 GMT
ENV HY_VERSION=0.27.0
# Thu, 26 Oct 2023 01:49:07 GMT
ENV HYRULE_VERSION=0.4.0
# Thu, 26 Oct 2023 01:52:05 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 26 Oct 2023 01:52:06 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0814e4a0bb8c615854a85a2b60cd043cfd20ad5a5d755acab1b30b18e4bfad3c`  
		Last Modified: Wed, 11 Oct 2023 02:46:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a5a98b72477000ef06eb79bfb3b25493744b54910aa53f67172f4a0409d54f`  
		Last Modified: Wed, 11 Oct 2023 06:37:50 GMT  
		Size: 446.1 KB (446147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bda9c0579f6d9423b6583385b098fe26e0ac02365bfa64fc2e30a1252fc329`  
		Last Modified: Wed, 11 Oct 2023 06:37:51 GMT  
		Size: 15.4 MB (15444426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f36f7ce6b22f93d0e7bcc3eeb5794856d2e0ad9e7728cadf77375c51df74fc5a`  
		Last Modified: Thu, 26 Oct 2023 01:29:11 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e776e4053e2dec485651cc2659b541647616afb2c250eb99f5e96100e506a7`  
		Last Modified: Thu, 26 Oct 2023 01:30:13 GMT  
		Size: 26.5 MB (26515636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890bbdf4f37c14d23ab4ff33644f24ef9c38620c2e71c24683ef3118566db279`  
		Last Modified: Thu, 26 Oct 2023 01:30:07 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa225c50c32cf081feedfdd417191a4454b14a3ebdee3e49875655b2ca0bef1`  
		Last Modified: Thu, 26 Oct 2023 01:30:07 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7ad6033470f19ced27e88c5405ceb5b84080c2b720c29a37973466609922f`  
		Last Modified: Thu, 26 Oct 2023 01:30:08 GMT  
		Size: 3.4 MB (3437543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a79c62fc36a94040fcf7b802569e346297696ed7d033c7b85a1dbd26a9acded3`  
		Last Modified: Thu, 26 Oct 2023 01:30:07 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4db9b44a23a369281121f7c2c170fa8ca08dd2956ec1cf3bb9eec033bac74dc`  
		Last Modified: Thu, 26 Oct 2023 01:52:52 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453f1c7f5673e7c58fc245c235e413271c0a56074c4548c4fd622e966351bad3`  
		Last Modified: Thu, 26 Oct 2023 01:52:52 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9195be8e5b56c73d7a7105a0de3a6739d85593a80a526515bc80d2bfe6578b1`  
		Last Modified: Thu, 26 Oct 2023 01:52:53 GMT  
		Size: 4.5 MB (4547747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce56f5b0683d8a3341b760e63dd15680d7ccb1173955ddd357260649f7e4be6d`  
		Last Modified: Thu, 26 Oct 2023 01:52:52 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
