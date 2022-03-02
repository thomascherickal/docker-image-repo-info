## `hylang:pypy3.9-buster`

```console
$ docker pull hylang@sha256:2cd1a2ee421f80cd31b13a35cc90dc6c84a90c3d1dc80c6237bdcd760866f101
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; 386
	-	linux; s390x

### `hylang:pypy3.9-buster` - linux; amd64

```console
$ docker pull hylang@sha256:53f0981370cd5de019e393fc9ca6ad6fe5e2654905f673597cd21379cf96aeed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71954039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4054fa2cb746a8ade29e313760b2f6d3df87e228bb94935a2f9a70edccc31899`
-	Default Command: `["hy"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:59 GMT
ADD file:c51141702f568a28a7e3e7a2748f5ead5754e32d7b1cf7ebc8f4326273d05206 in / 
# Wed, 26 Jan 2022 01:40:59 GMT
CMD ["bash"]
# Thu, 27 Jan 2022 02:06:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jan 2022 02:06:02 GMT
ENV LANG=C.UTF-8
# Thu, 27 Jan 2022 02:06:02 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Feb 2022 01:25:33 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 23 Feb 2022 01:26:01 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux64.tar.bz2'; 			sha256='129a055032bba700cd1d0acacab3659cf6b7180e25b1b2f730e792f06d5b3010'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-aarch64.tar.bz2'; 			sha256='89d7ee12a8c416e83fae80af82482531fc6502321e75e5b7a0cc01d756ee5f0e'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux32.tar.bz2'; 			sha256='a0d18e4e73cc655eb02354759178b8fb161d3e53b64297d05e2fff91f7cf862d'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-s390x.tar.bz2'; 			sha256='37b596bfe76707ead38ffb565629697e9b6fa24e722acc3c632b41ec624f5d95'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 23 Feb 2022 01:26:01 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 23 Feb 2022 01:26:01 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 23 Feb 2022 01:26:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 23 Feb 2022 01:26:13 GMT
CMD ["pypy3"]
# Wed, 23 Feb 2022 22:20:37 GMT
ENV HY_VERSION=1.0a4
# Wed, 23 Feb 2022 22:20:37 GMT
ENV HYRULE_VERSION=0.1
# Wed, 23 Feb 2022 22:20:42 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 23 Feb 2022 22:20:42 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:6552179c3509e3c4314b4065e0d2790563d01cd474e2fdd58be4d46acd48af6a`  
		Last Modified: Wed, 26 Jan 2022 01:47:31 GMT  
		Size: 27.2 MB (27153731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8f922fe49f2aee573854860b2e0443934b4d089bb4f6d83e881e4f4adfd06c`  
		Last Modified: Thu, 27 Jan 2022 02:16:47 GMT  
		Size: 2.8 MB (2757961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d6510b6022149ef8bd0f46678facd26bb72ecdcb1ceb1788ec4d83636f70ef4`  
		Last Modified: Wed, 23 Feb 2022 01:36:38 GMT  
		Size: 36.6 MB (36573292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b17bbdae937c8b0b5294943c90a1758c3b4f6f0e34b2c0692fc028c13e180af`  
		Last Modified: Wed, 23 Feb 2022 01:36:33 GMT  
		Size: 2.6 MB (2634649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d220ab8e3720b9184fc942b96f26ca3ce7ff569b12174c0b1c3d189662edbbbe`  
		Last Modified: Wed, 23 Feb 2022 22:22:36 GMT  
		Size: 2.8 MB (2834406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9-buster` - linux; 386

```console
$ docker pull hylang@sha256:5fcef85b60bc3565c6f4c7df2f5b0438c87258cd27f166dcda5a24e79138475a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.3 MB (75256290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:733a5959463aa508bc4d10b32fa7ec70d5baeefb9facad9ed2ed82e3e8a0e626`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:08:04 GMT
ADD file:d9d384f0402bc696e46e7529f52d64859a66aa7a60bca9c7beee7433a5f7af6e in / 
# Tue, 01 Mar 2022 02:08:04 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 21:20:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 21:20:32 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 21:20:33 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 21:20:33 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 02 Mar 2022 09:09:30 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux64.tar.bz2'; 			sha256='129a055032bba700cd1d0acacab3659cf6b7180e25b1b2f730e792f06d5b3010'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-aarch64.tar.bz2'; 			sha256='89d7ee12a8c416e83fae80af82482531fc6502321e75e5b7a0cc01d756ee5f0e'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux32.tar.bz2'; 			sha256='a0d18e4e73cc655eb02354759178b8fb161d3e53b64297d05e2fff91f7cf862d'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-s390x.tar.bz2'; 			sha256='37b596bfe76707ead38ffb565629697e9b6fa24e722acc3c632b41ec624f5d95'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 02 Mar 2022 09:09:31 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 02 Mar 2022 09:09:31 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 02 Mar 2022 09:09:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 02 Mar 2022 09:09:45 GMT
CMD ["pypy3"]
# Wed, 02 Mar 2022 09:34:12 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 09:34:12 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 09:34:17 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 09:34:17 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:c761ce6f2bf0aed07e1198c6f827444969d6e76dda0e55dbb45900920e551d27`  
		Last Modified: Tue, 01 Mar 2022 02:16:51 GMT  
		Size: 27.8 MB (27804590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2fa69f8281d0c88d1c268092ba8dbb609cfa2a0eeb0b72e7acfdc35b5c255d`  
		Last Modified: Tue, 01 Mar 2022 21:40:45 GMT  
		Size: 2.8 MB (2769490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7c98a6ee81b0fc67140eeb8d5a97bd4e11859064de452257ef40e5e8d4845c`  
		Last Modified: Wed, 02 Mar 2022 09:24:47 GMT  
		Size: 39.2 MB (39213187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9206f9735ab6f10b0167138b3c4f628e492f10743c634724a17e161f661dca`  
		Last Modified: Wed, 02 Mar 2022 09:24:37 GMT  
		Size: 2.6 MB (2634835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45679e5c4861b9dba307d89c99f77d8820aba1430b3b502b98d29ea5dffffd23`  
		Last Modified: Wed, 02 Mar 2022 09:41:07 GMT  
		Size: 2.8 MB (2834188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hylang:pypy3.9-buster` - linux; s390x

```console
$ docker pull hylang@sha256:a288b47404e29638ec719326051ce1667a2d8a808863b910ca82ba26363db08c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68790251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d81daff60feb84b5a9f9f8ae9b0ec900cf568117808c3a4b820b6539bb1d0232`
-	Default Command: `["hy"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:27 GMT
ADD file:908bd36a2b17b792aa02339ed6a72d1051267279d72330b1c5cd8617ca5d819e in / 
# Tue, 01 Mar 2022 02:02:28 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 10:13:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends ca-certificates; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 10:13:42 GMT
ENV LANG=C.UTF-8
# Tue, 01 Mar 2022 10:13:42 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Mar 2022 10:13:42 GMT
ENV PYPY_VERSION=7.3.8
# Wed, 02 Mar 2022 01:42:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux64.tar.bz2'; 			sha256='129a055032bba700cd1d0acacab3659cf6b7180e25b1b2f730e792f06d5b3010'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-aarch64.tar.bz2'; 			sha256='89d7ee12a8c416e83fae80af82482531fc6502321e75e5b7a0cc01d756ee5f0e'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-linux32.tar.bz2'; 			sha256='a0d18e4e73cc655eb02354759178b8fb161d3e53b64297d05e2fff91f7cf862d'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy3.9-v7.3.8-s390x.tar.bz2'; 			sha256='37b596bfe76707ead38ffb565629697e9b6fa24e722acc3c632b41ec624f5d95'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		wget 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy3' /usr/local/bin/; 		pypy3 --version; 		cd /opt/pypy/lib/pypy3.9; 	if [ -f _gdbm_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libgdbm-dev; 		pypy3 _gdbm_build.py; 	fi; 	if [ -f _ssl_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libssl-dev; 		pypy3 _ssl_build.py; 	fi; 	if [ -f _lzma_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev liblzma-dev; 		pypy3 _lzma_build.py; 	fi; 	if [ -f _sqlite3_build.py ]; then 		apt-get install -y --no-install-recommends gcc libc6-dev libsqlite3-dev; 		pypy3 _sqlite3_build.py; 	fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy3 --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Wed, 02 Mar 2022 01:42:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 02 Mar 2022 01:42:36 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 02 Mar 2022 01:42:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends wget; 	rm -rf /var/lib/apt/lists/*; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy3 -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy3 get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	apt-get purge -y --auto-remove wget; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Wed, 02 Mar 2022 01:42:46 GMT
CMD ["pypy3"]
# Wed, 02 Mar 2022 02:06:19 GMT
ENV HY_VERSION=1.0a4
# Wed, 02 Mar 2022 02:06:19 GMT
ENV HYRULE_VERSION=0.1
# Wed, 02 Mar 2022 02:06:23 GMT
RUN pip install --no-cache-dir "hy == $HY_VERSION" "hyrule == $HYRULE_VERSION"
# Wed, 02 Mar 2022 02:06:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:cb73b674076b2da947cefa0692c1d193bda8bfd443c178f9bb39bbae7656ead8`  
		Last Modified: Tue, 01 Mar 2022 02:08:05 GMT  
		Size: 25.8 MB (25769053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09aaf957a3af05d974bd1245a06df174f1c8119b5cc605286be610ed8ae423b`  
		Last Modified: Tue, 01 Mar 2022 10:18:37 GMT  
		Size: 2.5 MB (2452746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7626fc7e4c124f806eae8531bc7b39e0b3e65f6b2345f5e4057c3082eef02a5c`  
		Last Modified: Wed, 02 Mar 2022 01:47:27 GMT  
		Size: 35.1 MB (35099133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d7f4017fab9ebf0fe41859c7cf6c2f7efbe61e85ae1d70766ffd38cf0796cd9`  
		Last Modified: Wed, 02 Mar 2022 01:47:21 GMT  
		Size: 2.6 MB (2635095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114bf60b9271c5c832377aaf5586c5a4b9b43bd9bacb0fa0bd0596725ae007f7`  
		Last Modified: Wed, 02 Mar 2022 02:09:38 GMT  
		Size: 2.8 MB (2834224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
