## `ruby:alpine`

```console
$ docker pull ruby@sha256:aba0ca611f01dd94ae9b0c73adef47e9e286dbc9167b1bd4bc2bc592a1f3f07d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ruby:alpine` - linux; amd64

```console
$ docker pull ruby@sha256:742b443a544b78834d44c4d0f18c3a1cbe81186a448d161e969f00cace2937aa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.7 MB (32668552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46c4b23869552a1a46bcf8aca21000ef715a44f3440565d52eb77f54756f0de`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:07:29 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 15 Apr 2021 03:07:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 15 Apr 2021 03:07:31 GMT
ENV LANG=C.UTF-8
# Thu, 15 Apr 2021 03:07:32 GMT
ENV RUBY_MAJOR=3.0
# Thu, 15 Apr 2021 03:07:32 GMT
ENV RUBY_VERSION=3.0.1
# Thu, 15 Apr 2021 03:07:32 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Thu, 15 Apr 2021 03:11:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 15 Apr 2021 03:11:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 15 Apr 2021 03:11:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 15 Apr 2021 03:11:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Apr 2021 03:11:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 15 Apr 2021 03:11:27 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a867505730167ce0636f0811cb765ebbde11bf979c1a9839f6915f2fc3b85b`  
		Last Modified: Thu, 15 Apr 2021 03:39:41 GMT  
		Size: 1.2 MB (1218679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c77620f6108dc0610cba72f77d68c271fb1b14cb0800a7a8b6aaeb8950fec9`  
		Last Modified: Thu, 15 Apr 2021 03:39:40 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637b907898172b7e027230e03a29f1218385572592714311c94c0c8f92d31d6f`  
		Last Modified: Thu, 15 Apr 2021 03:39:44 GMT  
		Size: 28.6 MB (28637510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a4d9a928ae550ce5d89bb0fc040e2df69faba726fdf300947fe6d0b141961`  
		Last Modified: Thu, 15 Apr 2021 03:39:40 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine` - linux; arm variant v6

```console
$ docker pull ruby@sha256:e0b6c77b678e638d2b229937444863dda647b344be6082cdc93aeadb587e8c21
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31294363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f609af90114c063e3dd57a90e5318f92a81a7b0d48a7ee1b172792e6105b6f`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:04:20 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 03:04:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 03:04:25 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 03:04:26 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 18:03:25 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 18:03:25 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 18:07:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 18:07:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 18:07:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 18:07:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 18:07:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 18:07:19 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e365e22ff88eced8f3c43f4bf5dc34311ced0edc76f4653af43dd8fa32c80702`  
		Last Modified: Thu, 01 Apr 2021 03:41:58 GMT  
		Size: 1.1 MB (1070949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bc1fce2fc936a17ba6325794ffefc36853244a2431958fed7fedbfb97460a4`  
		Last Modified: Thu, 01 Apr 2021 03:41:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4106a230e3c0020cbe209647fc8703cb8db494368b54fa1e1c5f4e5bc14bc7a2`  
		Last Modified: Mon, 05 Apr 2021 18:40:01 GMT  
		Size: 27.6 MB (27600903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5edd264c30e3d3ea2cb4b965e3f860c0014bfb0995f8a6fde71988703939d9ca`  
		Last Modified: Mon, 05 Apr 2021 18:39:54 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine` - linux; arm variant v7

```console
$ docker pull ruby@sha256:3e56dab385bf7e45c20fe2baaff2a5d8619b23d77de558ddc1dadd236040879d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30857353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76711b84328cf82a93590b51856dcdb52d977b8319ad016a874967bc56de97ae`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 06:22:17 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 06:22:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 06:22:25 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 06:22:27 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 18:35:28 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 18:35:29 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 18:38:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 18:38:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 18:38:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 18:38:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 18:38:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 18:38:49 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b29c64cdb8201c52135ac3c766242f25b331b5b4e83f88d1074b39b2546caef`  
		Last Modified: Thu, 01 Apr 2021 06:55:21 GMT  
		Size: 996.6 KB (996621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4defffef6c6fadec8bbce68e22061407956ccef29aa06432604c28ec68d8b448`  
		Last Modified: Thu, 01 Apr 2021 06:55:20 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289d5977b905629b0e0e2d9a656757e36ab54c53738c00b85bc44032c3fee8cf`  
		Last Modified: Mon, 05 Apr 2021 19:41:52 GMT  
		Size: 27.4 MB (27436228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5f249fb62b5b4fda9fc8b5e257b6c2720e972908df850445c452673968b492`  
		Last Modified: Mon, 05 Apr 2021 19:41:41 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:9f58fad69067dafb6279c3e6742c9259339a13a895f9e3c8c9bd226de74bf380
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32264320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06d9bd9424a2ea56bb36f3e0a01e27b66c7fecc8aab171817b965bc73098b2fe`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 11:22:47 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 11:22:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 11:22:51 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 11:22:52 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 21:42:00 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 21:42:01 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 21:45:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 21:45:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 21:45:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 21:45:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 21:45:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 21:45:18 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ad87e22eb6e6823616c9c7d49b75e77927a94fb70ad219aad372b48d4e912a`  
		Last Modified: Thu, 01 Apr 2021 11:53:53 GMT  
		Size: 1.2 MB (1221079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36680847d0d64157ef36dc0019fd9024c2685cf93ecb0d81eacd38dd66765340`  
		Last Modified: Thu, 01 Apr 2021 11:53:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f60a633244c49d33477fa670b8433a9e78b650eb477e54f94e8340cebaba51`  
		Last Modified: Mon, 05 Apr 2021 22:45:28 GMT  
		Size: 28.3 MB (28330924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:777f572e8a31f6ab5a8ea408f1bcc589f6044d46b5f00ca5e64046c3de4af9bc`  
		Last Modified: Mon, 05 Apr 2021 22:45:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine` - linux; 386

```console
$ docker pull ruby@sha256:6f18619c0b0370545480d33ac7d2a2ba57218504c3b13a549d5972d01fcd6e76
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31797078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32f596f2dad9b8c379ce38a5543f04fc7ed80b78596adeabdffc3d2b3221193`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 23:55:30 GMT
RUN apk add --no-cache 		gmp-dev
# Wed, 31 Mar 2021 23:55:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 31 Mar 2021 23:55:32 GMT
ENV LANG=C.UTF-8
# Wed, 31 Mar 2021 23:55:32 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 18:44:44 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 18:44:45 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 18:48:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 18:48:56 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 18:48:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 18:48:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 18:48:58 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 18:48:58 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3f50d953b6447de874c74f6f24c01f9db5f651cbc744d6bea0fc813e020a95`  
		Last Modified: Thu, 01 Apr 2021 00:35:20 GMT  
		Size: 1.3 MB (1257444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4caf3f7461bbef426586b45a0f318a08668425242d5e555a8108c49396c83c5`  
		Last Modified: Thu, 01 Apr 2021 00:35:20 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d54b9048c46230642a086ad7a6d56e0d54be2db5f55f35f09b2102fae2fcfe`  
		Last Modified: Mon, 05 Apr 2021 20:11:39 GMT  
		Size: 27.7 MB (27720437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b5ba8914cf42d96e3ad56389ab2269c9aad7552838ba7385e35ac024d9759c`  
		Last Modified: Mon, 05 Apr 2021 20:11:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine` - linux; ppc64le

```console
$ docker pull ruby@sha256:fdc8493c8d80c3c90d84c0dac67fbfa02a51b4ad11608eee1c351ef10ad9c5f7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.2 MB (33174458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4ce9fd96a928dc4ceb92aa152589fe81be675329e5eaa5f0b20aa8c3b2f5188`
-	Default Command: `["irb"]`

```dockerfile
# Wed, 31 Mar 2021 18:55:41 GMT
ADD file:1dd3315eb685a1b6729efb6f5b634e414f3da0f065078952bc6c0339dc09512d in / 
# Wed, 31 Mar 2021 18:55:49 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 18:21:24 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 18:21:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 18:21:44 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 18:21:50 GMT
ENV RUBY_MAJOR=3.0
# Mon, 05 Apr 2021 18:52:23 GMT
ENV RUBY_VERSION=3.0.1
# Mon, 05 Apr 2021 18:52:35 GMT
ENV RUBY_DOWNLOAD_SHA256=d06bccd382d03724b69f674bc46cd6957ba08ed07522694ce44b9e8ffc9c48e2
# Mon, 05 Apr 2021 18:55:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 18:56:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 18:56:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 18:56:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 18:56:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 18:56:53 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:dc4792b25345295bf964e1db1bceedb2338bfad8f0fb64f0cc07b152df9aef84`  
		Last Modified: Wed, 31 Mar 2021 18:57:19 GMT  
		Size: 2.8 MB (2813219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2844bec71be93b6a990c709d31b39d16a54da1edeb0058f3c10de9975c01bc40`  
		Last Modified: Thu, 01 Apr 2021 19:01:50 GMT  
		Size: 1.3 MB (1302664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db92fb641ba2e00ba2604ba6191f4af3cd2b087445ea604400878d3b08d41689`  
		Last Modified: Thu, 01 Apr 2021 19:01:49 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4d9fd0c7a9b72b27e334dc2fa621b840cb592bd0bc121ca07021444b18d9bb`  
		Last Modified: Mon, 05 Apr 2021 20:28:21 GMT  
		Size: 29.1 MB (29058179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67a5d4f23adc4900dabc4adc0f6b546f94394674a6247086c8e2fc93d52c835`  
		Last Modified: Mon, 05 Apr 2021 20:28:16 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:alpine` - linux; s390x

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
