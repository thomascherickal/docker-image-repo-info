## `ruby:2-alpine`

```console
$ docker pull ruby@sha256:6320d08e6e903a3193e15c93fd1efe5637119138be3c957ddcd29f6ac1d7c0dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ruby:2-alpine` - linux; amd64

```console
$ docker pull ruby@sha256:be7685db89caba9fb1ccc6479cb4be15b2472003b6488575610ce908c6ccc5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.4 MB (20437387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79a63cfc399aac7c1b4aed6a7c1663e3fae985f58862bd9dc331b4c7082ddd8e`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:54:34 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 06 Aug 2021 19:54:35 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 06 Aug 2021 19:54:35 GMT
ENV LANG=C.UTF-8
# Fri, 06 Aug 2021 20:01:07 GMT
ENV RUBY_MAJOR=2.7
# Fri, 06 Aug 2021 20:01:08 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 06 Aug 2021 20:01:08 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 06 Aug 2021 20:04:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 06 Aug 2021 20:04:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 06 Aug 2021 20:04:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 06 Aug 2021 20:04:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 06 Aug 2021 20:04:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 06 Aug 2021 20:04:52 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8128176f3a5e284cf58e95cb6a09827d081398e33dfae85702d511f9e959724a`  
		Last Modified: Fri, 06 Aug 2021 20:07:55 GMT  
		Size: 3.6 MB (3643910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b8d272a912171344b917f3f5426c80d0c1682cb4834ee2e5e1875d84adfc97`  
		Last Modified: Fri, 06 Aug 2021 20:07:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3d29640df7a127a9950c0dbf83b584be70f3d5a3130f2438453e3049f7f8a`  
		Last Modified: Fri, 06 Aug 2021 20:08:36 GMT  
		Size: 14.0 MB (13980075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6b623d48ef69de33eaa5309c40e9ab4ed589c251f98649d6d2454c65b61da5`  
		Last Modified: Fri, 06 Aug 2021 20:08:33 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine` - linux; arm variant v6

```console
$ docker pull ruby@sha256:ee91261470068759d88f06058eda7ccedc0a5ffb9679d2c82f08817b67ec4384
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24730066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f72861deda8ea8dfb9b9c3fe49b48b40ed3c1fd579a224f76b20d5df072ee72`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:34:10 GMT
RUN apk add --no-cache 		gmp-dev
# Mon, 21 Oct 2019 18:34:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Mon, 21 Oct 2019 18:41:24 GMT
ENV RUBY_MAJOR=2.6
# Mon, 21 Oct 2019 18:41:29 GMT
ENV RUBY_VERSION=2.6.5
# Mon, 21 Oct 2019 18:41:37 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Mon, 21 Oct 2019 18:48:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 21 Oct 2019 18:48:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 21 Oct 2019 18:48:12 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 21 Oct 2019 18:48:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 21 Oct 2019 18:48:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 21 Oct 2019 18:48:21 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e642771bfce54b4f119f9e7e7e2f8d4ca66f67241e36dc4bdff87d260f378bfa`  
		Last Modified: Mon, 21 Oct 2019 19:01:50 GMT  
		Size: 888.1 KB (888071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f605eda2fae16aad177e4eefde4d2429fa05675ba2e3414dc2b265ce1d85cd`  
		Last Modified: Mon, 21 Oct 2019 19:01:51 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82a8e19805f0467d60b68f88b4eeaf97e65827d69b6f04f1c8a2f9b79d79a4d`  
		Last Modified: Mon, 21 Oct 2019 19:02:16 GMT  
		Size: 21.3 MB (21270290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1f8e9edcc9ffef51af8893b2dc1f1341c51219800e6cc7a33c0a82cd90db66`  
		Last Modified: Mon, 21 Oct 2019 19:02:09 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine` - linux; arm variant v7

```console
$ docker pull ruby@sha256:51f4a10a6666c139b643bb49aca1025e1ba41a4d1b974beeedb88a67f3c0135d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.3 MB (24285220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85caef42cde932ae5d4e73f2e242fbb7990f27d2112e5b591789bbd79e99f2b7`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 19:31:48 GMT
RUN apk add --no-cache 		gmp-dev
# Mon, 21 Oct 2019 19:31:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Mon, 21 Oct 2019 19:35:08 GMT
ENV RUBY_MAJOR=2.6
# Mon, 21 Oct 2019 19:35:09 GMT
ENV RUBY_VERSION=2.6.5
# Mon, 21 Oct 2019 19:35:09 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Mon, 21 Oct 2019 19:37:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 21 Oct 2019 19:37:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 21 Oct 2019 19:37:50 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 21 Oct 2019 19:37:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 21 Oct 2019 19:37:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 21 Oct 2019 19:37:52 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3397092e1882b73493a2b0ec680f2e6ef011a2ed05ec0c99b60e9d72315142da`  
		Last Modified: Mon, 21 Oct 2019 19:48:53 GMT  
		Size: 827.3 KB (827262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a050b6f5da1c3b8618e9e962acd9ab2bb7e88e38f8db35c2f77e92772c349`  
		Last Modified: Mon, 21 Oct 2019 19:48:53 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2400983410773ff1cac1c1abbc396f5b8589e199ba07104b3a65d52cd9068768`  
		Last Modified: Mon, 21 Oct 2019 19:49:20 GMT  
		Size: 21.1 MB (21079126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a289fdd3dae490359be108ef7107eca6b866c73e527e0ff3127360796fc79195`  
		Last Modified: Mon, 21 Oct 2019 19:49:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:ada1b470d493e3417fba2feeb3d9463b115fdb358f3a6d15434f5c384bccf929
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **20.2 MB (20154370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38adece6b60e8ce7105cf2b7084ee34d314a84dc814486967cd2ae65ead8b5e2`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 01:05:15 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 07 Aug 2021 01:05:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 07 Aug 2021 01:05:16 GMT
ENV LANG=C.UTF-8
# Sat, 07 Aug 2021 01:08:44 GMT
ENV RUBY_MAJOR=2.7
# Sat, 07 Aug 2021 01:08:44 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 07 Aug 2021 01:08:44 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 07 Aug 2021 01:11:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 07 Aug 2021 01:11:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 07 Aug 2021 01:11:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 07 Aug 2021 01:11:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 07 Aug 2021 01:11:06 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 07 Aug 2021 01:11:06 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc7097f6544fd8a2b1818da82ea8157dab5d7157707bf11ddcf8b36fb1d7d22`  
		Last Modified: Sat, 07 Aug 2021 01:14:39 GMT  
		Size: 3.6 MB (3629786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:341562b3271fdb3c350aa7b13d656fafb148e151ef0587062df851209ac9a03f`  
		Last Modified: Sat, 07 Aug 2021 01:14:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e31b5542eda631faacbb1667a53b13347d83abf27fce0f7151153bf0e49723`  
		Last Modified: Sat, 07 Aug 2021 01:15:24 GMT  
		Size: 13.8 MB (13813576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc3223318628a47ba3069f1e1c1b314508b932d45a941826835e1dea80e0010`  
		Last Modified: Sat, 07 Aug 2021 01:15:22 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine` - linux; 386

```console
$ docker pull ruby@sha256:f1d2d55820fa900870290c9fd2ec4859c11a776c420059e30c95d790d9fa2ac0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **19.8 MB (19801184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12145bb23bf38d151319cf7835adbcc9aa2e6c0e9b5e959732ec4d7884fc7419`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 02:42:05 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 07 Aug 2021 02:42:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 07 Aug 2021 02:42:06 GMT
ENV LANG=C.UTF-8
# Sat, 07 Aug 2021 02:46:54 GMT
ENV RUBY_MAJOR=2.7
# Sat, 07 Aug 2021 02:46:54 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 07 Aug 2021 02:46:54 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 07 Aug 2021 02:50:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 07 Aug 2021 02:50:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 07 Aug 2021 02:50:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 07 Aug 2021 02:50:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 07 Aug 2021 02:50:06 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 07 Aug 2021 02:50:06 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce58f4bce0d83b9ad132c4e252e7ed5f4dc850f9dded0487855270e58107bfe`  
		Last Modified: Sat, 07 Aug 2021 02:54:03 GMT  
		Size: 3.7 MB (3679020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a416028927d984d7993822a28b14b7fea10e5fff1a5c2e5cae6a030543cb629`  
		Last Modified: Sat, 07 Aug 2021 02:54:01 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c59a58662c500087881ae94c827041b9a10aa1de395527104cf54328586f352`  
		Last Modified: Sat, 07 Aug 2021 02:54:50 GMT  
		Size: 13.3 MB (13299859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ade9b3483e6b0277eaf9926d5b54f9f818e91267e57c6ef6b0eb52bd59d1ff`  
		Last Modified: Sat, 07 Aug 2021 02:54:48 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine` - linux; ppc64le

```console
$ docker pull ruby@sha256:ecc20421f65e1a67bf7c81eeb7dd22a6334766000d96e59f7e58c053872b209a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 MB (21044959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae0639920c069e5caca071214d43c6c01bee5f54fd85ef11e3bc37b707c9c004`
-	Default Command: `["irb"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:59:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 27 Aug 2021 21:00:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 27 Aug 2021 21:00:35 GMT
ENV LANG=C.UTF-8
# Fri, 27 Aug 2021 21:05:37 GMT
ENV RUBY_MAJOR=2.7
# Fri, 27 Aug 2021 21:05:41 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 27 Aug 2021 21:05:48 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 27 Aug 2021 21:08:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 27 Aug 2021 21:08:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 27 Aug 2021 21:08:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 27 Aug 2021 21:08:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 27 Aug 2021 21:09:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 27 Aug 2021 21:09:04 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5e2e2db52d7e5f901854ad106be68d9b8df4c99ab6d4d740bc046cc6f34a715`  
		Last Modified: Fri, 27 Aug 2021 21:16:41 GMT  
		Size: 3.8 MB (3783896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb62b3d1d2806082b27eed458f75f812df7acb91dc474cc1076c38d8ca5c0cc`  
		Last Modified: Fri, 27 Aug 2021 21:16:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ad28d4353ce2db91f74bb1b18f1d1a148c99d79ecbf65adf8e9d3eeb29ff46`  
		Last Modified: Fri, 27 Aug 2021 21:17:27 GMT  
		Size: 14.4 MB (14448384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff555813f5f9c7700f11f2aaa774be582a77b9c1b66c23883e67bf26f2636ca`  
		Last Modified: Fri, 27 Aug 2021 21:17:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:2-alpine` - linux; s390x

```console
$ docker pull ruby@sha256:aa09239d411c371bf37af9fbe879c9a0c07b13728b785aee187615f684f69991
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (25970264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a872e8e4ce0a19ce0c6ad8c4606ada7c69b7c77f2ec8f823438e51b4df4685bc`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 21 Oct 2019 16:47:28 GMT
ADD file:49020543846e4f93b34d71c0e4234ade7bd6dde3f45cb73784aa73ce0522c8bc in / 
# Mon, 21 Oct 2019 16:47:29 GMT
CMD ["/bin/sh"]
# Tue, 22 Oct 2019 01:23:03 GMT
RUN apk add --no-cache 		gmp-dev
# Tue, 22 Oct 2019 01:23:04 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 22 Oct 2019 01:25:40 GMT
ENV RUBY_MAJOR=2.6
# Tue, 22 Oct 2019 01:25:40 GMT
ENV RUBY_VERSION=2.6.5
# Tue, 22 Oct 2019 01:25:40 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Tue, 22 Oct 2019 01:27:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 22 Oct 2019 01:27:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 22 Oct 2019 01:27:43 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 22 Oct 2019 01:27:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 22 Oct 2019 01:27:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 22 Oct 2019 01:27:45 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:fb7172052a60e640810f01efff381654bf9ed44082461455cfcc6306d192d541`  
		Last Modified: Mon, 21 Oct 2019 16:48:40 GMT  
		Size: 2.6 MB (2573587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef57812bb6e5d1db3ce1a535efaf0075220e7819127da4a402d3a153cd45496f`  
		Last Modified: Tue, 22 Oct 2019 01:35:00 GMT  
		Size: 1.1 MB (1111599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f06a5c7888d0bfaeab6931ac4ad0e747af97ec16a2b2eabf1a263ccfd554c5`  
		Last Modified: Tue, 22 Oct 2019 01:34:59 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9f7b8bb6bacd83440fc0b1907d501cb1a145098e6198df3055cd0a51d67959`  
		Last Modified: Tue, 22 Oct 2019 01:35:18 GMT  
		Size: 22.3 MB (22284740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d52d9cb1bf7985b860d375154d3d65ed801f16ed7e349b33aaf4c202f573042`  
		Last Modified: Tue, 22 Oct 2019 01:35:16 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
