## `ruby:3-alpine3.12`

```console
$ docker pull ruby@sha256:115ca01843799618a04db1470348ffa482e45a722ad8d4992c27db7aaba554e9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `ruby:3-alpine3.12` - linux; amd64

```console
$ docker pull ruby@sha256:3ee3d9e9820d3885cddec04ef7e61b994992163ac3d6f8d81f17ab99f3a94042
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.8 MB (32802125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ccb8ee44828941d968ad35464fe5207b80bd845850e4a95517806be5af154e1`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:11:41 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 15 Apr 2021 03:11:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 15 Apr 2021 03:11:43 GMT
ENV LANG=C.UTF-8
# Thu, 15 Apr 2021 03:11:44 GMT
ENV RUBY_MAJOR=3.0
# Thu, 15 Apr 2021 03:11:44 GMT
ENV RUBY_VERSION=3.0.1
# Thu, 15 Apr 2021 03:11:44 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Thu, 15 Apr 2021 03:16:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 15 Apr 2021 03:16:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 15 Apr 2021 03:16:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 15 Apr 2021 03:16:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Apr 2021 03:16:06 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 15 Apr 2021 03:16:06 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:467b8fbfadaf6004690377bd47dacd9f3cb1b32c529c126b5f3131f5a54b3c6b`  
		Last Modified: Thu, 15 Apr 2021 03:40:14 GMT  
		Size: 1.2 MB (1196163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f201a2281a386a91906846f1f508eadbe78e0cba8c5b0101df9d9612add16d`  
		Last Modified: Thu, 15 Apr 2021 03:40:13 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae406078fb51d6664175247de0e62416180d96c65172d597a6d5d564f0e7eb7`  
		Last Modified: Thu, 15 Apr 2021 03:40:18 GMT  
		Size: 28.8 MB (28804998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4e30433980336957645d2891bec7dd5e4322a663873b2871300ba0f3b2f6c1f`  
		Last Modified: Thu, 15 Apr 2021 03:40:13 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; arm variant v6

```console
$ docker pull ruby@sha256:22242c7500580c372e4ef56176dcb1fba12708aa8bdfcd5db0cbe95da3361b28
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31448571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8156326d6f33c9552676ec884db707dc2f58d82fa22de5e5846a5dd5b0ee4486`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:08:42 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 03:08:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 03:08:47 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 03:08:48 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 18:07:31 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 18:07:32 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 18:11:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 18:11:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 18:11:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 18:11:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 18:11:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 18:11:23 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e560f3f5f69db2274f88d7ab395cc265f6d76a53b7b7e5887c49d291c7db399`  
		Last Modified: Thu, 01 Apr 2021 03:42:19 GMT  
		Size: 1.1 MB (1050134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb86bab5a7cb0c5321edd384fb9bccb415326de5fde85c2deb43e3849ed5f0f`  
		Last Modified: Thu, 01 Apr 2021 03:42:18 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf36caf58a899109a7b324274587f1fbc79d7c50e04abb4332b524fe713041d`  
		Last Modified: Mon, 05 Apr 2021 18:40:26 GMT  
		Size: 27.8 MB (27793383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69eeaa60ac821861fd73e93d9915bbe7197349855c36586928a6a8c8ef8629f`  
		Last Modified: Mon, 05 Apr 2021 18:40:19 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; arm variant v7

```console
$ docker pull ruby@sha256:65f32f1e77b6a84aa202cf6f0375f896869bbdf809014ed55877d6e99c23522f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31000937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d3d8dcc9637449d58458556de2a133ccc4465075467ac8a0bf5bdf534d7ae57`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 06:26:10 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 06:26:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 06:26:14 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 06:26:16 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 18:39:05 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 18:39:06 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 18:41:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 18:41:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 18:41:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 18:41:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 18:41:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 18:41:54 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dd93bee14340912ec28d8250d6c5d8af237aff273b51ae5369ee73100a5d83`  
		Last Modified: Thu, 01 Apr 2021 06:55:43 GMT  
		Size: 977.0 KB (976952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627d798044d952b9a814aa4258dd447a1e5d98f2f89f4523c1f58f4645bc43c3`  
		Last Modified: Thu, 01 Apr 2021 06:55:43 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2606e90bad792e8fa0d9936f2adbde8db0ef67ae7f84a69bc1551d74715ce83e`  
		Last Modified: Mon, 05 Apr 2021 19:42:14 GMT  
		Size: 27.6 MB (27615322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593290be76a93aa178cdc2cb513582f5414062ec950564df0d517619a761aa28`  
		Last Modified: Mon, 05 Apr 2021 19:42:07 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:6522a19ad84d7ee05555967f30e0ea340f9ad27cf7c5eeaaf2b208e08f761015
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32429942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:586e139a3f0400e1500b8dd6c14943ddcce641a5f1f2767608a6f7b3b9dba94c`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:26:35 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 11:26:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 11:26:39 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 11:26:40 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 21:45:36 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 21:45:37 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 21:48:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 21:48:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 21:48:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 21:48:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 21:48:32 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 21:48:33 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650f12044fdb524016baca6ba353b003591cb305641126d0c8228c36db9aa9e8`  
		Last Modified: Thu, 01 Apr 2021 11:54:18 GMT  
		Size: 1.2 MB (1207174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1107ba88f696e91073d431af41cc8469c7739466d63628b267092d9ed5cbebb`  
		Last Modified: Thu, 01 Apr 2021 11:54:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d5d7e83f7e30e386b84554143d8e01398ef52b1d0202f645d41b2a8270fe68`  
		Last Modified: Mon, 05 Apr 2021 22:45:54 GMT  
		Size: 28.5 MB (28512521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c80682312b83c0288d3ff3943bee38dc2803b1a98d9e02c2686ee922dbde7fc1`  
		Last Modified: Mon, 05 Apr 2021 22:45:48 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; 386

```console
$ docker pull ruby@sha256:6e6c6fb5fb74870c2fd203b44569add8adf7dae787ace42348f1981c085ad387
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31993445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:266360eca8f344b7ae42a5cbb026a4df53c24007f08ec73e3015217694175e7d`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 00:00:16 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 00:00:17 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 00:00:17 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 00:00:17 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 18:49:12 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 18:49:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 18:54:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 18:54:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 18:54:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 18:54:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 18:54:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 18:54:44 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4466a8083abf9d842f98d0cba81098a01346f973c9162907dfd706294cd82db3`  
		Last Modified: Thu, 01 Apr 2021 00:35:59 GMT  
		Size: 1.2 MB (1236740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f63526dd8e8fa24cc0a5cc147686b17247196441cf3fe61329e04e70fcac56`  
		Last Modified: Thu, 01 Apr 2021 00:35:59 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3820c04c823de6c5deb998a06a016359c37c21fc2b9e191369dae7ed5315ac78`  
		Last Modified: Mon, 05 Apr 2021 20:12:18 GMT  
		Size: 28.0 MB (27961332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e5da46e7f2283040c7a0a0f5dfff69b9dcb80aa1d70a821a65efea06efeb82`  
		Last Modified: Mon, 05 Apr 2021 20:12:11 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; ppc64le

```console
$ docker pull ruby@sha256:bc7e6642a13c0367596e80ed61a072547d8f44ef0c598b0f1ad1466405a2e55e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33279256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddb3edc7058101aa0135dfa0699941df8d4ce7068342c3cabc82dc38e73045d4`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 18:26:21 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 18:26:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 18:26:39 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 18:26:45 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 18:57:19 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 18:57:30 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 19:00:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:01:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:01:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:01:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:01:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:01:51 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfdabdf294394b155a47243c3b77dedde6c9d793f19684cfbbd7719a3d5adce`  
		Last Modified: Thu, 01 Apr 2021 19:02:26 GMT  
		Size: 1.3 MB (1282989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37accb66e288b5da2baaafb39e66712cb0f2560bc409893ab3adcb3374b106f6`  
		Last Modified: Thu, 01 Apr 2021 19:02:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77df3e69e647fc15a8e3fa09fd1b32b86407d04358ea11d2a769441cc83448b`  
		Last Modified: Mon, 05 Apr 2021 20:28:53 GMT  
		Size: 29.2 MB (29189800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2021b77444a8df4b69ff975ff9dd2798830eec48032954fb3015d3aa2ab89b9b`  
		Last Modified: Mon, 05 Apr 2021 20:28:49 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
