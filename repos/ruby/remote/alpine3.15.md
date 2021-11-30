## `ruby:alpine3.15`

```console
$ docker pull ruby@sha256:8d2fe1b92d288204f9db1a64b02046c60d62a03add1398a8a3c56d9e3c78814e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ruby:alpine3.15` - linux; amd64

```console
$ docker pull ruby@sha256:8ec4194e3df279ef459ed06724dd455964defcf49857c161154378a0e4df98a9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33059555 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f8b052396a9a7d595d60490999f94f32d1e3bdbe5b2757b854d0b816eaabd44`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 09:19:26 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 09:19:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 09:19:27 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 09:24:15 GMT
ENV RUBY_MAJOR=3.0
# Tue, 30 Nov 2021 09:24:15 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 30 Nov 2021 09:24:15 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 30 Nov 2021 09:28:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 09:28:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 09:28:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 09:28:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 09:28:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 09:28:22 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfdfc99c764bed7ef3f6377b64d99601e47cc4087154ed69e70fa5b8cc8fa92`  
		Last Modified: Tue, 30 Nov 2021 09:37:08 GMT  
		Size: 3.7 MB (3692788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcec1f1cb7c30b5406814a3edc744a6a23fb0c8c6f304e2a2ca9521daa1da01`  
		Last Modified: Tue, 30 Nov 2021 09:37:08 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8a51348a068e62ab9b4d36f65bd530cac81c740174f81e503ce55607a84c01`  
		Last Modified: Tue, 30 Nov 2021 09:37:38 GMT  
		Size: 26.5 MB (26547959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0aa6c607b4ede3de74f0d09e6d0bc5ce397ea557170de4927dea9aa6ae8fc7d`  
		Last Modified: Tue, 30 Nov 2021 09:37:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine3.15` - linux; arm variant v6

```console
$ docker pull ruby@sha256:57b721f54ac56a294175d7051f17b002a377768d629dba003d94acfbfd5c90aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31732374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:042292b818246037fa67976fcdc4e02ef0de5def9bd7bdf7d6f1693ff8fe3066`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:31:21 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 05:31:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 05:31:23 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 05:36:33 GMT
ENV RUBY_MAJOR=3.0
# Tue, 30 Nov 2021 05:36:33 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 30 Nov 2021 05:36:34 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 30 Nov 2021 05:40:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 05:40:56 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 05:40:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 05:40:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 05:40:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 05:40:59 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842eb5d56c73e6f9e351db359308334ee810d1cb732270ae35bfdaa5208caf9c`  
		Last Modified: Tue, 30 Nov 2021 05:52:37 GMT  
		Size: 3.4 MB (3441437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c29b1da293c8320455d68a5d44ebe572144259afdb3aed7c4d69ac9d80a4d2`  
		Last Modified: Tue, 30 Nov 2021 05:52:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8b71b72a3b53d02f33792831496a22a8927d006cb19425203c8ad88115ac57`  
		Last Modified: Tue, 30 Nov 2021 05:53:20 GMT  
		Size: 25.7 MB (25659119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2feb123e649093eb646ed4fa20b3d89fa0cecc745bc572d3dae7e41e73a27ca6`  
		Last Modified: Tue, 30 Nov 2021 05:53:09 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:52a77fc6174f6609a5747b3846a3d93a54d2b63fb23df5893578c67502509d29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32629870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0136df5e14a82b00388520987de9282680f43eab01d26ff29c7e4c3acb7786bf`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:36:33 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 05:36:34 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 05:36:35 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 05:39:42 GMT
ENV RUBY_MAJOR=3.0
# Tue, 30 Nov 2021 05:39:43 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 30 Nov 2021 05:39:44 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 30 Nov 2021 05:42:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 05:42:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 05:42:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 05:42:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 05:42:06 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 05:42:07 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e12e2c567460b1b6fc7c47caaf0096b83279da72da30d631a78973212f186a`  
		Last Modified: Tue, 30 Nov 2021 05:50:38 GMT  
		Size: 3.7 MB (3657031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd57995982ca19298b043d92ab79f0d14ea093fda2b52a2b4a4a00ea9af2b13`  
		Last Modified: Tue, 30 Nov 2021 05:50:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909771bd70f7d1b94404e8ad63e2df3c5c82264baf2b286ceb4477256b26f49e`  
		Last Modified: Tue, 30 Nov 2021 05:51:18 GMT  
		Size: 26.3 MB (26257070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c904dab3d3dab4870237325d58d9bf8a83865f5a8fbd936586d7f5fa25b886`  
		Last Modified: Tue, 30 Nov 2021 05:51:15 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine3.15` - linux; 386

```console
$ docker pull ruby@sha256:6b3cc3ac047979b58efe2da3bf4a732d4fe4b06d28e48b63753a2752c66a0ef4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32197513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7057f3e5fd2eba58e660fed735499541c9686ca8ee391c1d99a5d584a43a080`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 08:37:44 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 08:37:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 08:37:47 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 08:45:42 GMT
ENV RUBY_MAJOR=3.0
# Tue, 30 Nov 2021 08:45:43 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 30 Nov 2021 08:45:43 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 30 Nov 2021 08:52:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 08:52:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 08:52:47 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 08:52:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 08:52:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 08:52:50 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae05e47cf02db9a8baff44ce7728fa8e3e4c903d33d017437f9c402d4c448299`  
		Last Modified: Tue, 30 Nov 2021 09:04:59 GMT  
		Size: 3.7 MB (3716923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6021ca2d58b5286b59b232c69e4e1f40cd538b8d4ca8893f2be4420c1198845`  
		Last Modified: Tue, 30 Nov 2021 09:04:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb9989e35efe23acc311bc31c1596612d8ce48c35333d6131ee30e2b58c0298`  
		Last Modified: Tue, 30 Nov 2021 09:05:43 GMT  
		Size: 25.7 MB (25653077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654fb84e774b1e52e24093f4d38679612c3a9f7d4f84040aa4001e3bf074351c`  
		Last Modified: Tue, 30 Nov 2021 09:05:40 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine3.15` - linux; ppc64le

```console
$ docker pull ruby@sha256:c961092447052719b4479d8841a33164b73509f8f59c041953b498b45cd6d771
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33544920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4de81da087f9ea826cce2072d1ec7cbfdb32881cfa73730ba772e1f02ec65999`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 07:45:57 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 07:46:04 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 07:46:07 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 07:50:28 GMT
ENV RUBY_MAJOR=3.0
# Tue, 30 Nov 2021 07:50:31 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 30 Nov 2021 07:50:32 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 30 Nov 2021 07:53:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 07:53:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 07:53:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 07:53:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 07:53:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 07:53:48 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60dfb224d10621897aed06dde46dd5c4c649f159947d6425fc8d43cd1b6437fb`  
		Last Modified: Tue, 30 Nov 2021 08:04:09 GMT  
		Size: 3.8 MB (3810519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a630f14514f37223fa8f0cbd3071c6b038a767df40188168543d2e3d3947ed72`  
		Last Modified: Tue, 30 Nov 2021 08:04:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2949386e0d7e7b2911b5b9c84306b5db151c3ccbcc1929e7f66f1f87f403f5`  
		Last Modified: Tue, 30 Nov 2021 08:04:49 GMT  
		Size: 26.9 MB (26919224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0b0c1b322f52a8c32c60fa0f0f31137bad4193cbfdf70404a752f2310da55`  
		Last Modified: Tue, 30 Nov 2021 08:04:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine3.15` - linux; s390x

```console
$ docker pull ruby@sha256:719cef340f7db7eb34fc1dc24ab45820a74024cfb557d68905560c24210fcd5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33124064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebb31797aaf219cff1d6083e2c7dfcca1a610b9d904ba5765390c47b8af8719f`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 09:51:07 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 09:51:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 09:51:08 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 09:54:03 GMT
ENV RUBY_MAJOR=3.0
# Tue, 30 Nov 2021 09:54:03 GMT
ENV RUBY_VERSION=3.0.3
# Tue, 30 Nov 2021 09:54:03 GMT
ENV RUBY_DOWNLOAD_SHA256=88cc7f0f021f15c4cd62b1f922e3a401697f7943551fe45b1fdf4f2417a17a9c
# Tue, 30 Nov 2021 09:56:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 09:56:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 09:56:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 09:56:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 09:56:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 09:56:28 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7faf48375ad71a3a34aeb82123f04c9dfdba63e9e43a8131a57fb8581ef31e0`  
		Last Modified: Tue, 30 Nov 2021 10:04:36 GMT  
		Size: 3.8 MB (3754915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b691f4487c4a11eb5d8ddb0d557cf1843f5c095ca7b8ac7934cffb1749fda1`  
		Last Modified: Tue, 30 Nov 2021 10:04:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0858e8632a486903c7a38b9a2305072b1123e4d5643380b8b08fcb7bd8976a95`  
		Last Modified: Tue, 30 Nov 2021 10:05:08 GMT  
		Size: 26.8 MB (26762809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab19cd838e4cc9fdd92236c8a2895a50ab799c89e1aed38b20dcd8c4fe455b28`  
		Last Modified: Tue, 30 Nov 2021 10:05:06 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
