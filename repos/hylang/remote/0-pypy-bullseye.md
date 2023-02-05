## `hylang:0-pypy-bullseye`

```console
$ docker pull hylang@sha256:19969b1a5be20f759880d420fc49da48babcaef2881cd848f94ffb8f57787e7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-pypy-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:44006d5e97b293333f218aa8da29425f9534e0540622f5d1a7d3372235f37b10
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.9 MB (75869455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:655ee473609137120099d3e0d225dbecd1387fd68068f7aaacaba9e7ba7dea84`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:14:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:14:03 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 10:14:04 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 10:14:04 GMT
ENV PYPY_VERSION=7.3.11
# Sat, 04 Feb 2023 10:14:36 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 04 Feb 2023 10:14:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 04 Feb 2023 10:14:36 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 04 Feb 2023 10:14:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 04 Feb 2023 10:14:48 GMT
CMD ["pypy3"]
# Sun, 05 Feb 2023 01:42:57 GMT
ENV HY_VERSION=0.25.0
# Sun, 05 Feb 2023 01:42:57 GMT
ENV HYRULE_VERSION=0.2.1
# Sun, 05 Feb 2023 01:43:27 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sun, 05 Feb 2023 01:43:27 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b11e0b6bc0df3479428b6d6c71c16a9a05e94050fad9a222b4ca4746af187e`  
		Last Modified: Sat, 04 Feb 2023 10:23:14 GMT  
		Size: 1.1 MB (1066527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc6edec405cc4d50d66cf7c5c333763b24e988525fa1a840dd6e7311c083fa0`  
		Last Modified: Sat, 04 Feb 2023 10:23:20 GMT  
		Size: 36.2 MB (36187938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb0ac52a7b9a9581ba68eea2795c283bb6fef374723579cf0c289779aa8bed6`  
		Last Modified: Sat, 04 Feb 2023 10:23:14 GMT  
		Size: 3.2 MB (3170651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29201c1c0bc5dce3b51d383aede5225714a6e0f4075e7bdd252cf4da3ad868f9`  
		Last Modified: Sun, 05 Feb 2023 01:50:51 GMT  
		Size: 4.0 MB (4047420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:530e28c7978515bf5c6941cf88bfd2650de3310e3ec5e52691b181c21563c21f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (72009621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0f51bf70e79ab6d947b4f324ae6f0ca24a6e45097b0d92683cbaf332627282`
-	Default Command: `["hy"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 13:31:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 13:31:09 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 13:31:09 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 13:31:09 GMT
ENV PYPY_VERSION=7.3.11
# Sat, 04 Feb 2023 13:31:35 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Sat, 04 Feb 2023 13:31:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Sat, 04 Feb 2023 13:31:36 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Sat, 04 Feb 2023 13:31:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Sat, 04 Feb 2023 13:31:47 GMT
CMD ["pypy3"]
# Sun, 05 Feb 2023 00:16:59 GMT
ENV HY_VERSION=0.25.0
# Sun, 05 Feb 2023 00:16:59 GMT
ENV HYRULE_VERSION=0.2.1
# Sun, 05 Feb 2023 00:17:29 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Sun, 05 Feb 2023 00:17:29 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94d355ce69d649276dc220c3dfad9c0be5263fbc905a47c71e5cb93b76e493f`  
		Last Modified: Sat, 04 Feb 2023 13:39:27 GMT  
		Size: 1.1 MB (1054066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138768774c2dcccef9cbffeb31c873b60e34363b31de80ea4d3385acdd8ab9d2`  
		Last Modified: Sat, 04 Feb 2023 13:39:31 GMT  
		Size: 33.7 MB (33692941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dacc90fbb35934c105762f32cedfef6a0f9c79781def1a1846db344dfbe22ac3`  
		Last Modified: Sat, 04 Feb 2023 13:39:27 GMT  
		Size: 3.2 MB (3170351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc8b57a177b61a80d796fa39e2c312264d3cd58b58f5637f093d234b594040d`  
		Last Modified: Sun, 05 Feb 2023 00:25:07 GMT  
		Size: 4.0 MB (4047471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:bd1dfb2b905a43d059e4a94d006e9dccf50bebfb514815cee9e3d356fdde6a22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.7 MB (74673539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab22a57a8a3ca7ae539480edc8f18c06650d16ff796233cf7bc843dfd52366b2`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 11 Jan 2023 03:16:08 GMT
ADD file:68afc7c49a947a9fb253ffeba9950cdc39e241f8a5cf0133043cfc612447f597 in / 
# Wed, 11 Jan 2023 03:16:08 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 12:02:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 12:02:11 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 12:02:12 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 12:02:13 GMT
ENV PYPY_VERSION=7.3.11
# Wed, 11 Jan 2023 12:02:47 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux64.tar.bz2'; 			sha256='d506172ca11071274175d74e9c581c3166432d0179b036470e3b9e8d20eae581'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-aarch64.tar.bz2'; 			sha256='09175dc652ed895d98e9ad63d216812bf3ee7e398d900a9bf9eb2906ba8302b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-linux32.tar.bz2'; 			sha256='0099d72c2897b229057bff7e2c343624aeabdc60d6fb43ca882bff082f1ffa48'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.11-s390x.tar.bz2'; 			sha256='e1f30f2ddbe3f446ddacd79677b958d56c07463b20171fb2abf8f9a3178b79fc'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 11 Jan 2023 12:02:47 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 11 Jan 2023 12:02:48 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 11 Jan 2023 12:03:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 11 Jan 2023 12:03:04 GMT
CMD ["pypy3"]
# Wed, 11 Jan 2023 22:05:54 GMT
ENV HY_VERSION=0.25.0
# Wed, 11 Jan 2023 22:05:55 GMT
ENV HYRULE_VERSION=0.2.1
# Wed, 11 Jan 2023 22:06:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 11 Jan 2023 22:06:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:165165b78fad597abd0883f40adcaa0edcfe981a358deea181323680a07b7011`  
		Last Modified: Wed, 11 Jan 2023 03:22:01 GMT  
		Size: 32.4 MB (32375738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:435d3cd1791ff564259c0272b3f25ff4baec8c2625b9f26edab8e6f00147461c`  
		Last Modified: Wed, 11 Jan 2023 12:15:31 GMT  
		Size: 1.1 MB (1078739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0585cbcbdbd4f1389b5aec69256036cb9c9162450166c4a7035adeda3aeef934`  
		Last Modified: Wed, 11 Jan 2023 12:15:36 GMT  
		Size: 34.2 MB (34220216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6f4d6676db3f469ee3682c425cad18d01dbe4dfb2589b0b394c0c2e8dddb6d`  
		Last Modified: Wed, 11 Jan 2023 12:15:31 GMT  
		Size: 3.0 MB (2951520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281919a9e4e3b5fe0998e716afaee360790cf827b19d23837f3ad68b8e9dec07`  
		Last Modified: Wed, 11 Jan 2023 22:18:14 GMT  
		Size: 4.0 MB (4047326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
