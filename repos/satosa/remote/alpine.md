## `satosa:alpine`

```console
$ docker pull satosa@sha256:4ba6015c69ba92cd626cff49c9b23d1ddff171872e457445a3b0af437be1fed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `satosa:alpine` - linux; amd64

```console
$ docker pull satosa@sha256:a731c188b048f084b99fb584a2bc89b5665d17d99cd824387d8e572ea9b4971b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42551427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:893a85291e1c592697cb5ad859822c56fbf68d89082c7316bb4501ecbea858bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:29:54 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 23:33:43 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 23:33:45 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 09 Aug 2022 23:33:45 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 07 Sep 2022 22:31:37 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 07 Sep 2022 22:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 07 Sep 2022 22:43:37 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 07 Sep 2022 22:43:37 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 07 Sep 2022 22:43:37 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 07 Sep 2022 22:43:37 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 07 Sep 2022 22:43:37 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 07 Sep 2022 22:43:44 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 07 Sep 2022 22:43:44 GMT
CMD ["python3"]
# Thu, 08 Sep 2022 01:39:22 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Thu, 08 Sep 2022 01:39:22 GMT
ENV SATOSA_VERSION=8.1.1
# Thu, 08 Sep 2022 01:40:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 08 Sep 2022 01:40:06 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 08 Sep 2022 01:40:06 GMT
WORKDIR /etc/satosa
# Thu, 08 Sep 2022 01:40:06 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Thu, 08 Sep 2022 01:40:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Sep 2022 01:40:06 GMT
EXPOSE 8080
# Thu, 08 Sep 2022 01:40:06 GMT
USER satosa:satosa
# Thu, 08 Sep 2022 01:40:06 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2a141cd2277284ebaafc76d13b42cf8a7682e4663298a2a730f18331a95eb6`  
		Last Modified: Wed, 10 Aug 2022 01:10:21 GMT  
		Size: 681.4 KB (681402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e8f1c91cae38570ad1baba1b5e94fd7d1bf92015443f3c2841c4e3813232be`  
		Last Modified: Thu, 08 Sep 2022 00:56:23 GMT  
		Size: 12.5 MB (12515356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20828db47e2ee8630c1a3f5877d3300582cf28161f5dce3b54190b0106be6491`  
		Last Modified: Thu, 08 Sep 2022 00:56:21 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6e0c037c9fb0ad2bbae5bbdf6237c9f19d57554f4c3e010c11e8c37500b07`  
		Last Modified: Thu, 08 Sep 2022 00:56:22 GMT  
		Size: 3.0 MB (3043733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2daf71d1c9c55e84212928c965fc2c2c97da64e50337a8e857b3c605151e3bba`  
		Last Modified: Thu, 08 Sep 2022 01:40:47 GMT  
		Size: 9.4 MB (9406010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab7075b7796aeee6800f01b11dd75cae262df8889b5f8c293fce133a62c3319`  
		Last Modified: Thu, 08 Sep 2022 01:40:48 GMT  
		Size: 14.1 MB (14087085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d5f012762974c96b41a3334bc0d46a3ad53d450200ab657636b203c7dc4d21`  
		Last Modified: Thu, 08 Sep 2022 01:40:45 GMT  
		Size: 9.4 KB (9442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b1279164ccaf53ac3c899c1c1a6e59e15a74a822354bf6290756290916b062`  
		Last Modified: Thu, 08 Sep 2022 01:40:45 GMT  
		Size: 2.1 KB (2114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:alpine` - linux; arm variant v6

```console
$ docker pull satosa@sha256:03079c3a08de3132be780a19a0606958fb1f35d0f9d68d7276833066839cc812
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.9 MB (174861382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40e9f45dd39e78c6b11701840747833ca035ba538d3dd517f636ec1b501ec1e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 17:39:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 17:39:49 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 17:39:51 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 10 Aug 2022 17:39:52 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 10 Aug 2022 18:54:24 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 19:19:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 10 Aug 2022 19:19:40 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 10 Aug 2022 19:19:40 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 19:19:40 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Fri, 12 Aug 2022 03:54:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Fri, 12 Aug 2022 03:54:30 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Fri, 12 Aug 2022 03:54:42 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 12 Aug 2022 03:54:42 GMT
CMD ["python3"]
# Fri, 12 Aug 2022 07:25:37 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Fri, 12 Aug 2022 07:25:37 GMT
ENV SATOSA_VERSION=8.1.1
# Fri, 12 Aug 2022 07:29:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Fri, 12 Aug 2022 07:29:25 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Fri, 12 Aug 2022 07:29:25 GMT
WORKDIR /etc/satosa
# Fri, 12 Aug 2022 07:29:25 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Fri, 12 Aug 2022 07:29:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Aug 2022 07:29:25 GMT
EXPOSE 8080
# Fri, 12 Aug 2022 07:29:25 GMT
USER satosa:satosa
# Fri, 12 Aug 2022 07:29:26 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9accb01a83df969604c0c29e144cfb29f827afa7aaa2aef33764b1c3985780eb`  
		Last Modified: Wed, 10 Aug 2022 23:49:04 GMT  
		Size: 685.8 KB (685849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b575fc891c7384cc6c4df326810986903bedc577c30a3afe4a9a098a6f9878d9`  
		Last Modified: Wed, 10 Aug 2022 23:49:39 GMT  
		Size: 12.1 MB (12088976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89a4ce283e3c239c3a421efffe3ec29de680be8ad1344186df9cd8543ddb21e`  
		Last Modified: Wed, 10 Aug 2022 23:49:37 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afa7d7c582c85caa2f233f149c72bdddd1ec1be07bc5b1fc8f004d08ef5915f`  
		Last Modified: Fri, 12 Aug 2022 06:58:40 GMT  
		Size: 3.0 MB (3043706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d092d8d4bb63c7395e338e6eb72d1ab504e143d97679f6772cf7e38bbdba9c`  
		Last Modified: Fri, 12 Aug 2022 07:30:00 GMT  
		Size: 8.3 MB (8298757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f1d53bc30116bdce6ab24d34f94c4c387d4d97012a1e803a16de16c6119405`  
		Last Modified: Fri, 12 Aug 2022 07:30:11 GMT  
		Size: 148.1 MB (148118344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd00634600b354a1ef2917ca8aac6b4f26638631b4e72ed22636489fa4fdfebd`  
		Last Modified: Fri, 12 Aug 2022 07:29:58 GMT  
		Size: 9.4 KB (9438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7341492a6f2ed802f9a79c79bcfe434f1726c7bef47625414fd2e3cc830c4e`  
		Last Modified: Fri, 12 Aug 2022 07:29:58 GMT  
		Size: 2.1 KB (2117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:alpine` - linux; arm variant v7

```console
$ docker pull satosa@sha256:bfd55d2910e033f95af6225f96e8140a525fd2d0f20ac508439c2b701c17fbc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174270319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38d79d322799cd764de19cac9a0f304ed531faefaf0ae82508a31cdc18feb302`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 20:41:20 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 20:41:20 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 20:41:21 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 10 Aug 2022 20:41:22 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 10 Aug 2022 21:41:34 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 22:01:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 10 Aug 2022 22:01:14 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 10 Aug 2022 22:01:14 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 22:01:14 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Fri, 12 Aug 2022 06:54:29 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Fri, 12 Aug 2022 06:54:29 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Fri, 12 Aug 2022 06:54:35 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Fri, 12 Aug 2022 06:54:35 GMT
CMD ["python3"]
# Fri, 12 Aug 2022 11:08:34 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Fri, 12 Aug 2022 11:08:34 GMT
ENV SATOSA_VERSION=8.1.1
# Fri, 12 Aug 2022 11:11:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Fri, 12 Aug 2022 11:12:01 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Fri, 12 Aug 2022 11:12:01 GMT
WORKDIR /etc/satosa
# Fri, 12 Aug 2022 11:12:01 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Fri, 12 Aug 2022 11:12:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Aug 2022 11:12:01 GMT
EXPOSE 8080
# Fri, 12 Aug 2022 11:12:02 GMT
USER satosa:satosa
# Fri, 12 Aug 2022 11:12:02 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe115a90a2a7540a0fafad5c9fdaed18869ade3f7bbf6a98bcecb8aba0bcf10c`  
		Last Modified: Thu, 11 Aug 2022 02:12:05 GMT  
		Size: 678.8 KB (678781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7011ad146248f14eb2602d052f76af68d0f1ebf4a70ff4ff53eead2a9a82a967`  
		Last Modified: Thu, 11 Aug 2022 02:13:02 GMT  
		Size: 11.6 MB (11558685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cdde388dddcfd9fc1725f96aa287533651bb011d0fe2b6b03a8cb5c27c20894`  
		Last Modified: Thu, 11 Aug 2022 02:12:59 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbe2eb7a6e500fd4864106e7e0cf0b8f3490a2a4858eec337b6883625f47841`  
		Last Modified: Fri, 12 Aug 2022 10:06:21 GMT  
		Size: 3.0 MB (3043667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10547872027cb10330b8ab2ea08038af4dcc6aadcf4f88a7b3ca2ddf57753603`  
		Last Modified: Fri, 12 Aug 2022 11:13:31 GMT  
		Size: 8.0 MB (8046186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:520f1b9716045701ca9caeed18342a0b877f6736c5d4152a79c7cafc3a4c2d5a`  
		Last Modified: Fri, 12 Aug 2022 11:13:44 GMT  
		Size: 148.5 MB (148514147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1055809568182d4edaab588e6109a8ba69790cf4ef25848507c19738d245adb`  
		Last Modified: Fri, 12 Aug 2022 11:13:30 GMT  
		Size: 9.4 KB (9441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabf72c80e9ac82642b443c9378b5913b06f8f04ae845817fe307415e6c5f034`  
		Last Modified: Fri, 12 Aug 2022 11:13:30 GMT  
		Size: 2.1 KB (2116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:alpine` - linux; arm64 variant v8

```console
$ docker pull satosa@sha256:a0be29adc3a06da8251b6727e04990d55f8e3991203117c1a16f5980b6e8c921
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40936174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:643fe5384220d5a780fa080b25e79ebfa51351a96dfb1c3ca67e54b228a33454`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:29:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 02:53:17 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 02:53:19 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Wed, 10 Aug 2022 02:53:19 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 07 Sep 2022 22:22:38 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 07 Sep 2022 22:37:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 07 Sep 2022 22:37:03 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 07 Sep 2022 22:37:04 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 07 Sep 2022 22:37:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 07 Sep 2022 22:37:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 07 Sep 2022 22:37:07 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 07 Sep 2022 22:37:14 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 07 Sep 2022 22:37:15 GMT
CMD ["python3"]
# Thu, 08 Sep 2022 01:12:37 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Thu, 08 Sep 2022 01:12:37 GMT
ENV SATOSA_VERSION=8.1.1
# Thu, 08 Sep 2022 01:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 08 Sep 2022 01:13:28 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 08 Sep 2022 01:13:29 GMT
WORKDIR /etc/satosa
# Thu, 08 Sep 2022 01:13:31 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Thu, 08 Sep 2022 01:13:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Sep 2022 01:13:32 GMT
EXPOSE 8080
# Thu, 08 Sep 2022 01:13:33 GMT
USER satosa:satosa
# Thu, 08 Sep 2022 01:13:34 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588f86efd8c29ba77a66b93122eebbf205c99abcbe092432668d8c347cc3ce5e`  
		Last Modified: Wed, 10 Aug 2022 04:54:39 GMT  
		Size: 682.3 KB (682301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f7f1e58a1b6b1ddbac7d24d4e06f4af6d498a4a6adf6483361d68df30f7a0e`  
		Last Modified: Thu, 08 Sep 2022 00:43:14 GMT  
		Size: 12.6 MB (12581186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5cdcf80b8d9caa9e43bddac5228183b2b799cbf3b4bb534e16e07367ed10909`  
		Last Modified: Thu, 08 Sep 2022 00:43:12 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ebb02bb86701dda49e423b63b25139bb02c3788fce98e2765713428d47acb4`  
		Last Modified: Thu, 08 Sep 2022 00:43:13 GMT  
		Size: 3.0 MB (3044954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7539265a1f0cf30bda8228d2ece3b2b5cd001a9281d6604026c969672839c8`  
		Last Modified: Thu, 08 Sep 2022 01:14:31 GMT  
		Size: 8.2 MB (8235499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5326724d88d55b81cb6766b55ce523e0415a72f3e3a28983e74741cbcc1323`  
		Last Modified: Thu, 08 Sep 2022 01:14:32 GMT  
		Size: 13.7 MB (13672827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4ac55ea1e71e73c5d9839d1f67d29456ca6deba44d0daa4f9ffa31f3ef5eab`  
		Last Modified: Thu, 08 Sep 2022 01:14:30 GMT  
		Size: 9.4 KB (9395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7532f6a3432b5d098d61ecfb4a2cb77ec91de5aede6eff50eb4609afeeb7f2ca`  
		Last Modified: Thu, 08 Sep 2022 01:14:30 GMT  
		Size: 2.1 KB (2119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:alpine` - linux; 386

```console
$ docker pull satosa@sha256:425fbac782432a82b41fb4c1c72b3f7e8c165041b37a2e5fd99b34ff6ef87d05
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135151127 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05118ee5a941eff949bbf5a85df05724d282541e12e54dd35cbf97da01b29af0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 21:22:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 21:22:15 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 21:22:17 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 09 Aug 2022 21:22:18 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 07 Sep 2022 22:10:38 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 07 Sep 2022 22:24:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 07 Sep 2022 22:24:02 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 07 Sep 2022 22:24:03 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 07 Sep 2022 22:24:04 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 07 Sep 2022 22:24:05 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 07 Sep 2022 22:24:06 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 07 Sep 2022 22:24:13 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 07 Sep 2022 22:24:14 GMT
CMD ["python3"]
# Thu, 08 Sep 2022 01:12:59 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Thu, 08 Sep 2022 01:13:00 GMT
ENV SATOSA_VERSION=8.1.1
# Thu, 08 Sep 2022 01:16:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 08 Sep 2022 01:16:03 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 08 Sep 2022 01:16:03 GMT
WORKDIR /etc/satosa
# Thu, 08 Sep 2022 01:16:05 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Thu, 08 Sep 2022 01:16:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Sep 2022 01:16:06 GMT
EXPOSE 8080
# Thu, 08 Sep 2022 01:16:07 GMT
USER satosa:satosa
# Thu, 08 Sep 2022 01:16:08 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb6e4c463b4b085b81ccd90e5d99d5d5b64a56c2f756e7ff5575080b0efc2e9f`  
		Last Modified: Tue, 09 Aug 2022 23:12:22 GMT  
		Size: 689.1 KB (689070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8169fab3362e74d5b1a4e767ac98947cb0ff7032606deb9b19b620e7779eeb5`  
		Last Modified: Thu, 08 Sep 2022 00:48:19 GMT  
		Size: 12.7 MB (12702334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bab460be51ec9763271585731ee28b4130152b8a4b87feae0131b30e87837e`  
		Last Modified: Thu, 08 Sep 2022 00:48:18 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa1ce5fa628e8be153581c61a1821b9742b420d5a7aed832909304189243845`  
		Last Modified: Thu, 08 Sep 2022 00:48:18 GMT  
		Size: 3.0 MB (3044941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ec2f6cc70e48214891a074d4553fdf8a0a0c26b884ae3dc2e51802ee3060d6`  
		Last Modified: Thu, 08 Sep 2022 01:17:19 GMT  
		Size: 8.5 MB (8513789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2c0e949087e34003c36748c1e5461913ae64b5152e0d5d94d08f7e8f75244b`  
		Last Modified: Thu, 08 Sep 2022 01:17:27 GMT  
		Size: 107.4 MB (107382135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d834e3da22f6ffc3794d76093a6dde905f98dca1b50600ff6fbb3a5a92949a8b`  
		Last Modified: Thu, 08 Sep 2022 01:17:18 GMT  
		Size: 9.4 KB (9392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d84d92951ed5f09fdeef21ffc452e1c8ed8991d13cbcec8d8480594b0241eac`  
		Last Modified: Thu, 08 Sep 2022 01:17:18 GMT  
		Size: 2.1 KB (2114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:alpine` - linux; ppc64le

```console
$ docker pull satosa@sha256:781eace0cbb5b456f9169233b1ffeb9aacb70cde105d2639c7ede9baa9ca748a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135488886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1a3e508c0cc53f767c1f1d8e480e18153c4d05ae2056a712b2f42c2aa5552e7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 22:44:31 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 22:44:31 GMT
ENV LANG=C.UTF-8
# Tue, 09 Aug 2022 22:44:34 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Tue, 09 Aug 2022 22:44:35 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Wed, 07 Sep 2022 22:48:03 GMT
ENV PYTHON_VERSION=3.10.7
# Wed, 07 Sep 2022 23:12:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	make -j "$nproc" 		EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000" 		LDFLAGS="-Wl,--strip-all" 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Wed, 07 Sep 2022 23:12:47 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Wed, 07 Sep 2022 23:12:47 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Wed, 07 Sep 2022 23:12:47 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 07 Sep 2022 23:12:48 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Wed, 07 Sep 2022 23:12:48 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Wed, 07 Sep 2022 23:12:59 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Wed, 07 Sep 2022 23:12:59 GMT
CMD ["python3"]
# Thu, 08 Sep 2022 03:15:33 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Thu, 08 Sep 2022 03:15:33 GMT
ENV SATOSA_VERSION=8.1.1
# Thu, 08 Sep 2022 03:21:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 08 Sep 2022 03:21:52 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 08 Sep 2022 03:21:52 GMT
WORKDIR /etc/satosa
# Thu, 08 Sep 2022 03:21:53 GMT
COPY file:052229d57447119afa18a76253b740426943fcd4cf1c553c23df3445a5ed9f32 in /usr/local/bin/ 
# Thu, 08 Sep 2022 03:21:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 08 Sep 2022 03:21:53 GMT
EXPOSE 8080
# Thu, 08 Sep 2022 03:21:54 GMT
USER satosa:satosa
# Thu, 08 Sep 2022 03:21:54 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97ea732185528f2d8be38ac21b7ddadc64d37137d97d34702609b1d5b011320`  
		Last Modified: Wed, 10 Aug 2022 02:04:25 GMT  
		Size: 690.0 KB (690020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f418aa7f35fdf447c371fc8a39b9398027cf9522bcf9914884be0b5b965fd1cf`  
		Last Modified: Thu, 08 Sep 2022 02:30:04 GMT  
		Size: 12.8 MB (12822639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3b7b9476db34b4aaaeaed9e6a5fe7aed618a91d24e11eec7565654929a2fc55`  
		Last Modified: Thu, 08 Sep 2022 02:30:00 GMT  
		Size: 230.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7095e0016be658ea48f7bb26d0fd2b0967e9705367d26635a41c7992b88cc7`  
		Last Modified: Thu, 08 Sep 2022 02:30:01 GMT  
		Size: 3.0 MB (3043771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c280874e3ffdcb5093cb607fe93ae962cac5731e653bc848520345d13d0d77`  
		Last Modified: Thu, 08 Sep 2022 03:22:27 GMT  
		Size: 8.5 MB (8484320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f6ba4c741684c5c262fcffadee333d5b120b4ba7b2a1d912a7a85b999e7724`  
		Last Modified: Thu, 08 Sep 2022 03:22:41 GMT  
		Size: 107.6 MB (107633031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb332abe7880d9121ddc124c87c0b6105a7d7d24a91303df00ce02b34de6e690`  
		Last Modified: Thu, 08 Sep 2022 03:22:25 GMT  
		Size: 9.4 KB (9440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a38e97a1050d363e171af65079d4c062915ed396a4ef2bc7d0cde846adbbfdbb`  
		Last Modified: Thu, 08 Sep 2022 03:22:25 GMT  
		Size: 2.1 KB (2115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
