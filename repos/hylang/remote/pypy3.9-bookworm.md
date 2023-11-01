## `hylang:pypy3.9-bookworm`

```console
$ docker pull hylang@sha256:3e5aeaaa1998a98d5d8e6ea14cb3e8d0a335213d9260b740886ce3cea4c49a58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:pypy3.9-bookworm` - linux; amd64

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

### `hylang:pypy3.9-bookworm` - linux; arm64 variant v8

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

### `hylang:pypy3.9-bookworm` - linux; 386

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
