## `hylang:0-pypy3.9`

```console
$ docker pull hylang@sha256:db8674073aacd50277692c0d749b64e248be35220b18f6870e3596a28dfbca98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `hylang:0-pypy3.9` - linux; amd64

```console
$ docker pull hylang@sha256:83d917dfd2f16f722b4a966c2cfc1aaff226ed429aac9a221f7afc69a340de97
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75869216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e6263824dd3e0512e0ae3e1ed518160d3562709939c1c48674c5ca363a40228`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 13:38:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 13:38:03 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 13:38:03 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 13:38:03 GMT
ENV PYPY_VERSION=7.3.11
# Wed, 01 Mar 2023 13:38:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 01 Mar 2023 13:38:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 01 Mar 2023 13:38:35 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 01 Mar 2023 13:38:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Mar 2023 13:38:47 GMT
CMD ["pypy3"]
# Thu, 02 Mar 2023 02:03:44 GMT
ENV HY_VERSION=0.26.0
# Thu, 02 Mar 2023 02:03:44 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 02 Mar 2023 02:04:17 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 02 Mar 2023 02:04:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c6d95e843f13867bc54ffb2aa2b46a4ee400099603b7d5c09ec77f6739a369`  
		Last Modified: Wed, 01 Mar 2023 13:47:09 GMT  
		Size: 1.1 MB (1066527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e019a4c855d394b707f64196d37d22d9b62d84e25da0cbcea7f6f23618d580d`  
		Last Modified: Wed, 01 Mar 2023 13:47:15 GMT  
		Size: 36.2 MB (36188076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f028622ddd4509797edb11c1c4b84cdaa34f340ad12123d6612ba477dbb2e6ac`  
		Last Modified: Wed, 01 Mar 2023 13:47:10 GMT  
		Size: 3.2 MB (3170665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3e5b8c5672672fca5b66a955e0783c3de0adccf6a80dedaae68cb97405ccc1`  
		Last Modified: Thu, 02 Mar 2023 02:11:50 GMT  
		Size: 4.0 MB (4032545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.9` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:495eb766f330fef8f4a941fb37c2ad599965d20962c45b974bfcfc84dcf6213a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (72012885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0f8ccfa3d2a6c42578839c525dea16b12f5eea3adeaffb28d3911595180ec42`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:39 GMT
ADD file:9dc5c6fb6431df80107eddb76fb18256d6f4a06b4b22f9a7c4bcd58476068186 in / 
# Wed, 01 Mar 2023 02:20:39 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 09:37:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 09:37:28 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 09:37:28 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 09:37:29 GMT
ENV PYPY_VERSION=7.3.11
# Wed, 01 Mar 2023 09:37:55 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 01 Mar 2023 09:37:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 01 Mar 2023 09:37:55 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 01 Mar 2023 09:38:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 01 Mar 2023 09:38:07 GMT
CMD ["pypy3"]
# Wed, 01 Mar 2023 20:28:37 GMT
ENV HY_VERSION=0.26.0
# Wed, 01 Mar 2023 20:28:37 GMT
ENV HYRULE_VERSION=0.3.0
# Wed, 01 Mar 2023 20:29:07 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 01 Mar 2023 20:29:07 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:66dbba0fb1b568cc3ffd53409ba2f9f82995ab7f80e379338f3f36e4dcd223be`  
		Last Modified: Wed, 01 Mar 2023 02:24:17 GMT  
		Size: 30.1 MB (30062814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3518646ce4a40714303b2693f143fbc507b90732e3f4e9941db488366fc24f`  
		Last Modified: Wed, 01 Mar 2023 09:46:04 GMT  
		Size: 1.1 MB (1054047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a968c901b6f45af3752b35f5dc5aa3fef536aaaf8f311315f98d64be6289437b`  
		Last Modified: Wed, 01 Mar 2023 09:46:08 GMT  
		Size: 33.7 MB (33692940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0549e87b0d8fbe01d6c4cc0f85485f327ba95b3c7763419f47c9fd8f609cac`  
		Last Modified: Wed, 01 Mar 2023 09:46:04 GMT  
		Size: 3.2 MB (3170487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4442796d2b61b9efe4feda42e4c63604bc2c172986f8e68e5478b32f90b835`  
		Last Modified: Wed, 01 Mar 2023 20:36:56 GMT  
		Size: 4.0 MB (4032597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.9` - linux; 386

```console
$ docker pull hylang@sha256:e10ba8ec8f59c363b7b0295d5875bddb6ef128d0a4bc108065ba900ef7506439
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75116705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7ac2ceb6febb8bf0b31f22ef72640b9cfe878d82145db85cfc8090841f68cb`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 01 Mar 2023 01:39:14 GMT
ADD file:7ff48f7b36d13400120a726cd394769a4c39e8424877f5b080aeb9da07eacebe in / 
# Wed, 01 Mar 2023 01:39:15 GMT
CMD ["bash"]
# Thu, 02 Mar 2023 04:12:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 04:12:05 GMT
ENV LANG=C.UTF-8
# Thu, 02 Mar 2023 04:12:06 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 02 Mar 2023 04:12:06 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 02 Mar 2023 04:12:39 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 02 Mar 2023 04:12:39 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 02 Mar 2023 04:12:39 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 02 Mar 2023 04:12:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 02 Mar 2023 04:12:52 GMT
CMD ["pypy3"]
# Thu, 02 Mar 2023 05:09:48 GMT
ENV HY_VERSION=0.26.0
# Thu, 02 Mar 2023 05:09:48 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 02 Mar 2023 05:10:24 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 02 Mar 2023 05:10:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:2b884ef8a2d2b7c2016a8d2926b5b284f2130128ee049cae31a2da609cda7257`  
		Last Modified: Wed, 01 Mar 2023 01:44:44 GMT  
		Size: 32.4 MB (32396138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c289128b6833e31e95e22ad48341fe66d7dce2ce9ba94a5befd98b42ac0754c8`  
		Last Modified: Thu, 02 Mar 2023 04:24:13 GMT  
		Size: 1.1 MB (1078985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:414cc0e8a0de2287e81a0a4edfca278b7b3c1a0ee11cf79d4130f1536bce0b4f`  
		Last Modified: Thu, 02 Mar 2023 04:24:20 GMT  
		Size: 34.4 MB (34439036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7e932403d3f882224c1a6de81931293f36e00ee68e206ed85d44fed65a8c6d`  
		Last Modified: Thu, 02 Mar 2023 04:24:13 GMT  
		Size: 3.2 MB (3170227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8309e214262e7c6252c28a6e86ee6a809a0c2a514a1b739b69beb5c451ab3be`  
		Last Modified: Thu, 02 Mar 2023 05:22:19 GMT  
		Size: 4.0 MB (4032319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.9` - windows version 10.0.20348.1547; amd64

```console
$ docker pull hylang@sha256:e0a5f1d1393f5e306ba7fe00b4bd96bc85d2789c58792ea186fa1e431ee09cb7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1731546128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e658579b156e904d2e689bbf44f25e9b3d7bdc85eb091b85882abd4f1290812`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Tue, 07 Feb 2023 11:42:22 GMT
RUN Install update 10.0.20348.1547
# Wed, 15 Feb 2023 22:37:49 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 05:30:01 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:30:46 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:30:47 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 16 Feb 2023 05:32:03 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '57faad132d42d3e7a6406fcffafffe0b4f390cf0e2966abb8090d073c6edf405'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:32:04 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 16 Feb 2023 05:32:05 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 16 Feb 2023 05:34:01 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:34:03 GMT
CMD ["pypy"]
# Thu, 16 Feb 2023 08:51:54 GMT
ENV HY_VERSION=0.26.0
# Thu, 16 Feb 2023 08:51:55 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 16 Feb 2023 08:54:48 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 16 Feb 2023 08:54:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d015a9e7adea898d81486dce8b513b0e9cbeca30904cac18c3ea98ab3be7a6`  
		Last Modified: Thu, 16 Feb 2023 00:28:01 GMT  
		Size: 293.3 MB (293317272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9c63a3d1906c0f8f7ca38587ab5f1c84160f9127cce25fb7f57d8a60dc7008`  
		Last Modified: Thu, 16 Feb 2023 00:26:46 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad006479ffac32867154bc9570ff452fcb7c37580b8242b18b7db53b8b59654`  
		Last Modified: Thu, 16 Feb 2023 08:32:17 GMT  
		Size: 769.5 KB (769463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace183ad9c1518bebe41951797d69049d8c98bb4453a88784ceafb86bc461eef`  
		Last Modified: Thu, 16 Feb 2023 08:32:19 GMT  
		Size: 15.8 MB (15761410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00906f2ef0ad2385f0a1ee4915c755048b11f2e5b390386eded3804918af326`  
		Last Modified: Thu, 16 Feb 2023 08:32:15 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3048ad15163aa04fe0b90d4f67206f7b0abf48764387c8b9827a88bbae53953`  
		Last Modified: Thu, 16 Feb 2023 08:32:26 GMT  
		Size: 26.9 MB (26851391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8014a72f693a3bbe5106fce553eb918100e44d8c5f21952d56e9403c8caf383`  
		Last Modified: Thu, 16 Feb 2023 08:32:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f2c8da72073140937b96431fb067103b95d36ee80eb721cb6ae91b3e1a04cf`  
		Last Modified: Thu, 16 Feb 2023 08:32:12 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d3bfd880190697f22216252aa7464855621c7ca5013f040e685024d53457de`  
		Last Modified: Thu, 16 Feb 2023 08:32:19 GMT  
		Size: 3.8 MB (3768846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e6fa1740f16c65d66e5fc4afb452e79b7c66a735844ac242c1932d1a245884`  
		Last Modified: Thu, 16 Feb 2023 08:32:13 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfbe1886a5d254e7e38a69f46dcbbabfbb579a64c21f0137f8b6ba484503ca3`  
		Last Modified: Tue, 28 Feb 2023 01:17:03 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fd2addd2daff410b500fa6f597c25a2ab32bb0c4a46d469b60096630a7f9b1b`  
		Last Modified: Tue, 28 Feb 2023 01:17:03 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6573a60105e791343c4ca917ed24e822c7397be77da992deb8fd7f2ad74e3d0f`  
		Last Modified: Tue, 28 Feb 2023 01:17:05 GMT  
		Size: 5.0 MB (5037382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ed5e600b80131cdeebcbdafd6eafd80d372690a211d3348a70cfb939029f32`  
		Last Modified: Tue, 28 Feb 2023 01:17:03 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.9` - windows version 10.0.17763.4010; amd64

```console
$ docker pull hylang@sha256:3191939d837b2ccc48b0f468e61ae701cd3234319a08a3e6a75b156068a3d648
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2013885229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:635ac6f3ec1d8e0d76f7b4230d7d2cecb017c4ab115658c0d6d1f4080a7bdd14`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Wed, 15 Feb 2023 22:41:28 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Feb 2023 05:35:46 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:37:17 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:37:18 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 16 Feb 2023 05:39:32 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.11-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '57faad132d42d3e7a6406fcffafffe0b4f390cf0e2966abb8090d073c6edf405'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.11-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:39:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 16 Feb 2023 05:39:34 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 16 Feb 2023 05:42:36 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Thu, 16 Feb 2023 05:42:38 GMT
CMD ["pypy"]
# Thu, 16 Feb 2023 08:55:09 GMT
ENV HY_VERSION=0.26.0
# Thu, 16 Feb 2023 08:55:10 GMT
ENV HYRULE_VERSION=0.3.0
# Thu, 16 Feb 2023 08:59:22 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Thu, 16 Feb 2023 08:59:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a5753d4956d637f7e88bedf0b91260e724500d9fa9b91c0a9ed419263659a9a`  
		Last Modified: Thu, 16 Feb 2023 00:28:25 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1a361b8441126a686a24bb6deea0bba50055328e15fdcb29fe389f052ee527`  
		Last Modified: Thu, 16 Feb 2023 08:32:56 GMT  
		Size: 511.9 KB (511942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07aa6101c78d58c681c60d015ca21d23cc2833bccc6519d6d74fa014cbcbb5ba`  
		Last Modified: Thu, 16 Feb 2023 08:32:59 GMT  
		Size: 15.5 MB (15511657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13dbdf99ef2f438b57c688a7bc5cd99816a2a97e0d543cff7ab79e40d839e58`  
		Last Modified: Thu, 16 Feb 2023 08:32:55 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaff92769ad50ea069a02d00aba0e8029c88808f518803019afd6871100180a1`  
		Last Modified: Thu, 16 Feb 2023 08:33:06 GMT  
		Size: 26.6 MB (26618225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d5412654e3c25f0d46317ec9b6ace8a48276d2271fd5f3629b38393ce0b129`  
		Last Modified: Thu, 16 Feb 2023 08:32:52 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97efcdee4de8eea51fc74889a8b51756e573306dacf28de4d6e33ee70ed00426`  
		Last Modified: Thu, 16 Feb 2023 08:32:52 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bb2776582a5cd3798d06f037cdbbcc7df2f20525a2a2494714aa9cdbb611b15`  
		Last Modified: Thu, 16 Feb 2023 08:32:59 GMT  
		Size: 3.5 MB (3534948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89bb447b882bccb0b1b4665c4681ab18cabc545df15a54cc8295f23cb84512d0`  
		Last Modified: Thu, 16 Feb 2023 08:32:52 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfc0f02a8b8b70c10f111316a21c47490b6ed58ecbf8b75186f6ad30b6b2ade8`  
		Last Modified: Tue, 28 Feb 2023 01:17:31 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30079a0f86b488c1905100178fb0635fd74384223380c2ec2b917fa4e98b77ce`  
		Last Modified: Tue, 28 Feb 2023 01:17:31 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2943cbc97d3dc43a665d0832662996d58965c936d0187d9b9fb9a2ea27d8ce99`  
		Last Modified: Tue, 28 Feb 2023 01:17:34 GMT  
		Size: 4.7 MB (4739373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815c88f36cdd400c4e347cd87b8f85607de52d7fe01e147ad114a1aff26285a7`  
		Last Modified: Tue, 28 Feb 2023 01:17:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
