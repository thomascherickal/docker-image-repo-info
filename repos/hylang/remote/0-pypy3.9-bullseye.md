## `hylang:0-pypy3.9-bullseye`

```console
$ docker pull hylang@sha256:7c0d04c62ffa6e691224e3d974c3516cec8bdc588adcec33baa272396d248705
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `hylang:0-pypy3.9-bullseye` - linux; amd64

```console
$ docker pull hylang@sha256:a227674d2925c0a1aba7f45f49d35293b6bfbb114e523cd264d9e05879bd637e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.7 MB (76693683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:218095c855ca8f86b6474dd876978ded84b49b17a5dbedcc945574aac875171d`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:12:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:12:23 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 09:12:24 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 09:12:24 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 05 Oct 2022 09:12:56 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux64.tar.bz2'; 			sha256='46818cb3d74b96b34787548343d266e2562b531ddbaf330383ba930ff1930ed5'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-aarch64.tar.bz2'; 			sha256='2e1ae193d98bc51439642a7618d521ea019f45b8fb226940f7e334c548d2b4b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux32.tar.bz2'; 			sha256='0de4b9501cf28524cdedcff5052deee9ea4630176a512bdc408edfa30914bae7'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-s390x.tar.bz2'; 			sha256='774dca83bcb4403fb99b3d155e7bd572ef8c52b9fe87a657109f64e75ad71732'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 05 Oct 2022 09:12:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 05 Oct 2022 09:12:57 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 05 Oct 2022 09:13:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 05 Oct 2022 09:13:10 GMT
CMD ["pypy3"]
# Thu, 06 Oct 2022 02:37:10 GMT
ENV HY_VERSION=0.24.0
# Thu, 06 Oct 2022 02:37:10 GMT
ENV HYRULE_VERSION=0.2
# Thu, 06 Oct 2022 02:37:43 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Thu, 06 Oct 2022 02:37:43 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9100dcb09907924979fa71f021fece2749671df15d0b6a0c7d48abd4b503f10c`  
		Last Modified: Wed, 05 Oct 2022 09:24:34 GMT  
		Size: 1.1 MB (1066538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a536d4f3fd5651490e5e915f72f5f42020c46d236acda25d9478b0a7525152f`  
		Last Modified: Wed, 05 Oct 2022 09:24:37 GMT  
		Size: 37.1 MB (37067851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906e30fb6d7a27502d16f60251cb8b3025eb286859f19fc3fe2fb011f7bf6e31`  
		Last Modified: Wed, 05 Oct 2022 09:24:34 GMT  
		Size: 3.2 MB (3170706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494482f4964bce7483eded760aa374a123bc3d6a7afcccca3db087d9f979030a`  
		Last Modified: Thu, 06 Oct 2022 02:45:54 GMT  
		Size: 4.0 MB (3968486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.9-bullseye` - linux; arm64 variant v8

```console
$ docker pull hylang@sha256:7018ef5a90bd73e2f92374892d996e960f63855ca61beccdbfb4b5769c520798
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.2 MB (72213639 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5e295bb6d491a483ce78883d761b627b2bbe035ac6566c342232a2abf4dcb41`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:56:32 GMT
ENV LANG=C.UTF-8
# Wed, 05 Oct 2022 12:56:33 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 05 Oct 2022 12:56:34 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 05 Oct 2022 12:57:05 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux64.tar.bz2'; 			sha256='46818cb3d74b96b34787548343d266e2562b531ddbaf330383ba930ff1930ed5'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-aarch64.tar.bz2'; 			sha256='2e1ae193d98bc51439642a7618d521ea019f45b8fb226940f7e334c548d2b4b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux32.tar.bz2'; 			sha256='0de4b9501cf28524cdedcff5052deee9ea4630176a512bdc408edfa30914bae7'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-s390x.tar.bz2'; 			sha256='774dca83bcb4403fb99b3d155e7bd572ef8c52b9fe87a657109f64e75ad71732'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 05 Oct 2022 12:57:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 05 Oct 2022 12:57:06 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 05 Oct 2022 12:57:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 05 Oct 2022 12:57:21 GMT
CMD ["pypy3"]
# Tue, 25 Oct 2022 07:31:05 GMT
ENV HY_VERSION=0.24.0
# Tue, 25 Oct 2022 07:31:05 GMT
ENV HYRULE_VERSION=0.2
# Tue, 25 Oct 2022 07:31:35 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 25 Oct 2022 07:31:35 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19adae9723d5098eecfbd9d7fed6afaa97f05d9b161bc9c4098031406553bf86`  
		Last Modified: Wed, 05 Oct 2022 13:13:34 GMT  
		Size: 849.6 KB (849581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2970597c5023e8f4e7ac95a92cd9554e876c1cb39969e77e46aa790ef0b9ec9c`  
		Last Modified: Wed, 05 Oct 2022 13:13:40 GMT  
		Size: 34.4 MB (34351081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dd32f44ff889470a5fed455eac177309f08d49b5ae21ae66c62a62d4ece758`  
		Last Modified: Wed, 05 Oct 2022 13:13:34 GMT  
		Size: 3.0 MB (2951791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16f4166f91a837570303d534cd9b812212b1b184444f3c3c5e705bb1ff0ac9a`  
		Last Modified: Tue, 25 Oct 2022 07:41:24 GMT  
		Size: 4.0 MB (3996791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:0-pypy3.9-bullseye` - linux; 386

```console
$ docker pull hylang@sha256:5b1a63d7668ca22d2059da946b0b1b1935c460926d06d8025815a9e72ee40ada
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.4 MB (76366176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd206f60b5598a8521ae4a13027207e166c3b4811cec271307b1dd80bd6bf9b1`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:34 GMT
ADD file:14adaece72e410cf04ac21a101e5b530aab1d5e5a189a2be72d195ec0ac5e6d4 in / 
# Tue, 25 Oct 2022 02:22:35 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 10:15:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 10:15:52 GMT
ENV LANG=C.UTF-8
# Tue, 25 Oct 2022 10:15:53 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 25 Oct 2022 10:15:54 GMT
ENV PYPY_VERSION=7.3.9
# Tue, 25 Oct 2022 10:16:28 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux64.tar.bz2'; 			sha256='46818cb3d74b96b34787548343d266e2562b531ddbaf330383ba930ff1930ed5'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-aarch64.tar.bz2'; 			sha256='2e1ae193d98bc51439642a7618d521ea019f45b8fb226940f7e334c548d2b4b9'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-linux32.tar.bz2'; 			sha256='0de4b9501cf28524cdedcff5052deee9ea4630176a512bdc408edfa30914bae7'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.9-s390x.tar.bz2'; 			sha256='774dca83bcb4403fb99b3d155e7bd572ef8c52b9fe87a657109f64e75ad71732'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Tue, 25 Oct 2022 10:16:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 25 Oct 2022 10:16:29 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 25 Oct 2022 10:16:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Tue, 25 Oct 2022 10:16:45 GMT
CMD ["pypy3"]
# Tue, 25 Oct 2022 18:08:31 GMT
ENV HY_VERSION=0.24.0
# Tue, 25 Oct 2022 18:08:32 GMT
ENV HYRULE_VERSION=0.2
# Tue, 25 Oct 2022 18:09:09 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Tue, 25 Oct 2022 18:09:10 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3c83067056c0f1bc4e162249831ac686f3a9a9c64c5366b903581580de8fcac2`  
		Last Modified: Tue, 25 Oct 2022 02:28:26 GMT  
		Size: 32.4 MB (32396384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f34ad0e38cd30386eb11e3298ac0c8eaabc036bcba30d5a2a9d44f330d34c1`  
		Last Modified: Tue, 25 Oct 2022 10:33:20 GMT  
		Size: 874.9 KB (874942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cb6ee7620bad558ff3f6a43c070c728524ea6cdbbaf4f4543b4c8adb8d9cb1`  
		Last Modified: Tue, 25 Oct 2022 10:33:26 GMT  
		Size: 36.1 MB (36146680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5572f7c4dbd80c80b77766cd63f657d1a5843293d278d6be27c3a304ed8277d`  
		Last Modified: Tue, 25 Oct 2022 10:33:20 GMT  
		Size: 3.0 MB (2951442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bcc16fbaea3f21dcc3ea3ec9980c6cef1ff82e4d0896a7d65787b7338743fd`  
		Last Modified: Tue, 25 Oct 2022 18:18:43 GMT  
		Size: 4.0 MB (3996728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
