## `ruby:buster`

```console
$ docker pull ruby@sha256:004c8eeca0d18a25c38f2fc173eaf94ceaba43609ffef2b041c94044e5e0d15d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `ruby:buster` - linux; amd64

```console
$ docker pull ruby@sha256:1f5dcae23539e683c77869156ea8cc09a0a8055e81f30414dd72fec6b40aa1e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.8 MB (344763843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409aa635c90f26819525650277aceb97cb982eb432a3d607ff760cb8bea375e5`
-	Default Command: `["irb"]`

```dockerfile
# Sat, 28 May 2022 01:20:32 GMT
ADD file:5c5cde050dbdbd5c7c0d9c723f436d37ab4a8b1a498647a719771eccce99d9cb in / 
# Sat, 28 May 2022 01:20:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:42:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:42:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:42:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:43:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 10:36:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 10:36:38 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 10:46:00 GMT
ENV RUBY_MAJOR=3.1
# Sat, 28 May 2022 10:46:00 GMT
ENV RUBY_VERSION=3.1.2
# Sat, 28 May 2022 10:46:00 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Sat, 28 May 2022 10:47:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 10:47:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 10:47:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 10:47:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 10:47:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 10:47:59 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:982cba7e471c6d3ce96014cf58b2e4e115a525e60da2e1e08716818f2c057a6b`  
		Last Modified: Sat, 28 May 2022 01:25:39 GMT  
		Size: 50.4 MB (50440422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02d86f59850f3e13d394072350625a8526b912af24b3bfc0e50e9a8862a79d0`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 7.9 MB (7856653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b047e8f2e47bdf998a952572ae5e9d64edf8e29b716be0ee50a15e6d21cb2ce`  
		Last Modified: Sat, 28 May 2022 02:50:21 GMT  
		Size: 10.0 MB (9997224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478cfe935c2fb922eb2a95131ad8a2f1e6ff472bbdecdf94709edc3a85f74dfd`  
		Last Modified: Sat, 28 May 2022 02:50:38 GMT  
		Size: 51.8 MB (51843777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9044b155d8ec2ce83fdaefff4a4514dda53e8012b3d5aea2d0f182aeddc08dd`  
		Last Modified: Sat, 28 May 2022 02:51:18 GMT  
		Size: 192.5 MB (192488821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f579dc13756423f28714beacb8800891d0b97156044b7c88d082089cf389b9c`  
		Last Modified: Sat, 28 May 2022 11:09:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a8fa2e55ff64e3c8cd9c66884baee3217c09a2c09b1a665c8aa65953b482b`  
		Last Modified: Sat, 28 May 2022 11:10:30 GMT  
		Size: 32.1 MB (32136572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4518d18dbc089e17a59bea7bbab12db48eade082540e68fd3d4cf27effc1d876`  
		Last Modified: Sat, 28 May 2022 11:10:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:buster` - linux; arm variant v5

```console
$ docker pull ruby@sha256:ba5495f85881999eea13bdd43dee45ce7cb9b9339ef7a619439cf8a41ed8a69b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.0 MB (317042251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:963d9fbca01e7c32855f046a57c0af8c12c8b8de308e7c116e72a4f2caba30ee`
-	Default Command: `["irb"]`

```dockerfile
# Sat, 28 May 2022 02:03:32 GMT
ADD file:ad4ce97f6ea5c59c2f067ac3448d897881ae301cb606e52556637f74cac09774 in / 
# Sat, 28 May 2022 02:03:33 GMT
CMD ["bash"]
# Sat, 28 May 2022 03:10:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:11:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 03:12:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 03:14:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 18:30:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 18:30:48 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 18:52:05 GMT
ENV RUBY_MAJOR=3.1
# Sat, 28 May 2022 18:52:05 GMT
ENV RUBY_VERSION=3.1.2
# Sat, 28 May 2022 18:52:05 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Sat, 28 May 2022 18:56:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 18:56:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 18:56:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 18:56:36 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 18:56:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 18:56:38 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:ec27c4ead5d8a5ae35fd4bad58cadacd3d006bed1911fd9b07b5e4f74921f7c9`  
		Last Modified: Sat, 28 May 2022 02:19:24 GMT  
		Size: 48.2 MB (48160631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a992114821be2e9710384caf39f14081084f800a2696a444f4ccbb0b1871735b`  
		Last Modified: Sat, 28 May 2022 03:33:34 GMT  
		Size: 7.4 MB (7400831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d07ea5e22b64ba119dfad12a9075a671c03b7ef047af4ba61bc5fd78cd2a0982`  
		Last Modified: Sat, 28 May 2022 03:33:35 GMT  
		Size: 9.7 MB (9687617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c1044d72ac1d1a1dae001eae9012d7d0f660f5a0ce319794ab546237ac3803`  
		Last Modified: Sat, 28 May 2022 03:34:20 GMT  
		Size: 49.6 MB (49583647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff189f2617675f66495c8020d53c024610dd37b6738c0c2cf601d6a9f95c187`  
		Last Modified: Sat, 28 May 2022 03:36:12 GMT  
		Size: 171.4 MB (171424836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a506098e6014c4a306f1b2f64a5dc709ed2b68ceed4ec0fd38d1a025df5b415d`  
		Last Modified: Sat, 28 May 2022 19:45:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efc9c5a3cc54c919d78ddc63a447ab576402431eaf8ee2e2738eb37b1ef6522`  
		Last Modified: Sat, 28 May 2022 19:48:33 GMT  
		Size: 30.8 MB (30784315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d93653828d3ab151cd3e4e41b050f09e1af32151d79df67fbbbac668b6f772`  
		Last Modified: Sat, 28 May 2022 19:48:19 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:buster` - linux; arm variant v7

```console
$ docker pull ruby@sha256:8b6b8134642dd9393e0d5fdfd545c71655987bcea5884b6d766b14bf448788c7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309112132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb411dc777f292388d8423963817e2b53ed0e57e723848b4011ad4d4f1a1ebb5`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 11 May 2022 01:49:37 GMT
ADD file:9c75d7f24328b3f84cd700813a0a8ff5af16399f4475d24da9b0a859d584614c in / 
# Wed, 11 May 2022 01:49:38 GMT
CMD ["bash"]
# Wed, 11 May 2022 03:25:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 03:26:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:28:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 08:16:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 May 2022 08:16:53 GMT
ENV LANG=C.UTF-8
# Thu, 12 May 2022 08:37:26 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 May 2022 08:37:26 GMT
ENV RUBY_VERSION=3.1.2
# Thu, 12 May 2022 08:37:27 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Thu, 12 May 2022 08:41:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 May 2022 08:41:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 May 2022 08:41:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 May 2022 08:41:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 08:41:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 12 May 2022 08:41:47 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:f328f2671b27c760193a9d82808b176a8a7420205e8eb884e1fee20d2ac57ff0`  
		Last Modified: Wed, 11 May 2022 02:05:20 GMT  
		Size: 45.9 MB (45910176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e554a91160b4bf86ab199d7a5f5f105c5ffecc37b098c4274d98c264f677799`  
		Last Modified: Wed, 11 May 2022 03:49:35 GMT  
		Size: 7.1 MB (7145025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1b07ef419c0604851908ed718983760891b21a649a1b8758b871522e7d3e48`  
		Last Modified: Wed, 11 May 2022 03:49:36 GMT  
		Size: 9.3 MB (9343816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398961d3cf225ff82b93bd457012e308b756c455d1dbe1191bca51a54483f1d7`  
		Last Modified: Wed, 11 May 2022 03:50:19 GMT  
		Size: 47.4 MB (47359230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:672070a3841f8c8993724742262e409c973f2ea02773250aff8b7c5bfe81bde6`  
		Last Modified: Wed, 11 May 2022 03:52:03 GMT  
		Size: 168.7 MB (168680126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06568f834863d921a2356e1d8db5ddb7bb7863d8ec5482aa769ab9084bca7599`  
		Last Modified: Thu, 12 May 2022 09:32:02 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2059fcf83d1119aa3f045b2f819f137a8054351b139a9a15e9fa2b0f0f06b728`  
		Last Modified: Thu, 12 May 2022 09:34:52 GMT  
		Size: 30.7 MB (30673384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95ac7ff040ecb0f38b09a2c5c3d91a55b92fb7bbda052b129651bff9e1b807b1`  
		Last Modified: Thu, 12 May 2022 09:34:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:buster` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:696052c0b444b2a451956807b30d83871fca0db8b06720867c782e5d9c42448f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.3 MB (334314593 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7098f3cdfcc01471b43afad191ddfb55f77c76055e1f5be064c3f77a2dda58d9`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 11 May 2022 00:47:11 GMT
ADD file:5389b77733b44ebc41850baff3ebfc491726af264a745f108d5f16076a0f04ab in / 
# Wed, 11 May 2022 00:47:11 GMT
CMD ["bash"]
# Wed, 11 May 2022 01:26:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:26:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 01:27:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 01:28:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:54:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 11 May 2022 14:54:22 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 15:04:03 GMT
ENV RUBY_MAJOR=3.1
# Wed, 11 May 2022 15:04:04 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 11 May 2022 15:04:05 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 11 May 2022 15:05:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 11 May 2022 15:05:56 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 11 May 2022 15:05:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 11 May 2022 15:05:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 15:05:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 11 May 2022 15:06:00 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:5528d23e3f315103c99c14258e007a025d09bb4fd587c2d8a32d6dbb6047b891`  
		Last Modified: Wed, 11 May 2022 00:54:09 GMT  
		Size: 49.2 MB (49228300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64b2d66a1dbe5960c6de4181ca3512467d3303dfb9cde3d92ecf7a85111cf68b`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 7.7 MB (7719789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9244ac9f9851b43ddc1032930666d339c3a5d9b934e2ca42ecd2e8ef3dd680`  
		Last Modified: Wed, 11 May 2022 01:37:01 GMT  
		Size: 9.8 MB (9767329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06885dc77f03f05a5f98ceb35e871f027525d932d32027ed9d4ffb0cbd29786c`  
		Last Modified: Wed, 11 May 2022 01:37:21 GMT  
		Size: 52.2 MB (52174787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be89f33c0b133b07e3c53ae901bde6bf63f6a395cdf9c89c263e8d1e625a61cf`  
		Last Modified: Wed, 11 May 2022 01:37:55 GMT  
		Size: 184.1 MB (184054008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670769473ba1e5324e0181ee972fbd68854f8c406dbdd45fe3ab56684c8fa958`  
		Last Modified: Wed, 11 May 2022 15:28:55 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315c426612dba716c2e149e54840b97c79773fcfa09324a79ffdf349a43b758e`  
		Last Modified: Wed, 11 May 2022 15:30:37 GMT  
		Size: 31.4 MB (31370039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b430636703032b76077a94f6bb6573401daa8ef7dcd94782c57a71a0c55ccafe`  
		Last Modified: Wed, 11 May 2022 15:30:34 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:buster` - linux; 386

```console
$ docker pull ruby@sha256:d0c2dcdc873a5a4ebd3fc24d1203275659e8b349a98368a7c25529f64af6bb28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.5 MB (352539554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:386dea908b25b6c5a42266bbeb65615445821e9b91c51a42a4dfe680fbbd1b1b`
-	Default Command: `["irb"]`

```dockerfile
# Sat, 28 May 2022 00:39:45 GMT
ADD file:3995ccc1e3f12a1e3f28dd818223bdc5454a7651248bfb98fae7c14961c49bba in / 
# Sat, 28 May 2022 00:39:45 GMT
CMD ["bash"]
# Sat, 28 May 2022 01:12:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 01:12:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 01:12:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 01:14:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:48:41 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 11:48:42 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 11:58:23 GMT
ENV RUBY_MAJOR=3.1
# Sat, 28 May 2022 11:58:24 GMT
ENV RUBY_VERSION=3.1.2
# Sat, 28 May 2022 11:58:25 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Sat, 28 May 2022 12:00:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 12:00:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 12:00:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 12:00:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 12:00:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 12:00:21 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:045913a916496008850e7e3b499b9acc93c72b4018eda833a11c562a6d8413b5`  
		Last Modified: Sat, 28 May 2022 00:47:08 GMT  
		Size: 51.2 MB (51204248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8b88cac678bf7c61d66ca5c565ceb244ff4764b8651c88bf3e1ae159872dd0`  
		Last Modified: Sat, 28 May 2022 01:22:38 GMT  
		Size: 8.0 MB (8022586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbc00efc59e7dbf25d25c6c5d412bc1115e1d5d65c61cb6e2c9d65b1f39faf8`  
		Last Modified: Sat, 28 May 2022 01:22:39 GMT  
		Size: 10.1 MB (10121911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7916ade5bb54b5ab127448e4b330bab4425569af949deb035ba142298784c147`  
		Last Modified: Sat, 28 May 2022 01:23:00 GMT  
		Size: 53.4 MB (53443985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde1cf8841a6c64f6fb1dce7d6d058db53618d3d3a123f80b2c158b5dfad4e7a`  
		Last Modified: Sat, 28 May 2022 01:23:35 GMT  
		Size: 199.0 MB (199012105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c6325e60865de1b8855f15cb7e2321963caa0188b0aeeaf3ca2c836dba1af7`  
		Last Modified: Sat, 28 May 2022 12:23:45 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b09bf21023a2ec107466e5479f43e633478bf3c0972c6037037acda71707ad`  
		Last Modified: Sat, 28 May 2022 12:25:35 GMT  
		Size: 30.7 MB (30734380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae643662c2f55cff63520f89207bee991040fb0c07686b8158e9ef5acaab09b`  
		Last Modified: Sat, 28 May 2022 12:25:31 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:buster` - linux; mips64le

```console
$ docker pull ruby@sha256:2ba9ea362165f332c5e5ada0a7feb954fabd0e7fd10f3c95f3bdbc1407914b5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.9 MB (328915382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f920cd51a4ee93d6965e98ca7b00f2955b0e5753e09eb8de4db14f9b9d052651`
-	Default Command: `["irb"]`

```dockerfile
# Sat, 28 May 2022 01:11:47 GMT
ADD file:e86c610403bdbc84066b42627ffdf92eb051badd2f3d1fcc964fba096215c297 in / 
# Sat, 28 May 2022 01:11:52 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:03:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:03:58 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:05:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:11:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 11:54:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 11:54:14 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 12:45:30 GMT
ENV RUBY_MAJOR=3.1
# Sat, 28 May 2022 12:45:36 GMT
ENV RUBY_VERSION=3.1.2
# Sat, 28 May 2022 12:45:42 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Sat, 28 May 2022 12:55:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 12:56:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 12:56:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 12:56:17 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 12:56:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 12:56:32 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:3ab17b7e8f7dffe546de1529b66b42c5d3aaa0aca409effcd962eae29b834d3e`  
		Last Modified: Sat, 28 May 2022 01:22:17 GMT  
		Size: 49.1 MB (49073373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d8359db5e9434db65ff74cbeb6fb2a3c11834bea89c8bc0c7a81edce49d561`  
		Last Modified: Sat, 28 May 2022 02:27:30 GMT  
		Size: 7.3 MB (7272979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e11e4fd36af841919e6113b762dace3a649390107a2ed9224e952e9b71cec164`  
		Last Modified: Sat, 28 May 2022 02:27:30 GMT  
		Size: 9.8 MB (9800289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4e1559e22aa070dc273c40b7ca110c836f73f219de789819c50db5abf12294`  
		Last Modified: Sat, 28 May 2022 02:28:18 GMT  
		Size: 50.9 MB (50861197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edc6014a1d77c037b5ca755cb082ca750b5b0caf9a70fcb56472fcbcfc4050`  
		Last Modified: Sat, 28 May 2022 02:30:21 GMT  
		Size: 180.0 MB (180015753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eecf6c6e75821ecc6e0e818a431c2bfa41d179a9da4ad040b4090c0462265e5`  
		Last Modified: Sat, 28 May 2022 14:35:59 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e69303267f3ad5f8f85c338c565222f4aca3ce95eef2bffa00b1a02f6db5a5`  
		Last Modified: Sat, 28 May 2022 14:38:17 GMT  
		Size: 31.9 MB (31891450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50fa94bcb07f3dfcd996cb101f7c1127e68d32624d6b6b47f65a024366e415`  
		Last Modified: Sat, 28 May 2022 14:38:03 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:buster` - linux; ppc64le

```console
$ docker pull ruby@sha256:5d630d703496d51d4f8131a8540f75a6cc752a3a293122a6807ef089235c5d5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.3 MB (366331881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eebcf562b5930ba73d012a9b09782d836985f9a68004f37d8fdbe5a2adf6fa7`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 11 May 2022 01:32:53 GMT
ADD file:73ff2a18e50b226a862b74c50f091d80ddcd29f404879c4937887c560fdf624d in / 
# Wed, 11 May 2022 01:33:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:54:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:55:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 May 2022 02:58:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 03:20:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 05:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 12 May 2022 05:08:32 GMT
ENV LANG=C.UTF-8
# Thu, 12 May 2022 05:37:10 GMT
ENV RUBY_MAJOR=3.1
# Thu, 12 May 2022 05:37:11 GMT
ENV RUBY_VERSION=3.1.2
# Thu, 12 May 2022 05:37:14 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Thu, 12 May 2022 05:41:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 12 May 2022 05:41:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 12 May 2022 05:41:32 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 12 May 2022 05:41:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 12 May 2022 05:41:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 12 May 2022 05:41:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:88d357d3afb8b0de721a4298ddb31fe73077663376e53d241a3d5217080e1f73`  
		Last Modified: Wed, 11 May 2022 01:43:32 GMT  
		Size: 54.2 MB (54170196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad446f507e97c97d9b6d29a8cd467c962ad6b7baa48356927e7afec937107eb`  
		Last Modified: Wed, 11 May 2022 03:49:39 GMT  
		Size: 8.3 MB (8293358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8784653a0c174d00c413056e723bd1a8692a8c27bfbe6508e37152d86bb395f4`  
		Last Modified: Wed, 11 May 2022 03:49:39 GMT  
		Size: 10.7 MB (10727832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8e974e0992db0fc98b88da2883b630af2407799183b4fe45d51e044b60ccf7`  
		Last Modified: Wed, 11 May 2022 03:50:04 GMT  
		Size: 57.5 MB (57458396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32fe3cc75c4624247cf639de03bd8d25c55a40ee6f9c3c999ec982a16043e11`  
		Last Modified: Wed, 11 May 2022 03:50:50 GMT  
		Size: 203.4 MB (203371891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3373780f497d47b847419510d44dffe2abfd373de09c1fb9603743f2112711`  
		Last Modified: Thu, 12 May 2022 06:43:56 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2593ca53c56d3526bc9e97dd5979913d4abbb2c5aac1a07cc6048ae607fc99c4`  
		Last Modified: Thu, 12 May 2022 06:46:04 GMT  
		Size: 32.3 MB (32309832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee6e770d71b5d2d04d650d9ae93a42492cf29352fc00894672c205902f40b43`  
		Last Modified: Thu, 12 May 2022 06:46:00 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:buster` - linux; s390x

```console
$ docker pull ruby@sha256:4f4990a1fe22f4ecd1b4f3e5da184cb2fb1a0a3eab2fcaeab57591023a551a6c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.7 MB (326731812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22a6f0721d169e28889bf1fddb6999c44884ebef66c9418d0483a938d0fa2d27`
-	Default Command: `["irb"]`

```dockerfile
# Sat, 28 May 2022 00:43:20 GMT
ADD file:65712051a170cb9d0b18d0085bc26171598119b8946fa55b5ee959661b48a5d2 in / 
# Sat, 28 May 2022 00:43:26 GMT
CMD ["bash"]
# Sat, 28 May 2022 02:25:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:25:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 May 2022 02:25:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 02:27:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:37:12 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 May 2022 14:37:12 GMT
ENV LANG=C.UTF-8
# Sat, 28 May 2022 14:55:35 GMT
ENV RUBY_MAJOR=3.1
# Sat, 28 May 2022 14:55:36 GMT
ENV RUBY_VERSION=3.1.2
# Sat, 28 May 2022 14:55:36 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Sat, 28 May 2022 14:58:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 May 2022 14:59:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 28 May 2022 14:59:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 28 May 2022 14:59:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 May 2022 14:59:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 28 May 2022 14:59:05 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:771d2d61f47933c8d05a5f7e35dcb16848a6225e7531db8e5971d528982538e9`  
		Last Modified: Sat, 28 May 2022 00:50:02 GMT  
		Size: 49.0 MB (49006810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df770b877bc8966d8f5d52cb3a7ab3f8bbd879f885cd61e637b2561657af7817`  
		Last Modified: Sat, 28 May 2022 02:36:01 GMT  
		Size: 7.4 MB (7423705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfa8ac3a66d83a9351be236e2dad0b6305f4fc7f162891629ed852f205e884e`  
		Last Modified: Sat, 28 May 2022 02:36:01 GMT  
		Size: 9.9 MB (9883325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bc90555bb48ea3318f33a26a32ad4a827ace919e55dd094bd11e93c555a857`  
		Last Modified: Sat, 28 May 2022 02:36:17 GMT  
		Size: 51.4 MB (51382611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc0c1ea0ceff56a8da88d248fa4aed641749e436417dcebf9e8611397fdebfd`  
		Last Modified: Sat, 28 May 2022 02:36:43 GMT  
		Size: 177.0 MB (176965534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23771c958a6cab189770ed57ad0cf84460487bf5ee7d7b859135ac7fec618b6c`  
		Last Modified: Sat, 28 May 2022 15:38:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8885e7f95a85e960f6c248a009dca9d6cdd84a091a92275f9aac6a4614afda4e`  
		Last Modified: Sat, 28 May 2022 15:39:30 GMT  
		Size: 32.1 MB (32069455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f89950e4aff63e8d2d155e1fc6b7fe9169cb6c93155bbbddb28730c394d9d60`  
		Last Modified: Sat, 28 May 2022 15:39:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
