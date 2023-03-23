## `satosa:8-alpine3.16`

```console
$ docker pull satosa@sha256:520e126e5a19a25b0a366181ad240c68150697efdc8a4c2576be667c78f39fd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `satosa:8-alpine3.16` - linux; amd64

```console
$ docker pull satosa@sha256:9f25b84bbcd65b7fea67c9ece51c88c189716538f946538b55b2645c9956408d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49334860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1013db5a878b573a71a62daf2fd38ac4c44fb7d91e1798fcd96b8a2f600763cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Mar 2023 23:32:52 GMT
ENV LANG=C.UTF-8
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_VERSION=3.11.2
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
CMD ["python3"]
# Thu, 23 Mar 2023 18:21:45 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Thu, 23 Mar 2023 18:21:46 GMT
ENV SATOSA_VERSION=8.2.0
# Thu, 23 Mar 2023 18:22:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 23 Mar 2023 18:22:07 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 23 Mar 2023 18:22:07 GMT
WORKDIR /etc/satosa
# Thu, 23 Mar 2023 18:22:07 GMT
COPY file:c55013587aaf85deb9d4e88a802c99946f6d607afbf641c34429da762c1aa229 in /usr/local/bin/ 
# Thu, 23 Mar 2023 18:22:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 18:22:07 GMT
EXPOSE 8080
# Thu, 23 Mar 2023 18:22:07 GMT
USER satosa:satosa
# Thu, 23 Mar 2023 18:22:07 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bb9323a0669ce046fe6ad4ddd3772bd5f8d821917c9b4675e4119b2bfe8471d`  
		Last Modified: Thu, 23 Mar 2023 05:41:45 GMT  
		Size: 661.9 KB (661885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a51756f6aa307bd5f248c569455c50e13450ed8e87bbbe20f45bda47bcf02f`  
		Last Modified: Thu, 23 Mar 2023 05:43:21 GMT  
		Size: 14.2 MB (14152219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54e3c97cd1aeebec90226e87d54421abda6e3816238b9d3d6ff0277bb4a2925`  
		Last Modified: Thu, 23 Mar 2023 05:43:19 GMT  
		Size: 241.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d682b335145d050eb77aef645c4c81ffdcf2aade7262f398440779b6d6342e0`  
		Last Modified: Thu, 23 Mar 2023 05:43:19 GMT  
		Size: 3.1 MB (3080518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1272ab83a159eb46a62f009793423405563e58d7e6a4a5e35568a178213d2fde`  
		Last Modified: Thu, 23 Mar 2023 18:22:39 GMT  
		Size: 10.8 MB (10823178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7d2c02654f50a94c2e398d78e241e36bb37f3cbb0fe21199bcbeb8c9bfa855`  
		Last Modified: Thu, 23 Mar 2023 18:22:41 GMT  
		Size: 17.8 MB (17797425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd06a6d589ace8def9bf323c98b323abca08bdd2c34b8a9e72e20c3d2b42d2be`  
		Last Modified: Thu, 23 Mar 2023 18:22:38 GMT  
		Size: 9.5 KB (9485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3238580d6e02e4e3d97652ae62c607e1037fd39583083220a91a433e24cc8ccc`  
		Last Modified: Thu, 23 Mar 2023 18:22:38 GMT  
		Size: 2.1 KB (2147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:8-alpine3.16` - linux; arm variant v6

```console
$ docker pull satosa@sha256:90f4fa55454483b820ca00c217d28b3d9dd796542e3cfb53c70449cfa4ee210d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295365399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ba343d3856a2756e3b0c476eefc68a7e3bf45b7b442a6f3e2f4c48dfb27c025`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:12:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Mar 2023 23:12:30 GMT
ENV LANG=C.UTF-8
# Mon, 13 Mar 2023 23:12:32 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Mon, 13 Mar 2023 23:47:05 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Mon, 13 Mar 2023 23:47:06 GMT
ENV PYTHON_VERSION=3.11.2
# Tue, 14 Mar 2023 05:11:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 14 Mar 2023 05:11:15 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 14 Mar 2023 05:11:16 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Tue, 14 Mar 2023 05:11:16 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Tue, 14 Mar 2023 05:11:16 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Tue, 14 Mar 2023 05:11:16 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Tue, 14 Mar 2023 05:11:22 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 14 Mar 2023 05:11:22 GMT
CMD ["python3"]
# Tue, 14 Mar 2023 06:20:49 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Tue, 14 Mar 2023 06:20:49 GMT
ENV SATOSA_VERSION=8.2.0
# Tue, 14 Mar 2023 06:25:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Tue, 14 Mar 2023 06:25:09 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Tue, 14 Mar 2023 06:25:10 GMT
WORKDIR /etc/satosa
# Tue, 14 Mar 2023 06:25:10 GMT
COPY file:c55013587aaf85deb9d4e88a802c99946f6d607afbf641c34429da762c1aa229 in /usr/local/bin/ 
# Tue, 14 Mar 2023 06:25:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 06:25:10 GMT
EXPOSE 8080
# Tue, 14 Mar 2023 06:25:10 GMT
USER satosa:satosa
# Tue, 14 Mar 2023 06:25:10 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1309a5f014ba861663c27c1590c426da913481a144ed22dcf128aa0c9324d6`  
		Last Modified: Tue, 14 Mar 2023 00:55:22 GMT  
		Size: 666.4 KB (666377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26eff4cadf164931af413ea8c9c4085b0b6470c0dbbc3b524fa3357dff193520`  
		Last Modified: Tue, 14 Mar 2023 06:03:20 GMT  
		Size: 12.2 MB (12210028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d2566f9a8f76844a85c8d4df34cf3c9a2a82eef9f2c94916617f88f886e82d`  
		Last Modified: Tue, 14 Mar 2023 06:03:18 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76caede435b6e083a7c41b0a72d647a04818359ece119596a626103f30eb3e0b`  
		Last Modified: Tue, 14 Mar 2023 06:03:19 GMT  
		Size: 3.1 MB (3056425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fbae4fd59523f437eb43e422e5a1cced39763ef93c91018f0fccf898eb32994`  
		Last Modified: Tue, 14 Mar 2023 06:25:43 GMT  
		Size: 9.7 MB (9675750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc1267a2f39eeb0b6285a942ae0e1d5f5292ceee3488b3e3e045df1af33139a`  
		Last Modified: Tue, 14 Mar 2023 06:26:00 GMT  
		Size: 267.1 MB (267128179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccab47584555cebaaf624b1170d8a7b775b7573edca83675e5ba855498554d7a`  
		Last Modified: Tue, 14 Mar 2023 06:25:42 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0948c0d887765e95ba32d30f1b65f17433f18290ec0fdfb377c53bacd4c48f24`  
		Last Modified: Tue, 14 Mar 2023 06:25:42 GMT  
		Size: 2.1 KB (2146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:8-alpine3.16` - linux; arm variant v7

```console
$ docker pull satosa@sha256:abae7a3722747829fd3deedb0d78e37a453334e41313ef0614dab3179c03ffbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.1 MB (328077844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:205ade9bc170bcaaecb97deda8ea88c688605bcd7b7ce21edf7cda534b6a2212`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Mar 2023 23:32:52 GMT
ENV LANG=C.UTF-8
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_VERSION=3.11.2
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
CMD ["python3"]
# Thu, 23 Mar 2023 17:09:01 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Thu, 23 Mar 2023 17:09:01 GMT
ENV SATOSA_VERSION=8.2.0
# Thu, 23 Mar 2023 17:13:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 23 Mar 2023 17:13:55 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 23 Mar 2023 17:13:55 GMT
WORKDIR /etc/satosa
# Thu, 23 Mar 2023 17:13:55 GMT
COPY file:c55013587aaf85deb9d4e88a802c99946f6d607afbf641c34429da762c1aa229 in /usr/local/bin/ 
# Thu, 23 Mar 2023 17:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 17:13:55 GMT
EXPOSE 8080
# Thu, 23 Mar 2023 17:13:55 GMT
USER satosa:satosa
# Thu, 23 Mar 2023 17:13:55 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf86d08852a3e565994878ac9306830d0714852669ad6c0bb7200c2c2a0ec45`  
		Last Modified: Thu, 23 Mar 2023 07:41:28 GMT  
		Size: 659.4 KB (659391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6a47dc41f424d0fc274967ea20e6644d5de89b52df8b10fa09de7d5e631577`  
		Last Modified: Thu, 23 Mar 2023 07:41:30 GMT  
		Size: 13.0 MB (12993370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698b1d91907190c1a4eabed84d81b3fbe73489a406355f6f88f852263c184748`  
		Last Modified: Thu, 23 Mar 2023 07:41:28 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfe0506d3d3dd2e1d5e780b886dd8de153d8aa744a95876f07ed6291fa171a3c`  
		Last Modified: Thu, 23 Mar 2023 07:41:29 GMT  
		Size: 3.1 MB (3080434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd56ae1f390fa1f2283f32a4107574c089507713546ecdfa4f2a3de7a70b80f9`  
		Last Modified: Thu, 23 Mar 2023 17:14:45 GMT  
		Size: 9.5 MB (9453115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2939a4c66b68b7ed10b1b7d44f88f0d38ff7d93b389b858417eb2a7cba3173`  
		Last Modified: Thu, 23 Mar 2023 17:15:03 GMT  
		Size: 299.5 MB (299459160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d677f6e94edbe16d881e38a8fa4076dcefc746903da1723d14c7ea4ebf97112`  
		Last Modified: Thu, 23 Mar 2023 17:14:43 GMT  
		Size: 9.5 KB (9488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869de228ea40f97573d7a9bef6f089d2032b43718c85576c01fa3d20c9f04072`  
		Last Modified: Thu, 23 Mar 2023 17:14:43 GMT  
		Size: 2.1 KB (2150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:8-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull satosa@sha256:b885d423f682115102e9bb63185536dcf95b6747460445d9815599a78185476f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47791924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c03c3e107c7fe588396731b73125e786883df0aa181ab0ac21d117747ce750`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Mar 2023 23:32:52 GMT
ENV LANG=C.UTF-8
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_VERSION=3.11.2
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
CMD ["python3"]
# Thu, 23 Mar 2023 14:57:24 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Thu, 23 Mar 2023 14:57:24 GMT
ENV SATOSA_VERSION=8.2.0
# Thu, 23 Mar 2023 14:57:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 23 Mar 2023 14:57:46 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 23 Mar 2023 14:57:46 GMT
WORKDIR /etc/satosa
# Thu, 23 Mar 2023 14:57:46 GMT
COPY file:c55013587aaf85deb9d4e88a802c99946f6d607afbf641c34429da762c1aa229 in /usr/local/bin/ 
# Thu, 23 Mar 2023 14:57:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 14:57:46 GMT
EXPOSE 8080
# Thu, 23 Mar 2023 14:57:47 GMT
USER satosa:satosa
# Thu, 23 Mar 2023 14:57:47 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196915721f2b44a093ffa9a18a68ced28fa3722310f70a56b21656b610638699`  
		Last Modified: Thu, 23 Mar 2023 05:32:14 GMT  
		Size: 663.1 KB (663147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837b8d7adaebbcf6ffc67d71e03a40fa9623a96335ff852de27aaeabc231d38c`  
		Last Modified: Thu, 23 Mar 2023 05:33:46 GMT  
		Size: 14.1 MB (14140039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034f5b8034ab619e77e56501348059a0e007729d74cea8b6d774883751b9a59b`  
		Last Modified: Thu, 23 Mar 2023 05:33:44 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f098a84d97130fd24e64686ab8eb51fc9d593249e60c50ca3ed5c4a496274`  
		Last Modified: Thu, 23 Mar 2023 05:33:44 GMT  
		Size: 3.1 MB (3080435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3d625ffc6c6b75ad370303ea328b1f1f8bd52b9ecb97ecfcc18022152231dc`  
		Last Modified: Thu, 23 Mar 2023 14:58:14 GMT  
		Size: 9.7 MB (9655921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b54e5d549851dad81d3bf9546f0d70c6a2d26bbd6d49f0b8a13ce98c39507c6`  
		Last Modified: Thu, 23 Mar 2023 14:58:16 GMT  
		Size: 17.5 MB (17531010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837de5564d7802a99623f7af3ccfd472580b1a847d94a31e6bf1237cc15a5493`  
		Last Modified: Thu, 23 Mar 2023 14:58:13 GMT  
		Size: 9.5 KB (9485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776d649befe72830d81f1d75cbcb86e2736cd7de7546f91802df488942c5be06`  
		Last Modified: Thu, 23 Mar 2023 14:58:13 GMT  
		Size: 2.1 KB (2145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:8-alpine3.16` - linux; 386

```console
$ docker pull satosa@sha256:5ea888a6b99e0afe108f6191ca1a8cc4c3b0fac6f9e00d98f23474dbf642132a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **296.2 MB (296199567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce227a6dffdf2d93fff2c67fc561c35f24f6df55f65433bb010cf178b6397a41`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:29 GMT
ADD file:59ac1f8f33f9b9727892b7e45b33f54ef3c20d9d876c49d6a4c057641821d68f in / 
# Fri, 10 Feb 2023 21:24:29 GMT
CMD ["/bin/sh"]
# Sat, 25 Feb 2023 01:14:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 25 Feb 2023 01:14:58 GMT
ENV LANG=C.UTF-8
# Sat, 25 Feb 2023 01:15:00 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	;
# Sat, 25 Feb 2023 03:10:56 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Sat, 25 Feb 2023 03:10:56 GMT
ENV PYTHON_VERSION=3.11.2
# Tue, 14 Mar 2023 04:34:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version
# Tue, 14 Mar 2023 04:34:07 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done
# Tue, 14 Mar 2023 04:34:07 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Tue, 14 Mar 2023 04:34:07 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Tue, 14 Mar 2023 04:34:07 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Tue, 14 Mar 2023 04:34:07 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Tue, 14 Mar 2023 04:34:14 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version
# Tue, 14 Mar 2023 04:34:14 GMT
CMD ["python3"]
# Tue, 14 Mar 2023 08:12:46 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Tue, 14 Mar 2023 08:12:46 GMT
ENV SATOSA_VERSION=8.2.0
# Tue, 14 Mar 2023 08:16:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Tue, 14 Mar 2023 08:16:59 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Tue, 14 Mar 2023 08:16:59 GMT
WORKDIR /etc/satosa
# Tue, 14 Mar 2023 08:16:59 GMT
COPY file:c55013587aaf85deb9d4e88a802c99946f6d607afbf641c34429da762c1aa229 in /usr/local/bin/ 
# Tue, 14 Mar 2023 08:17:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Mar 2023 08:17:00 GMT
EXPOSE 8080
# Tue, 14 Mar 2023 08:17:00 GMT
USER satosa:satosa
# Tue, 14 Mar 2023 08:17:00 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:0987f51cd58a7d03bc7d6ff0a3a0a843c1a3fefcd41e3c8adc3999ddde7441e8`  
		Last Modified: Fri, 10 Feb 2023 21:25:30 GMT  
		Size: 2.8 MB (2810653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b46b4ed1a9500772676da09f03658a766a985faeb849b4cfb302b802a11d3c`  
		Last Modified: Sat, 25 Feb 2023 06:42:31 GMT  
		Size: 669.9 KB (669885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62351b7993f319f737ff62d2d4f97ffc62f6099eea00a5ac68d1eb418481801b`  
		Last Modified: Tue, 14 Mar 2023 07:45:22 GMT  
		Size: 12.7 MB (12727969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7edd623d5792978cd82804a82294b8ef9a0ac1d38ab2c817adb64d6fb5190ede`  
		Last Modified: Tue, 14 Mar 2023 07:45:19 GMT  
		Size: 231.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e8e5a1bdb962fa81706a8395d1ab22306e2e223fec788ecf7fd18a89174fe0`  
		Last Modified: Tue, 14 Mar 2023 07:45:20 GMT  
		Size: 3.1 MB (3056467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2144f8a9560b7d00985dbcb7d0edd6466f465439263dede01930aa57502dc795`  
		Last Modified: Tue, 14 Mar 2023 08:18:32 GMT  
		Size: 9.9 MB (9907728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe219d8706fb6ce0b5f51c726b68ca41c942b2acef06cd7269033dec2f28d94`  
		Last Modified: Tue, 14 Mar 2023 08:18:54 GMT  
		Size: 267.0 MB (267015000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da2ef48e0995b6f55cf17c8ef44505ac109dedad3069c25dec6e6720aba496`  
		Last Modified: Tue, 14 Mar 2023 08:18:30 GMT  
		Size: 9.5 KB (9486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba31014edcebc12467d82f590b66fe3fda5b8890995a758601b8f17d46e0e0`  
		Last Modified: Tue, 14 Mar 2023 08:18:30 GMT  
		Size: 2.1 KB (2148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `satosa:8-alpine3.16` - linux; ppc64le

```console
$ docker pull satosa@sha256:a4d24d59ade30b13b71fc4218c2c1d3bf8eaa3949543bd5d5fc1d1acdc302f29
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330781333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111e83f7fe72071fd4d0d584f5392a4647abb8f6bf0f41aa549cca7d24c72e86`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["gunicorn","-b0.0.0.0:8080","satosa.wsgi:app"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Mar 2023 23:32:52 GMT
ENV LANG=C.UTF-8
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 	apk add --no-cache 		ca-certificates 		tzdata 	; # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
ENV GPG_KEY=A035C8C19219BA821ECEA86B64E628F8D684696D
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_VERSION=3.11.2
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		gnupg 		tar 		xz 				bluez-dev 		bzip2-dev 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		ncurses-dev 		openssl-dev 		pax-utils 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 		wget -O python.tar.xz "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz"; 	wget -O python.tar.xz.asc "https://www.python.org/ftp/python/${PYTHON_VERSION%%[a-z]*}/Python-$PYTHON_VERSION.tar.xz.asc"; 	GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPG_KEY"; 	gpg --batch --verify python.tar.xz.asc python.tar.xz; 	command -v gpgconf > /dev/null && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" python.tar.xz.asc; 	mkdir -p /usr/src/python; 	tar --extract --directory /usr/src/python --strip-components=1 --file python.tar.xz; 	rm python.tar.xz; 		cd /usr/src/python; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-loadable-sqlite-extensions 		--enable-optimizations 		--enable-option-checking=fatal 		--enable-shared 		--with-lto 		--with-system-expat 		--without-ensurepip 	; 	nproc="$(nproc)"; 	EXTRA_CFLAGS="-DTHREAD_STACK_SIZE=0x100000"; 	LDFLAGS="${LDFLAGS:--Wl},--strip-all"; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:-}" 		"PROFILE_TASK=${PROFILE_TASK:-}" 	; 	rm python; 	make -j "$nproc" 		"EXTRA_CFLAGS=${EXTRA_CFLAGS:-}" 		"LDFLAGS=${LDFLAGS:--Wl},-rpath='\$\$ORIGIN/../lib'" 		"PROFILE_TASK=${PROFILE_TASK:-}" 		python 	; 	make install; 		cd /; 	rm -rf /usr/src/python; 		find /usr/local -depth 		\( 			\( -type d -a \( -name test -o -name tests -o -name idle_test \) \) 			-o \( -type f -a \( -name '*.pyc' -o -name '*.pyo' -o -name 'libpython*.a' \) \) 		\) -exec rm -rf '{}' + 	; 		find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| xargs -rt apk add --no-network --virtual .python-rundeps 	; 	apk del --no-network .build-deps; 		python3 --version # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 	for src in idle3 pydoc3 python3 python3-config; do 		dst="$(echo "$src" | tr -d 3)"; 		[ -s "/usr/local/bin/$src" ]; 		[ ! -e "/usr/local/bin/$dst" ]; 		ln -svT "$src" "/usr/local/bin/$dst"; 	done # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_PIP_VERSION=22.3.1
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d5cb0afaf23b8520f1bbcfed521017b4a95f5c01/public/get-pip.py
# Fri, 10 Mar 2023 23:32:52 GMT
ENV PYTHON_GET_PIP_SHA256=394be00f13fa1b9aaa47e911bdb59a09c3b2986472130f30aa0bfaf7f3980637
# Fri, 10 Mar 2023 23:32:52 GMT
RUN set -eux; 		wget -O get-pip.py "$PYTHON_GET_PIP_URL"; 	echo "$PYTHON_GET_PIP_SHA256 *get-pip.py" | sha256sum -c -; 		export PYTHONDONTWRITEBYTECODE=1; 		python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		"pip==$PYTHON_PIP_VERSION" 		"setuptools==$PYTHON_SETUPTOOLS_VERSION" 	; 	rm -f get-pip.py; 		pip --version # buildkit
# Fri, 10 Mar 2023 23:32:52 GMT
CMD ["python3"]
# Thu, 23 Mar 2023 18:24:23 GMT
RUN set -eux; 	addgroup --gid 1000 satosa; 	adduser -D -G satosa --uid 1000 satosa; 	apk add --no-cache 		bash 		jq 		libxml2-utils 		openssl 		xmlsec 	; 	pip install --no-cache-dir 		yq 	;
# Thu, 23 Mar 2023 18:24:23 GMT
ENV SATOSA_VERSION=8.2.0
# Thu, 23 Mar 2023 18:33:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bluez-dev 		bzip2-dev 		cargo 		coreutils 		dpkg-dev dpkg 		expat-dev 		findutils 		gcc 		gdbm-dev 		libc-dev 		libffi-dev 		libnsl-dev 		libtirpc-dev 		linux-headers 		make 		musl-dev 		ncurses-dev 		openssl-dev 		pax-utils 		python3-dev 		readline-dev 		sqlite-dev 		tcl-dev 		tk 		tk-dev 		util-linux-dev 		xz-dev 		zlib-dev 	; 	pip install --no-cache-dir 		satosa==${SATOSA_VERSION} 	; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec scanelf --needed --nobanner --format '%n#p' '{}' ';' 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		| fgrep -v libgcc_s- 		| xargs -rt apk add --no-network --virtual .satosa-rundeps 	; 	apk del --no-network .build-deps; 	mkdir /etc/satosa; 	chown -R satosa:satosa /etc/satosa
# Thu, 23 Mar 2023 18:33:22 GMT
RUN set -eux; 	python -c 'import urllib.request; urllib.request.urlretrieve("https://github.com/IdentityPython/SATOSA/archive/refs/tags/v'${SATOSA_VERSION%%[a-z]*}'.tar.gz","/tmp/satosa.tgz")'; 	mkdir /usr/share/satosa; 	tar --extract --directory /usr/share/satosa --strip-components=1 --file /tmp/satosa.tgz SATOSA-${SATOSA_VERSION%%[a-z]*}/example/; 	rm /tmp/satosa.tgz
# Thu, 23 Mar 2023 18:33:22 GMT
WORKDIR /etc/satosa
# Thu, 23 Mar 2023 18:33:23 GMT
COPY file:c55013587aaf85deb9d4e88a802c99946f6d607afbf641c34429da762c1aa229 in /usr/local/bin/ 
# Thu, 23 Mar 2023 18:33:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Mar 2023 18:33:23 GMT
EXPOSE 8080
# Thu, 23 Mar 2023 18:33:23 GMT
USER satosa:satosa
# Thu, 23 Mar 2023 18:33:24 GMT
CMD ["gunicorn" "-b0.0.0.0:8080" "satosa.wsgi:app"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b1a617981acad40662d103ba8dfda4223a7b01e9605c9b56a0a47da78d0cf9`  
		Last Modified: Thu, 23 Mar 2023 09:16:29 GMT  
		Size: 670.3 KB (670328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b6d03cbe00fb3183c1c57952e9044f7de776a5f12c2981038ef687c89e33ea`  
		Last Modified: Thu, 23 Mar 2023 09:17:50 GMT  
		Size: 14.4 MB (14385051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f9f9367c2836f6cb19c8157f5f64832c1acc381da5d284154f52f074b0502e`  
		Last Modified: Thu, 23 Mar 2023 09:17:46 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccdf99f4021e7150bf86c23b4742711d0210f967b53567005918fbdbba9c573`  
		Last Modified: Thu, 23 Mar 2023 09:17:48 GMT  
		Size: 3.1 MB (3080477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867ed621119e962b454d105802ded815d8fbd6ee0fdcd214d538f87e2d60eda0`  
		Last Modified: Thu, 23 Mar 2023 18:34:29 GMT  
		Size: 9.9 MB (9901942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13920edf07dc36aaede20058a91f5362adf0237fba7a9ff3d3c870c40e290f6`  
		Last Modified: Thu, 23 Mar 2023 18:34:55 GMT  
		Size: 299.9 MB (299927029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c594b9fdbe78fee879ccaa8edd8fa863ab5de505e208f63f91392f601ed3d47a`  
		Last Modified: Thu, 23 Mar 2023 18:34:26 GMT  
		Size: 9.5 KB (9487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43d2c4296b1b296c0952e252e33d0c8ecfe769b96f5f19b093b8d5878669bb1`  
		Last Modified: Thu, 23 Mar 2023 18:34:26 GMT  
		Size: 2.1 KB (2147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
