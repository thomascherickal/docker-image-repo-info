## `ruby:3-alpine3.17`

```console
$ docker pull ruby@sha256:151d31fc487a68d1027655956a2d595e55c5584beb578916c401fb9778c13ad3
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

### `ruby:3-alpine3.17` - linux; amd64

```console
$ docker pull ruby@sha256:5e11b2787dfc1891744171ba0112435d2fcd2d4b13019e57d0696b1bf360bea0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39322970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc069cfc4113d49e432d6e44330a87cb385377354961c12ba4db51058dafc542`
-	Default Command: `["irb"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:58 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Thu, 30 Nov 2023 23:22:59 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:40:10 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 01 Dec 2023 05:40:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 01 Dec 2023 05:40:10 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:46:20 GMT
ENV RUBY_MAJOR=3.2
# Fri, 01 Dec 2023 05:46:20 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 01 Dec 2023 05:46:20 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 01 Dec 2023 05:49:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 01 Dec 2023 05:49:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 01 Dec 2023 05:49:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 01 Dec 2023 05:49:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 01 Dec 2023 05:49:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 01 Dec 2023 05:49:08 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483120b6e93a3f0c99a3333bebde74a4236a5b2346de09fde22b7f9c8328a74e`  
		Last Modified: Fri, 01 Dec 2023 05:57:40 GMT  
		Size: 4.1 MB (4126455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8014301d882d8224ffe51e7659dd0acf2e5e95eea7304cebbb9c37ab2b3ad9`  
		Last Modified: Fri, 01 Dec 2023 05:57:39 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401feed4d188acdc73d3cb7d2807e5ed9960b1670e441a43271c3b099f498280`  
		Last Modified: Fri, 01 Dec 2023 05:58:22 GMT  
		Size: 31.8 MB (31816796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08c21e8ff8bf48d4cfd40daa0fa6a4ad0bf039df1f6d812e382dfc2a8f8798d`  
		Last Modified: Fri, 01 Dec 2023 05:58:19 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.17` - linux; arm variant v6

```console
$ docker pull ruby@sha256:cf5d23beed285cbbd893547116502f7154f089d64dbf412a0546630f7c0fb4f4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36938443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:252bd90ca9adb0fc64c6cc477e34ee01854a40469e011776caceb32df4aa0c89`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:46:42 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 00:46:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 00:46:44 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 00:53:54 GMT
ENV RUBY_MAJOR=3.2
# Sat, 21 Oct 2023 00:53:54 GMT
ENV RUBY_VERSION=3.2.2
# Sat, 21 Oct 2023 00:53:54 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 21 Oct 2023 00:55:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 00:55:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 00:55:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 00:55:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:55:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 00:55:59 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8778eaf311f49cd974a66c8163d1d4c22644058e1cc7bc391294035bb8eb8d88`  
		Last Modified: Sat, 21 Oct 2023 01:04:20 GMT  
		Size: 3.9 MB (3868092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a4bdd19ea5dfbfa96d128b6fcb0cbb655877e0f5719dcbacd35c851622a1fe`  
		Last Modified: Sat, 21 Oct 2023 01:04:19 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1219128b3562579f5133697e29b18abc8451aafabb97f87e1fa63b1a01eb2bf`  
		Last Modified: Sat, 21 Oct 2023 01:05:01 GMT  
		Size: 30.0 MB (29957505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac656aac345a6bf4c60da0383db057582f677f0948625b827c4767308e533599`  
		Last Modified: Sat, 21 Oct 2023 01:04:58 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.17` - linux; arm variant v7

```console
$ docker pull ruby@sha256:19a0e965485705b9a0b7d6ed99eb6e22ea8e1f69a3c9f3e29c9688d36e5bf851
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.3 MB (36313008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54cb27d26d21c0500e5e938712cd5291ded4a790002519905877b6592a894265`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:29 GMT
ADD file:7f36c30ba2b714d09a8650dba1545abdf892443dadbe9113b9a166b84ba7ac3f in / 
# Mon, 07 Aug 2023 19:57:29 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:10:20 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 01:10:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 01:10:20 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 01:18:08 GMT
ENV RUBY_MAJOR=3.2
# Sat, 21 Oct 2023 01:18:08 GMT
ENV RUBY_VERSION=3.2.2
# Sat, 21 Oct 2023 01:18:08 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 21 Oct 2023 01:20:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 01:20:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 01:20:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 01:20:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 01:20:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 01:20:23 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b82e4fd40279a40aa2eecd301fabb2dca254727cc09daa8d0caf69ac28c44af1`  
		Last Modified: Mon, 07 Aug 2023 19:58:08 GMT  
		Size: 2.9 MB (2869425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f18b31907d8c8994599107b563dde6f5c641aac2f0b3f8e538839087b24d672`  
		Last Modified: Sat, 21 Oct 2023 01:29:55 GMT  
		Size: 3.7 MB (3722659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a9975c527b8152bcd66ce03c3c7b2c30975c3cf95ae3c990216b4b25a61c1c`  
		Last Modified: Sat, 21 Oct 2023 01:29:54 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bb432a5fdcdf5c681084d02ff20142424a2062c3d54b0ad4b6999e6a235651`  
		Last Modified: Sat, 21 Oct 2023 01:30:43 GMT  
		Size: 29.7 MB (29720527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc1f88a6c28875ae781cfaa85b0fb45ac2cd2cbb891379361fee94b17ba3c6a`  
		Last Modified: Sat, 21 Oct 2023 01:30:39 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull ruby@sha256:0216cd39369be27da02d195d4508d71578834c5720977a11997ddd1e30e2e01c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.2 MB (41176631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3cfc79c1b57a2bc14584b729aeebcc6390a5474f87a499df02321cca08f7adc`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:43:53 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 02:43:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 02:43:54 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 02:50:43 GMT
ENV RUBY_MAJOR=3.2
# Sat, 21 Oct 2023 02:50:43 GMT
ENV RUBY_VERSION=3.2.2
# Sat, 21 Oct 2023 02:50:43 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 21 Oct 2023 02:52:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 02:52:37 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 02:52:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 02:52:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 02:52:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 02:52:38 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cbd5ecc1f80385af26443ae4918fc41f9b4d918f88509d6bb75560911ae423`  
		Last Modified: Sat, 21 Oct 2023 02:59:11 GMT  
		Size: 4.1 MB (4119073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77544063d4b7a17343cf4f8f7d9120cfa8c432c336879220f3f8502e7108155`  
		Last Modified: Sat, 21 Oct 2023 02:59:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a292ce0179149c0b9b0c96d55ed54ec48dcee428ad070b69875bfa4c7657836`  
		Last Modified: Sat, 21 Oct 2023 02:59:55 GMT  
		Size: 33.8 MB (33798870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b461cd2109c3f712567085afc91dedda1d28c4aa6f58b54cc9f1668c70fdb2c9`  
		Last Modified: Sat, 21 Oct 2023 02:59:52 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.17` - linux; 386

```console
$ docker pull ruby@sha256:f97808f68ad32f67e624a7ab15cf9eed868815ed76b262b8d488da5f3cbdb946
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37693874 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50797e9249b47e10f8cf844b91fd6ea0b249e33ef63056d4d6372688e3337d12`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:33:15 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 01:33:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 01:33:16 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 01:43:50 GMT
ENV RUBY_MAJOR=3.2
# Sat, 21 Oct 2023 01:43:50 GMT
ENV RUBY_VERSION=3.2.2
# Sat, 21 Oct 2023 01:43:50 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 21 Oct 2023 01:47:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 01:47:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 01:47:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 01:47:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 01:47:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 01:47:42 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302694c6cea03cca65b4faf48df4f5cfb6a12c0e500361c79d2cfb14cbc9885a`  
		Last Modified: Sat, 21 Oct 2023 02:01:54 GMT  
		Size: 4.2 MB (4196080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a8a4be4a0dbeef98268fa348a21fd5860556760b330d2d2dde2185d63fd749`  
		Last Modified: Sat, 21 Oct 2023 02:01:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b95d35154edb7573bfd3345a3b765e7c0e31f156b854d86d7450648b8fbaeb0`  
		Last Modified: Sat, 21 Oct 2023 02:02:41 GMT  
		Size: 30.1 MB (30083619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab750a3e6e9fab47f323cd2c98239e053a663a943333cbd66fc636b0509b96e2`  
		Last Modified: Sat, 21 Oct 2023 02:02:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.17` - linux; ppc64le

```console
$ docker pull ruby@sha256:0bed2ef1d0748e030be331a3ac19e21ed4fc8ef83c2e4b58076ab9a8172e5239
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39055174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c107fff57db187d60f886e2450274335c38b2f3742ef69c044c83140f0c15262`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:53:18 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 00:53:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 00:53:19 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 01:01:12 GMT
ENV RUBY_MAJOR=3.2
# Sat, 21 Oct 2023 01:01:12 GMT
ENV RUBY_VERSION=3.2.2
# Sat, 21 Oct 2023 01:01:13 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 21 Oct 2023 01:03:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 01:03:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 01:03:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 01:03:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 01:03:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 01:03:23 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b760dabc92bd519ca870ca0c07a6b178e56946bb50b81290cdcf4fa51130f54`  
		Last Modified: Sat, 21 Oct 2023 01:11:27 GMT  
		Size: 4.3 MB (4282013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209278cff3c8219a6a9fa31189ab43b49d4d49d5af5d50076fdc0152eacd1969`  
		Last Modified: Sat, 21 Oct 2023 01:11:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a310b1d912c95aebdde3925d0cd2a5c2db28160a21d1a4c475bbab3e25d868f1`  
		Last Modified: Sat, 21 Oct 2023 01:12:12 GMT  
		Size: 31.4 MB (31381415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852080e398305e8565d5fddfabb5c3ef187dcb23025865988992481f478985fd`  
		Last Modified: Sat, 21 Oct 2023 01:12:09 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ruby:3-alpine3.17` - linux; s390x

```console
$ docker pull ruby@sha256:04d3e8993bbf822a83d03c99db5928992707cfce8474c99a1bd1f8591f60a1dd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (37984268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:479cc675394f37bde245914c2d62b16118c614a70f1418b7bafcc4c3d702556e`
-	Default Command: `["irb"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:48:18 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 00:48:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 00:48:19 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 00:55:10 GMT
ENV RUBY_MAJOR=3.2
# Sat, 21 Oct 2023 00:55:10 GMT
ENV RUBY_VERSION=3.2.2
# Sat, 21 Oct 2023 00:55:10 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 21 Oct 2023 00:57:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='95427cb0592e32ed39c8bd522fe2a40a746ba07afb8149f91e936cddb4d6eeac' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.25.1/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='7855404cdc50c20040c743800c947b6f452490d47f8590a4a83bc6f75d1d8eda' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.66.0' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 00:57:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 00:57:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 00:57:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:57:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 00:57:17 GMT
CMD ["irb"]
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b11aafd2203b5aab7ce5c760684b9328d1a04357483a48933382f538b7a08e`  
		Last Modified: Sat, 21 Oct 2023 01:06:15 GMT  
		Size: 4.2 MB (4199177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b62af3780bf813ebd28108bcab425ee8492575cd99bc16cf9ef92736bb8684`  
		Last Modified: Sat, 21 Oct 2023 01:06:14 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee2ebd64690824d5496e7b32c77a4bd985ef20c7344029e2688ea35f8c0360`  
		Last Modified: Sat, 21 Oct 2023 01:06:57 GMT  
		Size: 30.6 MB (30608721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18436dd8900751e2e38b5ffc41d673787184fa78d1af16aa3b3e88a27692a135`  
		Last Modified: Sat, 21 Oct 2023 01:06:54 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
