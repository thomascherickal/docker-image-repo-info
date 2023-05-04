## `pypy:2-bullseye`

```console
$ docker pull pypy@sha256:424cb6c11aee13894bfd7464d4d732f95957262a4c729bb49497ef819d872753
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `pypy:2-bullseye` - linux; amd64

```console
$ docker pull pypy@sha256:6d5250dc5ba4c8fee4fbbdfc48414aff65dde4f13b9813564f11495345bbea11
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.6 MB (358580012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0afa1cfbc144e0f3c60a13fb606b98c6753dcf70c03690ab08bc38bb76503e7`
-	Default Command: `["pypy"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:58:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:59:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 11:20:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 11:20:14 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 11:20:14 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 11:20:14 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 04 May 2023 11:22:44 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-linux64.tar.bz2'; 			sha256='ba8ed958a905c0735a4cfff2875c25089954dc020e087d982b0ffa5b9da316cd'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-aarch64.tar.bz2'; 			sha256='ea924da1defe9325ef760e288b04f984614e405580f5321eb6a5c8f539bd415a'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-linux32.tar.bz2'; 			sha256='30fd245fab7068c96a75b9ff1323ac55174c64fc8c4751cceb4b7a9bedc1851e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-s390x.tar.bz2'; 			sha256='8fe9481c473178e53266983678684a70fe0c42bafc95f1807bf3ef28770316d4'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 04 May 2023 11:22:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 04 May 2023 11:22:45 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 04 May 2023 11:22:50 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 May 2023 11:22:50 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eedd9c5abf7e5f63753a5e788cb0872a715fa1141e8ce5ea87638e6cd370a41`  
		Last Modified: Wed, 03 May 2023 20:13:22 GMT  
		Size: 54.6 MB (54584552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cdadd40055fb82fef74a0a38f29fb1ee7b6922e18370ebdc3502ec66f79fa3f`  
		Last Modified: Wed, 03 May 2023 20:13:55 GMT  
		Size: 196.8 MB (196849980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d17445bd16cc1a587cfd3fca360849983a86fa65aaca5dd662c35ac66ce8a1d`  
		Last Modified: Thu, 04 May 2023 11:24:08 GMT  
		Size: 3.2 MB (3210762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8163a2ac3a955f25d4699d8b5e197ee15b9adac8cae309fa9be5bc874af183de`  
		Last Modified: Thu, 04 May 2023 11:25:48 GMT  
		Size: 31.2 MB (31228726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1783d1bb94193c4672d58d29afba466475d213e6bcb20498d54523278aa8d323`  
		Last Modified: Thu, 04 May 2023 11:25:43 GMT  
		Size: 1.9 MB (1896582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-bullseye` - linux; arm64 variant v8

```console
$ docker pull pypy@sha256:9b9d188c6d1e4aaebc677af36a2a7011b5d8658f917e31b75a2c2c5702aefd41
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.3 MB (348252185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eebc833f0989b67429892821a8d395bc61691d48ebfc757db2e4ca56e2178b6`
-	Default Command: `["pypy"]`

```dockerfile
# Wed, 03 May 2023 00:22:41 GMT
ADD file:f930fdb659332a615b0042ca415d6d7feda9ba6b2f58222e3e5bbed326db4d40 in / 
# Wed, 03 May 2023 00:22:42 GMT
CMD ["bash"]
# Wed, 03 May 2023 17:21:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:21:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 17:22:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:10:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:10:43 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 08:10:43 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 08:10:43 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 04 May 2023 08:12:59 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-linux64.tar.bz2'; 			sha256='ba8ed958a905c0735a4cfff2875c25089954dc020e087d982b0ffa5b9da316cd'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-aarch64.tar.bz2'; 			sha256='ea924da1defe9325ef760e288b04f984614e405580f5321eb6a5c8f539bd415a'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-linux32.tar.bz2'; 			sha256='30fd245fab7068c96a75b9ff1323ac55174c64fc8c4751cceb4b7a9bedc1851e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-s390x.tar.bz2'; 			sha256='8fe9481c473178e53266983678684a70fe0c42bafc95f1807bf3ef28770316d4'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 04 May 2023 08:13:00 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 04 May 2023 08:13:00 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 04 May 2023 08:13:05 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 May 2023 08:13:05 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:d677c78be691f8dcbe9d44ce576b97ad205b3dd78557dc62794e59eb19553ee9`  
		Last Modified: Wed, 03 May 2023 00:25:31 GMT  
		Size: 53.7 MB (53692705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73587d290df17347645f166c8385f0a2d320a31f4803658f619f2887a5d88faf`  
		Last Modified: Wed, 03 May 2023 17:36:59 GMT  
		Size: 15.7 MB (15746737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd49b43770afa984b42a50282487e41b4ca05ba0e9f8bf233e6fc6d2fa99353e`  
		Last Modified: Wed, 03 May 2023 17:37:15 GMT  
		Size: 54.7 MB (54675990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a96e84daab7feb81c20a699d776f6cb02383bdcc7f2b02d4f3af942e740c2a`  
		Last Modified: Wed, 03 May 2023 17:37:47 GMT  
		Size: 189.8 MB (189773685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3386c2b87afddb89d9da06e042344dd59c1e111a6fb94889ae22fe4a47621d24`  
		Last Modified: Thu, 04 May 2023 08:14:18 GMT  
		Size: 3.2 MB (3214865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90759e02a6c71cbbfd960dff45b9865ce44334fdb132738b6fd9f0e8487d139`  
		Last Modified: Thu, 04 May 2023 08:15:51 GMT  
		Size: 29.3 MB (29251591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808d806ad344618848c5d09afc8067e79f2b9e6cc2740446dcaf7ba1fe827a5e`  
		Last Modified: Thu, 04 May 2023 08:15:47 GMT  
		Size: 1.9 MB (1896612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `pypy:2-bullseye` - linux; 386

```console
$ docker pull pypy@sha256:92887993a75d9f22f89b396395a9cb76a831ed091d44bf521c368997c64f247e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **360.5 MB (360528891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81f70772c5e955749a0adc6082a7dd2def4377221a352f73b216f044ef5b0a5b`
-	Default Command: `["pypy"]`

```dockerfile
# Wed, 03 May 2023 00:00:45 GMT
ADD file:59d53253d7691be0330c735eb4b57791a8fc5894572d3deaeb7138cce45132ad in / 
# Wed, 03 May 2023 00:00:46 GMT
CMD ["bash"]
# Wed, 03 May 2023 22:28:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:29:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 22:30:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:12:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		tcl 		tk 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 08:12:33 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 08:12:33 GMT
ENV PATH=/opt/pypy/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 May 2023 08:12:33 GMT
ENV PYPY_VERSION=7.3.11
# Thu, 04 May 2023 08:15:34 GMT
RUN set -eux; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		'amd64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-linux64.tar.bz2'; 			sha256='ba8ed958a905c0735a4cfff2875c25089954dc020e087d982b0ffa5b9da316cd'; 			;; 		'arm64') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-aarch64.tar.bz2'; 			sha256='ea924da1defe9325ef760e288b04f984614e405580f5321eb6a5c8f539bd415a'; 			;; 		'i386') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-linux32.tar.bz2'; 			sha256='30fd245fab7068c96a75b9ff1323ac55174c64fc8c4751cceb4b7a9bedc1851e'; 			;; 		's390x') 			url='https://downloads.python.org/pypy/pypy2.7-v7.3.11-s390x.tar.bz2'; 			sha256='8fe9481c473178e53266983678684a70fe0c42bafc95f1807bf3ef28770316d4'; 			;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding PyPy $PYPY_VERSION binary release"; exit 1 ;; 	esac; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libexpat1 		libncurses5 		libncursesw6 		libsqlite3-0 	; 		wget -O pypy.tar.bz2 "$url" --progress=dot:giga; 	echo "$sha256 *pypy.tar.bz2" | sha256sum --check --strict -; 	mkdir /opt/pypy; 	tar -xjC /opt/pypy --strip-components=1 -f pypy.tar.bz2; 	find /opt/pypy/lib* -depth -type d -a \( -name test -o -name tests \) -exec rm -rf '{}' +; 	rm pypy.tar.bz2; 		ln -sv '/opt/pypy/bin/pypy' /usr/local/bin/; 		pypy --version; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark > /dev/null; 	find /opt/pypy -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 	pypy --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +
# Thu, 04 May 2023 08:15:35 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Thu, 04 May 2023 08:15:35 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Thu, 04 May 2023 08:15:41 GMT
RUN set -ex; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum --check --strict -; 		pipVersion="$(pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)')"; 	setuptoolsVersion="$(pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)')"; 		pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		"pip == $pipVersion" 		"setuptools == $setuptoolsVersion" 	; 	pip --version; 		find /opt/pypy -depth 		\( 			\( -type d -a \( -name test -o -name tests \) \) 			-o 			\( -type f -a \( -name '*.pyc' -o -name '*.pyo' \) \) 		\) -exec rm -rf '{}' +; 	rm -f get-pip.py
# Thu, 04 May 2023 08:15:42 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:6ac0eb37fce5e6fca952bf804df5de5ebb63724d4d44bf23abc5d5736ee32afd`  
		Last Modified: Wed, 03 May 2023 00:04:44 GMT  
		Size: 56.0 MB (56029150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de21dcd769e703c034c16b0e5b92aecd56468d2eb0a9c1719775735654f8cf3`  
		Last Modified: Wed, 03 May 2023 22:36:04 GMT  
		Size: 16.3 MB (16263234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed46c5383778b8d3b20b09e9296d4d8ecdb363c3436f0188d69ef066bed07cbb`  
		Last Modified: Wed, 03 May 2023 22:36:26 GMT  
		Size: 55.9 MB (55922651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfa5b0eba28a6e85b96b76f161af708d6f1d0015d7e7955e025f7fcddc506141`  
		Last Modified: Wed, 03 May 2023 22:37:11 GMT  
		Size: 199.8 MB (199763056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6457c59e2566b0a04b3e37a29a628f688f476f3227d7aac0a38593a4729d2bef`  
		Last Modified: Thu, 04 May 2023 08:17:00 GMT  
		Size: 3.4 MB (3360889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2565fa6082f73f43fc21929648e1cfcfaf87dad3560c494d11bf6bc25aa26db9`  
		Last Modified: Thu, 04 May 2023 08:18:47 GMT  
		Size: 27.3 MB (27293337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f7eec82d401ef0ee712ae1e6e426a054c10cdb2afaa03c7b315cdc1cf74ed1`  
		Last Modified: Thu, 04 May 2023 08:18:41 GMT  
		Size: 1.9 MB (1896574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
