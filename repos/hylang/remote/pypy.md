## `hylang:pypy`

```console
$ docker pull hylang@sha256:05ce986d4a8c9c4cc91baa80ad14521cb61cf1a9df887048cd038b92dcf9286d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.17763.2237; amd64

### `hylang:pypy` - linux; amd64

```console
$ docker pull hylang@sha256:08f1d441cf858b5be94ab0810bc6e5bcd12c2f324140cb044abc5f64606ccc57
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73622488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2fe3ffcee7245e264fd02dedb3b65533714780ffc7e322d887d106179f5e83f2`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 16:07:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 16:07:44 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 16:07:44 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Oct 2021 21:38:27 GMT
ENV PYPY_VERSION=7.3.6
# Mon, 18 Oct 2021 21:38:56 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux64.tar.bz2'; 			sha256='c41d07063b1d002a91ad2a0763b4baaca2b306ec635889c2e4826e706cc7f9ca'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-aarch64.tar.bz2'; 			sha256='d446b6987eeaa03d706603863e83d6b99df69232cf1e06d3ee5706add6a84cd6'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux32.tar.bz2'; 			sha256='459e77c845b31fa9367f7b1b1122155f0ba7888b1d4ce4455c35d2111eeeb275'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-s390x.tar.bz2'; 			sha256='3659bf96a177a53426ffc38d3619c6ee307e600c80e924edc9cee604680c141d'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 18 Oct 2021 21:38:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 18 Oct 2021 21:38:56 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 18 Oct 2021 21:39:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 18 Oct 2021 21:39:07 GMT
CMD ["pypy3"]
# Mon, 18 Oct 2021 22:06:19 GMT
ENV HY_VERSION=1.0a3
# Mon, 18 Oct 2021 22:06:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 18 Oct 2021 22:06:28 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed35c7420899dc2a554276761fec7776c759be3ab1dc2b373bed21cf08006be6`  
		Last Modified: Tue, 12 Oct 2021 16:16:25 GMT  
		Size: 1.1 MB (1065980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be42675c5beef59d476d85e2e1d63f867f9833a3409a70ba6d25c962293df5cb`  
		Last Modified: Mon, 18 Oct 2021 21:45:30 GMT  
		Size: 35.8 MB (35762424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c973f5f42999cfc5d3e59ec102a41ffb22cf22b659da9d4c2efee7e00238f7ba`  
		Last Modified: Mon, 18 Oct 2021 21:45:23 GMT  
		Size: 2.4 MB (2370099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7bdd90a3aed7ab9ae00e773bdb9ba6caf78ca55712ba637ed4f8cce79bf215`  
		Last Modified: Mon, 18 Oct 2021 22:08:24 GMT  
		Size: 3.1 MB (3066674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:291d1fc5a6b84cbf88f76c559ffde15ffb92aa6d95abf5cf251931467d9ccdbc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68773993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07c1cbd59873d1223d31768f3c460bce701c06afd28bc21ac33b427a16ba2aa8`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:18 GMT
ADD file:d84144ad575672cd6cc8a00c8e5a88ab0545348f040fc249ea5fcf8193b2bce6 in / 
# Tue, 12 Oct 2021 01:41:18 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 16:39:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 16:39:55 GMT
ENV LANG=C.UTF-8
# Wed, 13 Oct 2021 16:39:56 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Oct 2021 22:23:17 GMT
ENV PYPY_VERSION=7.3.6
# Mon, 18 Oct 2021 22:23:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux64.tar.bz2'; 			sha256='c41d07063b1d002a91ad2a0763b4baaca2b306ec635889c2e4826e706cc7f9ca'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-aarch64.tar.bz2'; 			sha256='d446b6987eeaa03d706603863e83d6b99df69232cf1e06d3ee5706add6a84cd6'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux32.tar.bz2'; 			sha256='459e77c845b31fa9367f7b1b1122155f0ba7888b1d4ce4455c35d2111eeeb275'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-s390x.tar.bz2'; 			sha256='3659bf96a177a53426ffc38d3619c6ee307e600c80e924edc9cee604680c141d'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 18 Oct 2021 22:23:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 18 Oct 2021 22:23:45 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 18 Oct 2021 22:23:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 18 Oct 2021 22:23:58 GMT
CMD ["pypy3"]
# Mon, 18 Oct 2021 23:24:26 GMT
ENV HY_VERSION=1.0a3
# Mon, 18 Oct 2021 23:24:36 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 18 Oct 2021 23:24:37 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:a9eb63951c1c2ee8efcc12b696928fee3741a2d4eae76f2da3e161a5d90548bf`  
		Last Modified: Tue, 12 Oct 2021 01:48:13 GMT  
		Size: 30.0 MB (30043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244bad71c45dd865aa32743cd1ff31b180595e799db39b4954c7a6928b9ba8ae`  
		Last Modified: Wed, 13 Oct 2021 16:48:39 GMT  
		Size: 1.1 MB (1053927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afad86007a56c979c72e02ef09583700b21ba366e2d762cff970521b0809889`  
		Last Modified: Mon, 18 Oct 2021 22:31:35 GMT  
		Size: 32.5 MB (32455123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4749e444f6a5e920e32999fb0972257982e96879f523a25d8e8142c5b7ac10f7`  
		Last Modified: Mon, 18 Oct 2021 22:31:29 GMT  
		Size: 2.2 MB (2154902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9eff55bf7e3e09e903f758e5fd79a30b45a735f6b7a820aed2f66e9690886e6`  
		Last Modified: Mon, 18 Oct 2021 23:28:04 GMT  
		Size: 3.1 MB (3066135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - linux; 386

```console
$ docker pull hylang@sha256:cf5039c832613efc0ce6ba398f60c4cd3330ce0716a0c9c841f9002718662fde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.8 MB (73823877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:005f5a0a92ce18771b35c9fd67a97e42448f21ac78b93166429ce45be700e012`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:47 GMT
ADD file:42196ffa4c70af8d9f1e7b74edb3bb92d47296acf989adf615e8208230f8bd0c in / 
# Tue, 12 Oct 2021 01:39:47 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:51:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:51:57 GMT
ENV LANG=C.UTF-8
# Tue, 12 Oct 2021 09:51:57 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Oct 2021 21:47:39 GMT
ENV PYPY_VERSION=7.3.6
# Mon, 18 Oct 2021 21:48:11 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux64.tar.bz2'; 			sha256='c41d07063b1d002a91ad2a0763b4baaca2b306ec635889c2e4826e706cc7f9ca'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-aarch64.tar.bz2'; 			sha256='d446b6987eeaa03d706603863e83d6b99df69232cf1e06d3ee5706add6a84cd6'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-linux32.tar.bz2'; 			sha256='459e77c845b31fa9367f7b1b1122155f0ba7888b1d4ce4455c35d2111eeeb275'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.7-v7.3.6-s390x.tar.bz2'; 			sha256='3659bf96a177a53426ffc38d3619c6ee307e600c80e924edc9cee604680c141d'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib-python -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib_pypy; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Mon, 18 Oct 2021 21:48:11 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 18 Oct 2021 21:48:11 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 18 Oct 2021 21:48:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Mon, 18 Oct 2021 21:48:23 GMT
CMD ["pypy3"]
# Mon, 18 Oct 2021 22:20:09 GMT
ENV HY_VERSION=1.0a3
# Mon, 18 Oct 2021 22:20:18 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION"
# Mon, 18 Oct 2021 22:20:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:87318d165b5c0fdf05c8ccf97d83084f56b4608075a3335b1a46c76295b82753`  
		Last Modified: Tue, 12 Oct 2021 01:47:39 GMT  
		Size: 32.4 MB (32370344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e56cd7d03192db8b2e7e5fc40267a5319da47f0a28fcfeb91b2309b27db20f`  
		Last Modified: Tue, 12 Oct 2021 10:02:16 GMT  
		Size: 1.1 MB (1078385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e39b32c71b4806ee961e6905413b9923baa1b96b9d6c0bdb930930d1afd317`  
		Last Modified: Mon, 18 Oct 2021 21:57:12 GMT  
		Size: 34.9 MB (34938689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f502ba525ad229ab09865e74ac300524dde57d1153b8dcdc2b5f6ca986fd37`  
		Last Modified: Mon, 18 Oct 2021 21:57:03 GMT  
		Size: 2.4 MB (2369808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2480d58857801eb7fdb34a2f9f9c401c76a4c0b77d4c785ec508c1c23224c4`  
		Last Modified: Mon, 18 Oct 2021 22:24:13 GMT  
		Size: 3.1 MB (3066651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy` - windows version 10.0.17763.2237; amd64

```console
$ docker pull hylang@sha256:33742746fb47d7f908d0a86639b53fe4a54c1c86c55d5242b94c16084ccf2e28
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2734321064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19788a51152234444b90691a3b217fdc5cde7b85146e7385d43bc11fbc5a1236`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Oct 2021 12:04:48 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 13 Oct 2021 12:06:13 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Mon, 18 Oct 2021 22:18:34 GMT
ENV PYPY_VERSION=7.3.6
# Mon, 18 Oct 2021 22:20:17 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.7-v7.3.6-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '341e69a369da5a1f4f69dbbd47e7dff5e745439b203e28c7afcf98308a24b003'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.7-v7.3.6-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy3 --version") ...'; 	pypy3 --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Mon, 18 Oct 2021 22:20:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Mon, 18 Oct 2021 22:20:19 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Mon, 18 Oct 2021 22:22:24 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Mon, 18 Oct 2021 22:22:25 GMT
CMD ["pypy3"]
# Mon, 18 Oct 2021 22:44:38 GMT
ENV HY_VERSION=1.0a3
# Mon, 18 Oct 2021 22:46:29 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Mon, 18 Oct 2021 22:46:30 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a3bdf70816ac16df25478dbbccc6214bf88a0b692485f62ab5c8786d6712f0`  
		Last Modified: Wed, 13 Oct 2021 12:18:06 GMT  
		Size: 346.8 KB (346768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41276917c6b2081d9aae93760066800018afb849c5db8de79720a2e590568b57`  
		Last Modified: Wed, 13 Oct 2021 12:18:10 GMT  
		Size: 15.5 MB (15492096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00932d7df2664db2fd45cff32a616ebccb0410c6cb80e53db1f45929371b057f`  
		Last Modified: Mon, 18 Oct 2021 22:27:13 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f622866d679ad7975e3439aa7eb1f7613bc9d62a89dcd3419446e8223ffd705a`  
		Last Modified: Mon, 18 Oct 2021 22:27:18 GMT  
		Size: 25.3 MB (25278970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4912f72b6a4671245a9b727d205da06b48470e0bff0f6c67b6c2ffad783fd239`  
		Last Modified: Mon, 18 Oct 2021 22:27:11 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a04dd942dd278f8c37ba8d934ffcb80027020ac4155b86a5a51fd0550de574f`  
		Last Modified: Mon, 18 Oct 2021 22:27:11 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e454d1db8361cf67588eaea8c87e94b67ef7643f2dd68c5bc750bab9d63232`  
		Last Modified: Mon, 18 Oct 2021 22:27:13 GMT  
		Size: 2.8 MB (2822712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf0bc68aec4d98ab33a1c2d5dea3f4e7ae01e7fd609a1ecd63c06402a4e3539`  
		Last Modified: Mon, 18 Oct 2021 22:27:11 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21201aecaa8ef83728f902f1054a3d6872be398da04eb2fd08b188d1e19a6451`  
		Last Modified: Mon, 18 Oct 2021 22:47:14 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b55f0a3707ef2e2de2b099244dc991f929adcfcb08af6321be03d55e5c3d79f`  
		Last Modified: Mon, 18 Oct 2021 22:47:15 GMT  
		Size: 4.1 MB (4051762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7233e83221d6e8a3088d6a20b376b3a9dc3a957bed38b2476f1b09d1f479267`  
		Last Modified: Mon, 18 Oct 2021 22:47:13 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
