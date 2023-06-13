## `hylang:0-pypy-buster`

```console
$ docker pull hylang@sha256:a446d52910e84df449e56abdbac16e4d1fee60794d304a4b82782ab464b71adb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-pypy-buster` - linux; amd64

```console
$ docker pull hylang@sha256:18e67e73b3155a1b17bc191bf398150bc58d9d9531e5bcd1cb7ce38ec0cec6e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.4 MB (74431651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4387fdeba34eb136dfd8ab12af933222b87d7d05d0a4a8fcab6cf8a7c6cfe8bc`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 12 Jun 2023 23:21:32 GMT
ADD file:2818e508d01da2188fb234b38fb19aa1ea9eeeae92d361ecdf49318d949f51a9 in / 
# Mon, 12 Jun 2023 23:21:32 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 13:00:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 13:00:19 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 13:00:20 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 13:00:20 GMT
ENV PYPY_VERSION=7.3.11
# Tue, 13 Jun 2023 13:00:52 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 13 Jun 2023 13:00:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 13 Jun 2023 13:00:53 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 13 Jun 2023 13:01:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 13 Jun 2023 13:01:05 GMT
CMD ["pypy3"]
# Tue, 13 Jun 2023 23:08:16 GMT
ENV HY_VERSION=0.26.0
# Tue, 13 Jun 2023 23:08:16 GMT
ENV HYRULE_VERSION=0.3.0
# Tue, 13 Jun 2023 23:08:46 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 13 Jun 2023 23:08:46 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8b91b88d557765cd8c6802668755a3f6dc4337b6ce15a17e4857139e5fc964f3`  
		Last Modified: Mon, 12 Jun 2023 23:27:09 GMT  
		Size: 27.1 MB (27138450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1357c5038e4f3e7f48bb0a1eeb487071b7cd2626433d2dce63c5a33c4a762771`  
		Last Modified: Tue, 13 Jun 2023 13:07:44 GMT  
		Size: 2.8 MB (2768417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:549b4375179c52117781d774e045edcde58ee56022f629c7928a234c0b38c1b6`  
		Last Modified: Tue, 13 Jun 2023 13:07:50 GMT  
		Size: 37.3 MB (37271659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ea0d479bd2a47db827a8cc3e7cfff68f57649526b073272fcd66f4ef558618d`  
		Last Modified: Tue, 13 Jun 2023 13:07:45 GMT  
		Size: 3.2 MB (3192295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa5b2b06ad7969ffe4a1e9e9bbaf01dddea801dfaae99f2c99f31cf14761610`  
		Last Modified: Tue, 13 Jun 2023 23:15:13 GMT  
		Size: 4.1 MB (4060830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-buster` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:38a603c62c47467d82bb3f8d052a9725354a2b386e154610420c073defe659db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70186009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1aeb0e83d982ef5291facc7bec07a711bacebd33067eff801886c771d58ed73`
-	Default Command: `["hy"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:52 GMT
ADD file:d4a87f28032264e15d38bdd7efb6ffca8deadeb5388758f243e4866b360324c2 in / 
# Mon, 12 Jun 2023 23:40:52 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 10:19:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 10:19:24 GMT
ENV LANG=C.UTF-8
# Tue, 13 Jun 2023 10:19:24 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Jun 2023 10:19:24 GMT
ENV PYPY_VERSION=7.3.11
# Tue, 13 Jun 2023 10:19:53 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 13 Jun 2023 10:19:53 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 13 Jun 2023 10:19:53 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 13 Jun 2023 10:20:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 13 Jun 2023 10:20:05 GMT
CMD ["pypy3"]
# Tue, 13 Jun 2023 21:32:12 GMT
ENV HY_VERSION=0.26.0
# Tue, 13 Jun 2023 21:32:12 GMT
ENV HYRULE_VERSION=0.3.0
# Tue, 13 Jun 2023 21:32:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 13 Jun 2023 21:32:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:d191be7a3c9fa95847a482db8211b6f85b45096c7817fdad4d7661ee7ff1a421`  
		Last Modified: Mon, 12 Jun 2023 23:45:21 GMT  
		Size: 25.9 MB (25921353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37410a8b9170252b5374a141ca139ced2b33dd752151ddc71d07d66e9fdc7bc0`  
		Last Modified: Tue, 13 Jun 2023 10:26:17 GMT  
		Size: 2.6 MB (2636876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c6ea886328152257f505d036d00fafa8021629d28ed5d9b4af3c83abf2cf94`  
		Last Modified: Tue, 13 Jun 2023 10:26:21 GMT  
		Size: 34.4 MB (34375105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2653527995ff244d10ae0e49a7e5fc8fd0b826b2b8f824dbf24431e6706d7ffb`  
		Last Modified: Tue, 13 Jun 2023 10:26:17 GMT  
		Size: 3.2 MB (3191824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e19942ca3dd219ccb85f1d0387565bf616a1a0e85402d44490870f76afe765e`  
		Last Modified: Tue, 13 Jun 2023 21:38:29 GMT  
		Size: 4.1 MB (4060851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-buster` - linux; 386

```console
$ docker pull hylang@sha256:0ff086273d7800f186f941ed3938ce6d20ffcc2043cb12856a1cad4f449b5d52
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.1 MB (76060183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2a947342d76fc517ac5f81c8fd8e7910cb53652b0da94a2283e6265975b34fc`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 23 May 2023 00:40:01 GMT
ADD file:96715cff0e3569a2a1d7e203f0797ed4880da7714d455e25f032c67bff27221f in / 
# Tue, 23 May 2023 00:40:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 14:58:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 14:58:09 GMT
ENV LANG=C.UTF-8
# Tue, 23 May 2023 14:58:10 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 May 2023 14:58:10 GMT
ENV PYPY_VERSION=7.3.11
# Tue, 23 May 2023 14:58:48 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 23 May 2023 14:58:49 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 23 May 2023 14:58:49 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 23 May 2023 14:59:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 23 May 2023 14:59:03 GMT
CMD ["pypy3"]
# Wed, 24 May 2023 00:06:12 GMT
ENV HY_VERSION=0.26.0
# Wed, 24 May 2023 00:06:12 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 24 May 2023 00:06:50 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 24 May 2023 00:06:50 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3c2058520f8e2dee0c8d97a0e68335849888066e5d0d1b82b6ef302541b5c874`  
		Last Modified: Tue, 23 May 2023 00:45:13 GMT  
		Size: 27.8 MB (27797210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d31224a82e23a5a6c5836599281605ed15e4ac3f8eac4ed104f34f9566bd821`  
		Last Modified: Tue, 23 May 2023 15:07:06 GMT  
		Size: 2.8 MB (2783852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da00703a056bbc805b7c74ff2f817be8026d3517101c8c69a8025d67f983ad0a`  
		Last Modified: Tue, 23 May 2023 15:07:14 GMT  
		Size: 38.2 MB (38226161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1aefbd3b2f6eeded363cb7b461de04d1e76c5b880ee8551c6aeee8bfeba78b0`  
		Last Modified: Tue, 23 May 2023 15:07:06 GMT  
		Size: 3.2 MB (3191925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79e3f3d8ab66b56193d268884a34bbf4f567d7fb4710466a233389c79cba9de`  
		Last Modified: Wed, 24 May 2023 00:13:10 GMT  
		Size: 4.1 MB (4061035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
