## `ruby:3-alpine3.12`

```console
$ docker pull ruby@sha256:c7a5a092e3c460284f456162ad23a3c88a25373c8e4d6fd66bf70372f765ac61
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
$ docker pull ruby@sha256:10415c86802f78d316e4dd5f24d64a755769c6593adde86554e0383fed246857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31449397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3215bb7c039c25cab3a10c0afb0f753456d268179d0e56cefcd412e9fafb40d3`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 05:38:24 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 15 Apr 2021 05:38:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 15 Apr 2021 05:38:27 GMT
ENV LANG=C.UTF-8
# Thu, 15 Apr 2021 05:38:27 GMT
ENV RUBY_MAJOR=3.0
# Thu, 15 Apr 2021 05:38:28 GMT
ENV RUBY_VERSION=3.0.1
# Thu, 15 Apr 2021 05:38:29 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Thu, 15 Apr 2021 05:42:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 15 Apr 2021 05:42:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 15 Apr 2021 05:42:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 15 Apr 2021 05:42:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Apr 2021 05:42:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 15 Apr 2021 05:42:10 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7655d9df4646c33ccfa32156b446cd8b152c14f060e96ce39527c5542f0190cc`  
		Last Modified: Thu, 15 Apr 2021 06:10:44 GMT  
		Size: 1.1 MB (1050136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159eeaab42659c5e68ddaf80d206c80992059bb2fddf50f1e086bd4a95f113f`  
		Last Modified: Thu, 15 Apr 2021 06:10:43 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b76961d07ee4ab15f1e1d34f3e764e1653164cc32eddc6f9807c4015ff26b5`  
		Last Modified: Thu, 15 Apr 2021 06:10:50 GMT  
		Size: 27.8 MB (27793613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9570c7c08cf2a93616f26a85b60599c1a697f8c7c9f854d0990607577d969c8`  
		Last Modified: Thu, 15 Apr 2021 06:10:43 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; arm variant v7

```console
$ docker pull ruby@sha256:34083b1195ae29ced6c31b81986a3767226137275397fdb5d35ccf624579f2b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31002548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4b7df73114f3388a57c1e4cac8d6b674da17600bdda578109a8ec12ba3bd16`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:03:04 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 15 Apr 2021 06:03:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 15 Apr 2021 06:03:06 GMT
ENV LANG=C.UTF-8
# Thu, 15 Apr 2021 06:03:07 GMT
ENV RUBY_MAJOR=3.0
# Thu, 15 Apr 2021 06:03:08 GMT
ENV RUBY_VERSION=3.0.1
# Thu, 15 Apr 2021 06:03:09 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Thu, 15 Apr 2021 06:06:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 15 Apr 2021 06:06:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 15 Apr 2021 06:06:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 15 Apr 2021 06:06:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Apr 2021 06:06:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 15 Apr 2021 06:06:09 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09480fc10c010f540a110f70c0f39834f2b77078f297eb21a107ca2f24476e34`  
		Last Modified: Thu, 15 Apr 2021 06:33:24 GMT  
		Size: 977.0 KB (976959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f632d30be12418a01478f8173ef83a560ee866cfca3cdc19b402528b07f109c`  
		Last Modified: Thu, 15 Apr 2021 06:33:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5156ee0b9b9e67c38f176f19356281002bf019a45914eff0c24eaa314423e297`  
		Last Modified: Thu, 15 Apr 2021 06:33:31 GMT  
		Size: 27.6 MB (27616015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9a53fd146e8c10e60acedeec45bd997ca2816b5b922fdaea409a505a38ed6b`  
		Last Modified: Thu, 15 Apr 2021 06:33:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:5ba4b2400731ae2926015ccf4a470a84523017341f9704c26ed1e90352c5d832
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32430859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fdbd5623cb2b5af16d4c1912c33769decf8883d4205ecd149645b63399ba08`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Fri, 28 May 2021 11:35:18 GMT
RUN apk add --no-cache 		gmp-dev
# Fri, 28 May 2021 11:35:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 28 May 2021 11:35:19 GMT
ENV LANG=C.UTF-8
# Fri, 28 May 2021 11:35:19 GMT
ENV RUBY_MAJOR=3.0
# Fri, 28 May 2021 11:35:19 GMT
ENV RUBY_VERSION=3.0.1
# Fri, 28 May 2021 11:35:19 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Fri, 28 May 2021 11:38:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 28 May 2021 11:38:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 28 May 2021 11:38:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 28 May 2021 11:38:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 28 May 2021 11:38:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 28 May 2021 11:38:05 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8494ae4cf9ff7841813e4c63a745cfa80eb141e8fe233779a888b432d04c8bd5`  
		Last Modified: Fri, 28 May 2021 12:22:03 GMT  
		Size: 1.2 MB (1207165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ce95f592ff7727675acb3bf60261d163f1d5d31ee1b27abba3519eb0573a32`  
		Last Modified: Fri, 28 May 2021 12:22:03 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf1482e52fc7e9462eeecd05fe151919b0fa5e269a18ce88857979377eb198e8`  
		Last Modified: Fri, 28 May 2021 12:22:06 GMT  
		Size: 28.5 MB (28512604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9476831e71d34cd1538bb33f299982150e0bd64d17691201f2ff6cf9534131fe`  
		Last Modified: Fri, 28 May 2021 12:22:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; 386

```console
$ docker pull ruby@sha256:eeb358f996a60aed8878a00025e8a1d8c15dbdf0fdf4fa5736adeb4f0c04c1b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31994642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be473f8e3179b2114406a4246cdd7db1b165ee21b6baf89414233afb9535765`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 06:51:19 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 15 Apr 2021 06:51:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 15 Apr 2021 06:51:20 GMT
ENV LANG=C.UTF-8
# Thu, 15 Apr 2021 06:51:20 GMT
ENV RUBY_MAJOR=3.0
# Thu, 15 Apr 2021 06:51:21 GMT
ENV RUBY_VERSION=3.0.1
# Thu, 15 Apr 2021 06:51:21 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Thu, 15 Apr 2021 06:54:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 15 Apr 2021 06:54:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 15 Apr 2021 06:54:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 15 Apr 2021 06:54:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Apr 2021 06:54:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 15 Apr 2021 06:54:46 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5726daf19bd6a37033bbfbdf7c34c9ad71e6ad233faad730dad942067353eec`  
		Last Modified: Thu, 15 Apr 2021 07:18:25 GMT  
		Size: 1.2 MB (1236726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a23379d9351d8d00f5c5ae437da763d1c50b130a4c72dd9dbad54ea530faea`  
		Last Modified: Thu, 15 Apr 2021 07:18:26 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b591bb5a5886bdaba5d63a737e200f615a8b28e703fb1cc29e45a7758d0e958`  
		Last Modified: Thu, 15 Apr 2021 07:18:28 GMT  
		Size: 28.0 MB (27961726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0151469497aedcc1f3ef82845259729b3272819968f87c12622d76df03c42b09`  
		Last Modified: Thu, 15 Apr 2021 07:18:25 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.12` - linux; ppc64le

```console
$ docker pull ruby@sha256:bfd00047ba27c129fcf93e4a2a3e7a148564fe6e9d74b06c906fc42e34038d27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33280158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1973bad44a920c9a47132d031259d126a43fbc1ee5321ce63bec58cb0d8e46b6`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 07:19:37 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 15 Apr 2021 07:19:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 15 Apr 2021 07:19:53 GMT
ENV LANG=C.UTF-8
# Thu, 15 Apr 2021 07:19:58 GMT
ENV RUBY_MAJOR=3.0
# Thu, 15 Apr 2021 07:20:05 GMT
ENV RUBY_VERSION=3.0.1
# Thu, 15 Apr 2021 07:20:09 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Thu, 15 Apr 2021 07:23:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 15 Apr 2021 07:23:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 15 Apr 2021 07:23:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 15 Apr 2021 07:23:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Apr 2021 07:23:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 15 Apr 2021 07:24:00 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe4403e0c97507760254cea7ebdf47a4eacb1f166709c8c7a153a70ca6a1272`  
		Last Modified: Thu, 15 Apr 2021 07:52:45 GMT  
		Size: 1.3 MB (1282985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9599e1a2e62814d61cf5ad119edde77075d4d11c84921ebd6f721dee12f08097`  
		Last Modified: Thu, 15 Apr 2021 07:52:44 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebd4a58c92d88027b7eca017be60bc215b3e92a940ca35d38144f10424019dd`  
		Last Modified: Thu, 15 Apr 2021 07:52:49 GMT  
		Size: 29.2 MB (29190023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52a26c6afecebadd00a1ceedf50544e3576441e80a72ecf26c243a17abbebb6`  
		Last Modified: Thu, 15 Apr 2021 07:52:44 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
