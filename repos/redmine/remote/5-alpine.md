## `redmine:5-alpine`

```console
$ docker pull redmine@sha256:eadc31a33f113c6c7cd84c5838c6a16c7c2f39eefd1181f3db481a3d20ec7377
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	unknown; unknown
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `redmine:5-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:ddfa98a0682593417fe87055e9a699620fdfb5fb13316a2601ab6f41cd98cd74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.2 MB (200188575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64d8fc1b9eea208c08743f285eecccd6860ad4300873e39317c77c78efb68885`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:37:01 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 01 Dec 2023 05:37:01 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 01 Dec 2023 05:37:02 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 05:43:26 GMT
ENV RUBY_MAJOR=3.2
# Fri, 01 Dec 2023 05:43:26 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 01 Dec 2023 05:43:26 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 09 Dec 2023 06:32:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 09 Dec 2023 06:32:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 09 Dec 2023 06:32:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 09 Dec 2023 06:32:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 06:32:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 09 Dec 2023 06:32:44 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RAILS_ENV=production
# Tue, 19 Dec 2023 17:42:47 GMT
WORKDIR /usr/src/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
ENV HOME=/home/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_VERSION=5.1.1
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 19 Dec 2023 17:42:47 GMT
COPY docker-entrypoint.sh / # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 17:42:47 GMT
EXPOSE map[3000/tcp:{}]
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cda842cda46f6998263cef8856c3f37cc352155242cdad296bc1c0dff92612e0`  
		Last Modified: Fri, 01 Dec 2023 05:57:26 GMT  
		Size: 4.1 MB (4131408 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:78679cd21b9a9b06ed51b8b7eb5c1ce2721ba6a3fbbfca5c3c6d41d0e9c61858`  
		Last Modified: Fri, 01 Dec 2023 05:57:25 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850e05ff4aa3ec43b53bb22b337abe0e363f0260316a82e2b62c508e940b0754`  
		Last Modified: Sat, 09 Dec 2023 06:39:48 GMT  
		Size: 32.0 MB (31969744 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3be6727859bed14d2238e9dfc80ccc2a7480367aa4b4df42b45ccb4b1423cec0`  
		Last Modified: Sat, 09 Dec 2023 06:39:45 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e1d3012a80bec3dfe73d1896b474d87bdabe6d819d30a3180d28e11140d8c7c0`  
		Last Modified: Tue, 19 Dec 2023 22:53:59 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c7c40f0eb01bdd25b99d26f0937e5aacabbb7ab4fe8bd99717b9538f013a9eeb`  
		Last Modified: Tue, 19 Dec 2023 22:54:01 GMT  
		Size: 87.3 MB (87313659 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:023c788cd9ff520eb21bf46bf89891c98599b8c18f9db670760ecde08f70e012`  
		Last Modified: Tue, 19 Dec 2023 22:54:00 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d27412f0e9b961f575a7d122e7aaa7a434df4e6c566d0d99217393f217b0aa5b`  
		Last Modified: Tue, 19 Dec 2023 22:54:00 GMT  
		Size: 124.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:69a71cf7f6b8daa751c226b34cba16d0085825549a4ad7e688f380fafa50c3f8`  
		Last Modified: Tue, 19 Dec 2023 22:54:01 GMT  
		Size: 3.2 MB (3236779 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d33aa4bb16251b033abfd53b3c05ff307290e58fa006ec64476e7e541f16fc48`  
		Last Modified: Tue, 19 Dec 2023 22:54:03 GMT  
		Size: 70.1 MB (70130690 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:758b1c7bcd30612ccab3f353560a1d5df90728f48a6bf24c8eb9f0972047502c`  
		Last Modified: Tue, 19 Dec 2023 22:54:01 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:ed7c720734841340c70a3c42a2d751c2be3a8792ae00e81502481a76aa4fe47c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4608323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1d21b96a280e684880c8ecf6c03ab2e56328d78ed64c5825ee4c476d63d766`

```dockerfile
```

-	Layers:
	-	`sha256:4a3c6f987aceec8330e350b0ba974c1689baa67f80032d4910ed9a41b063a577`  
		Last Modified: Tue, 19 Dec 2023 22:53:59 GMT  
		Size: 4.6 MB (4573339 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d4f51c629726b8614de8f4924bb675d943657cbd55e3d3f66aa5f3ff4f66316`  
		Last Modified: Tue, 19 Dec 2023 22:53:59 GMT  
		Size: 35.0 KB (34984 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:cd03efa10c318c4af9a7f6d9b7152d109aaca79ef5a2213ff590798de9ebd918
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.8 MB (190753738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933041c4fca6b06f07cd854a61967e8c3d2acaaed2dc17b77d788ebe4fed4903`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 11:17:45 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 01 Dec 2023 11:17:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 01 Dec 2023 11:17:46 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 11:23:14 GMT
ENV RUBY_MAJOR=3.2
# Fri, 01 Dec 2023 11:23:14 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 01 Dec 2023 11:23:14 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Fri, 08 Dec 2023 22:10:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 08 Dec 2023 22:10:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 08 Dec 2023 22:10:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 08 Dec 2023 22:10:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 08 Dec 2023 22:10:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 08 Dec 2023 22:10:23 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RAILS_ENV=production
# Tue, 19 Dec 2023 17:42:47 GMT
WORKDIR /usr/src/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
ENV HOME=/home/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_VERSION=5.1.1
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 19 Dec 2023 17:42:47 GMT
COPY docker-entrypoint.sh / # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 17:42:47 GMT
EXPOSE map[3000/tcp:{}]
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e26cf146b5758871f70fdcf7cddfabfd98ae2c03f59fbf514087237074f7009d`  
		Last Modified: Fri, 01 Dec 2023 11:35:55 GMT  
		Size: 3.8 MB (3807454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:71b640c72cd556ccc0b798019f6de6286640a7d6b9f2792e33d1d6f8f4ebb1ea`  
		Last Modified: Fri, 01 Dec 2023 11:35:54 GMT  
		Size: 223.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7dbadd5b31b5616b5fccf4337438c1649a1e5e7f4291e95b502dfcda3eefafd4`  
		Last Modified: Fri, 08 Dec 2023 22:15:05 GMT  
		Size: 28.1 MB (28106403 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e265a668d726b2f458cb25df9ff78d68d4c20cd24d6d6b1a622d8357d2a42ba`  
		Last Modified: Fri, 08 Dec 2023 22:15:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7a1b95b437ca196a17f3a9c0c7450857bc3a0007e23d97b3ea639991643bbb51`  
		Last Modified: Tue, 19 Dec 2023 23:22:04 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5194e87bf0298e0a3aa2d3803a6f4f08f202ef1be1cb4cab6fe09eba47f94577`  
		Last Modified: Tue, 19 Dec 2023 23:22:07 GMT  
		Size: 82.9 MB (82897149 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fe19916a771bbb366aa390fbe11f77c28b359915d7a6b74c0c249a61373a86c1`  
		Last Modified: Tue, 19 Dec 2023 23:22:05 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c168058c503b183072b09a656b0a7877aab69c44f826ad936e867409dc06bc3b`  
		Last Modified: Tue, 19 Dec 2023 23:22:05 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1530ff9bf742182f89ce02cd1d73bd00610ca036eb49475a036abb3f1bb82e3b`  
		Last Modified: Tue, 19 Dec 2023 23:22:06 GMT  
		Size: 3.2 MB (3236814 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:51a890af866ec082332961abc82da4c2e4df66e77b80c3d74c62b7fff5260dbb`  
		Last Modified: Tue, 19 Dec 2023 23:22:09 GMT  
		Size: 69.6 MB (69555175 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc4d8aad9b559132123030d71a27cb25a1207c6b3429915824f426eae0f8fcad`  
		Last Modified: Tue, 19 Dec 2023 23:22:06 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:36f4af6d76b4dfabf3dfb406913aa1dd55ca03dcfa794a90ca4e618296374311
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 KB (34923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1f136a9e2b87eba1ec31dfd4666973885edef13f82856cbe3068e8ea638301b`

```dockerfile
```

-	Layers:
	-	`sha256:6ab8c87dfecb320e8b4eaa7eab8bfc3269f4bd0e39f82f0f33d5d1f2311744c9`  
		Last Modified: Tue, 19 Dec 2023 23:22:04 GMT  
		Size: 34.9 KB (34923 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:8e43def9a6d395b4a85747223b5603e8de14db8d09a6daeea0ef2db6807da27c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.7 MB (204675048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ff642795cc0bcb6f5a47d83344e684b3cec8d7960aaaac95af838e2070b93b2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 27 Nov 2023 21:32:27 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["/bin/sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Mon, 27 Nov 2023 21:32:27 GMT
ENV LANG=C.UTF-8
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_VERSION=3.1.4
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Nov 2023 21:32:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Nov 2023 21:32:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Nov 2023 21:32:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dc6237355c695ee0cfc4c4a82fad8257832e20e08674070310d6b1e12eb1125a`  
		Last Modified: Fri, 01 Dec 2023 09:06:34 GMT  
		Size: 3.7 MB (3717180 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4dd9b67b49d08b167e9cefaf4f2a4fa3517f9af7d695062be7378bb433e8ec02`  
		Last Modified: Fri, 01 Dec 2023 09:06:33 GMT  
		Size: 223.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:248f4d8300899874ce145cb1e444657427bd1da5757a5cdb3312d6c074cce658`  
		Last Modified: Fri, 01 Dec 2023 09:07:58 GMT  
		Size: 28.2 MB (28226663 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:349d5e611e22df19643de291a74434f5c3e85322260c65dd27b9d8d7a7950a3f`  
		Last Modified: Fri, 01 Dec 2023 09:07:55 GMT  
		Size: 173.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a721735a2afa6cb5fa4406afefa621b64988f003530a8f6aa7c4b800e0947f9`  
		Last Modified: Fri, 01 Dec 2023 12:54:40 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:78f86fce5f8a270e0b881f856b777bdfdd87f69f921642d32ac4eb2cf87aa94b`  
		Last Modified: Fri, 01 Dec 2023 12:54:43 GMT  
		Size: 79.3 MB (79331156 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:700b879920d3f1dd2724c67f80ca6426af2b84da86b2202520e56a13e80c0dc0`  
		Last Modified: Fri, 01 Dec 2023 12:54:41 GMT  
		Size: 134.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaeccdf55effbf06db7fbf66905cc65bc78b049354e11981c1d30621c4479d93`  
		Last Modified: Fri, 01 Dec 2023 12:54:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:833a4c6d8ccb9a7f78a2ca045981e9cc179b49787af43edbab6a091d1e88698d`  
		Last Modified: Fri, 01 Dec 2023 12:54:41 GMT  
		Size: 3.2 MB (3236743 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:366a99052e3dea51148ed2d2969468bc1439908bf6520b35ad086ecf730517e7`  
		Last Modified: Fri, 01 Dec 2023 12:54:45 GMT  
		Size: 87.3 MB (87258426 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99ab8f4118ec63de97a68e89eb613c7b6a84999d3f620586dfd389ff61d40246`  
		Last Modified: Wed, 29 Nov 2023 10:43:59 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:5334eb8f6c4d91301835c349037bc32b79a5db5c034b8e263adb3a35411357d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4594507 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad4459a4954d66018b044a06f56e4d346ffd1d5296018715b97cd6366885b7a8`

```dockerfile
```

-	Layers:
	-	`sha256:a599652727c9b16e4bc2135cd3b350e9246b4ff979647e73b013f6835325d96a`  
		Last Modified: Fri, 01 Dec 2023 12:54:39 GMT  
		Size: 4.6 MB (4559369 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:962ed5c82226d3acb9c39c9a806eadb3c224b0028c4b7cf9fa9f93f526be1f5d`  
		Last Modified: Fri, 01 Dec 2023 12:54:39 GMT  
		Size: 35.1 KB (35138 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:74e5f2a806dacd1740dcd99e23eb2853df9799bd7be5c1b87e8145f5645b2357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216505852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef0aa6ae1cbd6395adb70f260baa24f770b9e403e4e8f083a356ce934e1474e4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 27 Nov 2023 21:32:27 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["/bin/sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Mon, 27 Nov 2023 21:32:27 GMT
ENV LANG=C.UTF-8
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_VERSION=3.1.4
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Nov 2023 21:32:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Nov 2023 21:32:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Nov 2023 21:32:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5c85decdc668af8251b680f05f9ea641d60fb2b149e2d5f9b79bb7bfb78686c4`  
		Last Modified: Fri, 01 Dec 2023 09:26:46 GMT  
		Size: 4.1 MB (4061489 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39d853fce498d7a4c191568701422907832f2428c63374c3121dd954b27d02ff`  
		Last Modified: Fri, 01 Dec 2023 09:26:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:834ad69aeb1f9d6007dc04e109e6973b698fd421ae69ebc58de3d744dee8a15f`  
		Last Modified: Fri, 01 Dec 2023 09:27:56 GMT  
		Size: 28.9 MB (28935386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:74e7341b08b7fdc7c50bccd49e505a331684e658220ffbc8038333721ba95b01`  
		Last Modified: Fri, 01 Dec 2023 09:27:54 GMT  
		Size: 176.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd9f640dc9c5045d71511f1c29f82b904f535d5c4e31bf11310d09d35b2d9107`  
		Last Modified: Fri, 01 Dec 2023 14:28:39 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0f0106ea5fc7efdb47a28b2029ba229aaf4b1365e4dfbb801e478d54e5ed2322`  
		Last Modified: Fri, 01 Dec 2023 14:28:42 GMT  
		Size: 86.8 MB (86780105 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5615be3ac22e586f8b18e73cedbd5e4e6e421b48fdcf2f0f7046777278d29ddf`  
		Last Modified: Fri, 01 Dec 2023 14:28:39 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9bbfdb54c6134f513fec4673c702970c5ba5b31091e8f05c6873d5da89a92407`  
		Last Modified: Fri, 01 Dec 2023 14:28:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df48d908dfb6be550b6537b332b887db9bd5b283e048e71012259f69ba03b192`  
		Last Modified: Fri, 01 Dec 2023 14:28:40 GMT  
		Size: 3.2 MB (3236744 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7b8ac215d51881afedbd72e86d649f58826dd3e807da26828bf23babc7131892`  
		Last Modified: Fri, 01 Dec 2023 14:28:43 GMT  
		Size: 90.2 MB (90155219 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96969b6597bdde4a286f36497462f70b2549ca8c4b6bda57da836a1067d0a2ca`  
		Last Modified: Wed, 29 Nov 2023 06:13:25 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:05d0f338a1d4790c8184c6a0e5ec807c1a0d2a0a153eaf0468ad837fc7745f4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4595101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b935278d42021ca937569ce1ed374e1f059c92341ebe96e88ad050bd94a279e`

```dockerfile
```

-	Layers:
	-	`sha256:1f16b837d96e5f473f805c1201c61be545c49b2da0788bd1d0f0f4c0e6332968`  
		Last Modified: Fri, 01 Dec 2023 14:28:39 GMT  
		Size: 4.6 MB (4560099 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:62e05d6fad32aa73ad10f1aa50a69ebe815ec31b0e35a1bee5d02c0c66e66470`  
		Last Modified: Fri, 01 Dec 2023 14:28:38 GMT  
		Size: 35.0 KB (35002 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-alpine` - linux; 386

```console
$ docker pull redmine@sha256:f1d9d21b54c6bad8f25e1ea2ca9cffd3fea470ff7197338bf58c561f04fedb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.8 MB (192833612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2b32e4ddc0ac933c82ce31e1827df495b8b3afbedfea042b39932f11fe2d841`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:18:19 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 01 Dec 2023 09:18:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 01 Dec 2023 09:18:20 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 09:27:24 GMT
ENV RUBY_MAJOR=3.2
# Fri, 01 Dec 2023 09:27:24 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 01 Dec 2023 09:27:24 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 09 Dec 2023 05:22:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 09 Dec 2023 05:22:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 09 Dec 2023 05:22:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 09 Dec 2023 05:22:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 05:22:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 09 Dec 2023 05:22:05 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RAILS_ENV=production
# Tue, 19 Dec 2023 17:42:47 GMT
WORKDIR /usr/src/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
ENV HOME=/home/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_VERSION=5.1.1
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 19 Dec 2023 17:42:47 GMT
COPY docker-entrypoint.sh / # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 17:42:47 GMT
EXPOSE map[3000/tcp:{}]
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:45857a503bda93ec5f90d6be7019b19325aa1b8ea411d7f0aab7f72def9051ce`  
		Last Modified: Fri, 01 Dec 2023 09:49:41 GMT  
		Size: 4.1 MB (4135966 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c823e4c7827d69cd7daeab903d261be31e7d10229d297ac98f3ccf6910231880`  
		Last Modified: Fri, 01 Dec 2023 09:49:40 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:58e1c84e0942b99db11b93873610b8c57cf4a0eb02179576241a4af5c8fc66ee`  
		Last Modified: Sat, 09 Dec 2023 05:30:42 GMT  
		Size: 27.9 MB (27886732 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4149174558edf4981b1534a763d759d761b8d3ca6f196c69dd7ca71672cd16e7`  
		Last Modified: Sat, 09 Dec 2023 05:30:38 GMT  
		Size: 173.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b7526394aaffe103e152e97799b8a7ec70769d57cc8f5f3c0cedd036312240a`  
		Last Modified: Tue, 19 Dec 2023 22:54:04 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:451c55714933a6d6bd2f4c9db14156cdc2c332fe4ea9bf70c733245528729abb`  
		Last Modified: Tue, 19 Dec 2023 22:54:06 GMT  
		Size: 84.2 MB (84177229 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a436208c095f0cd66e7453e94b7bc745a6c20d59daa7a39dc45ac59064d8cf94`  
		Last Modified: Tue, 19 Dec 2023 22:54:05 GMT  
		Size: 133.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ded75ebc35eaa6601419dcee16846dcc12be2d60e7d4b9c9938af996ad40e90a`  
		Last Modified: Tue, 19 Dec 2023 22:54:06 GMT  
		Size: 124.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8b94a8bff288287fc1eb5696407b2a5c7f937ec9e7ce1cbe8fe0af8a7e5b47e3`  
		Last Modified: Tue, 19 Dec 2023 22:54:06 GMT  
		Size: 3.2 MB (3236839 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7377dac46245bb5c440304b43041f5a735adaa19a2cba51bbcd754d66924b84b`  
		Last Modified: Tue, 19 Dec 2023 22:54:08 GMT  
		Size: 70.2 MB (70154146 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:758b1c7bcd30612ccab3f353560a1d5df90728f48a6bf24c8eb9f0972047502c`  
		Last Modified: Tue, 19 Dec 2023 22:54:01 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:f65f55dcb2d3ed6a0279925ca9ff5f5ec106b533d899af879fe23734ff181063
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 KB (34712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6fe7abe16763bcb7597384c68e1502197d06071d7e523dba552fd903413c3b7`

```dockerfile
```

-	Layers:
	-	`sha256:22e81bc735e839d3071c01b40dd0003645d41b3b33a022b147a9686f72927d5b`  
		Last Modified: Tue, 19 Dec 2023 22:54:04 GMT  
		Size: 34.7 KB (34712 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-alpine` - linux; ppc64le

```console
$ docker pull redmine@sha256:d58977908dd48e033a945601d16b83c7dea24fad1ffd33ca6de839354b14a4bb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.2 MB (226231041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a6f0f286f20f8f64c29d97a47094700cc428fb044d988cf348d9d51474ad205`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 27 Nov 2023 21:32:27 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["/bin/sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Mon, 27 Nov 2023 21:32:27 GMT
ENV LANG=C.UTF-8
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_MAJOR=3.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_VERSION=3.1.4
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 27 Nov 2023 21:32:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 27 Nov 2023 21:32:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Nov 2023 21:32:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:954822bc395e895e7515fe42e29ae0165886e70ac0647e182974a1638e20c4af`  
		Last Modified: Fri, 01 Dec 2023 09:45:01 GMT  
		Size: 4.3 MB (4279318 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db16971a4fb0b6195be4e725c9c3e6b202c09eb8f202a4648f0ba59923e6904c`  
		Last Modified: Fri, 01 Dec 2023 09:44:59 GMT  
		Size: 223.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5655050237e2dd59e14ad3247f0ec3d406ed791a604b6668d32834ee7632f2ef`  
		Last Modified: Fri, 01 Dec 2023 09:46:24 GMT  
		Size: 29.7 MB (29661961 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:843494d201b363d93251fe1e62f79d895301caba96d5f408f1ea6ebbeb35b685`  
		Last Modified: Fri, 01 Dec 2023 09:46:20 GMT  
		Size: 173.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9b7686554a950d570bfe55500657ac5ed768764586a5934b7ea2aa096627be8b`  
		Last Modified: Fri, 01 Dec 2023 14:06:07 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ce7fd9226296cafc0f83f6fccae1771c39e136c2a8059b13a8e3e05967e3475`  
		Last Modified: Fri, 01 Dec 2023 14:06:11 GMT  
		Size: 92.9 MB (92934218 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d7c61a6712471d5233603444f05d92b828d8ea5ceeb78d08e4185f9714e6d8d`  
		Last Modified: Fri, 01 Dec 2023 14:06:07 GMT  
		Size: 134.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:17e76df1a1c0060d2a2b9f8785facc8a33d8d1ba6ff686bac62cf70acd61729f`  
		Last Modified: Fri, 01 Dec 2023 14:06:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:08412366718cf6c43dc487a08f74e86e7f852d18cc9217d96b5b2f5f85c604c4`  
		Last Modified: Fri, 01 Dec 2023 14:06:09 GMT  
		Size: 3.2 MB (3236742 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8a77f2d6db4821814aa5bc484f66e214d2f9d6837e1a607dd0907e8727b68ad`  
		Last Modified: Fri, 01 Dec 2023 14:06:11 GMT  
		Size: 92.8 MB (92766606 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1fc82a26ab76ae65ea372dd0cf157567fc2253e6863d58c2ff93ce206aed2148`  
		Last Modified: Wed, 29 Nov 2023 08:30:34 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:95437964945ca73921f8ea66632e19ff53a45a84b4765f4331983bef8e68e3b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4600577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0373b5f56882e497f251d17c602c39b8962c3ae4ebc65fd087fd64aab8da6219`

```dockerfile
```

-	Layers:
	-	`sha256:71f1b2ea0eeb47bbdcf09262db2148d001eba236d9172ef132292fa445509655`  
		Last Modified: Fri, 01 Dec 2023 14:06:07 GMT  
		Size: 4.6 MB (4565524 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:f803bf2a4f9cddc77214d763c3c5ed21bc908436bf6d36e95321a221001ab815`  
		Last Modified: Fri, 01 Dec 2023 14:06:06 GMT  
		Size: 35.1 KB (35053 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:5-alpine` - linux; s390x

```console
$ docker pull redmine@sha256:5c198d6c62374fc232a66c8c1f8cf016d2b90ec85e0c850196de1ac3be9687a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.3 MB (196336815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd1ef8157bced312f84311be6e3fa130adf2fbc43bfda59c3921ee21e883ff64`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 08:25:08 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 01 Dec 2023 08:25:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 01 Dec 2023 08:25:09 GMT
ENV LANG=C.UTF-8
# Fri, 01 Dec 2023 08:31:00 GMT
ENV RUBY_MAJOR=3.2
# Fri, 01 Dec 2023 08:31:01 GMT
ENV RUBY_VERSION=3.2.2
# Fri, 01 Dec 2023 08:31:01 GMT
ENV RUBY_DOWNLOAD_SHA256=4b352d0f7ec384e332e3e44cdbfdcd5ff2d594af3c8296b5636c710975149e23
# Sat, 09 Dec 2023 01:17:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		rustArch=; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') rustArch='x86_64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/x86_64-unknown-linux-musl/rustup-init'; rustupSha256='7aa9e2a380a9958fc1fc426a3323209b2c86181c6816640979580f62ff7d48d4' ;; 		'aarch64') rustArch='aarch64-unknown-linux-musl'; rustupUrl='https://static.rust-lang.org/rustup/archive/1.26.0/aarch64-unknown-linux-musl/rustup-init'; rustupSha256='b1962dfc18e1fd47d01341e6897cace67cddfabf547ef394e8883939bd6e002e' ;; 	esac; 		if [ -n "$rustArch" ]; then 		mkdir -p /tmp/rust; 				wget -O /tmp/rust/rustup-init "$rustupUrl"; 		echo "$rustupSha256 */tmp/rust/rustup-init" | sha256sum --check --strict; 		chmod +x /tmp/rust/rustup-init; 				export RUSTUP_HOME='/tmp/rust/rustup' CARGO_HOME='/tmp/rust/cargo'; 		export PATH="$CARGO_HOME/bin:$PATH"; 		/tmp/rust/rustup-init -y --no-modify-path --profile minimal --default-toolchain '1.74.1' --default-host "$rustArch"; 				rustc --version; 		cargo --version; 	fi; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 		${rustArch:+--enable-yjit} 	; 	make -j "$(nproc)"; 	make install; 		rm -rf /tmp/rust; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 09 Dec 2023 01:17:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 09 Dec 2023 01:17:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 09 Dec 2023 01:17:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 09 Dec 2023 01:17:16 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 09 Dec 2023 01:17:17 GMT
CMD ["irb"]
# Tue, 19 Dec 2023 17:42:47 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV RAILS_ENV=production
# Tue, 19 Dec 2023 17:42:47 GMT
WORKDIR /usr/src/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
ENV HOME=/home/redmine
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_VERSION=5.1.1
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Tue, 19 Dec 2023 17:42:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 19 Dec 2023 17:42:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 19 Dec 2023 17:42:47 GMT
COPY docker-entrypoint.sh / # buildkit
# Tue, 19 Dec 2023 17:42:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 19 Dec 2023 17:42:47 GMT
EXPOSE map[3000/tcp:{}]
# Tue, 19 Dec 2023 17:42:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9991c3469b380f3a26867a67c79c35e9b27bb8d9ca457e39492c956e4e79428b`  
		Last Modified: Fri, 01 Dec 2023 08:46:29 GMT  
		Size: 4.2 MB (4235380 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e7d78a35833bd8a2f38207becbe1f57b39c418eab98070bfb4179484955a006d`  
		Last Modified: Fri, 01 Dec 2023 08:46:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:46490eb2f2c1d090137f5c54a8f4bcdff0296ed60f44eceeb562e8d2b028afdf`  
		Last Modified: Sat, 09 Dec 2023 01:23:28 GMT  
		Size: 28.7 MB (28693755 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:747046b561b998cef822af21f281a99fb86bc4157aea556211d0767f79817dd0`  
		Last Modified: Sat, 09 Dec 2023 01:23:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b5dad2ef0d58f7808e229b6c03aa25e344c829a5ba26d8ed2ea3513208d8dd6b`  
		Last Modified: Wed, 20 Dec 2023 04:35:57 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fc94be59a1f26a4c3d2c7393305b9abbb0bdb33bd7e2f8e5cca235c887a6f7b`  
		Last Modified: Wed, 20 Dec 2023 04:35:59 GMT  
		Size: 86.7 MB (86682810 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:66f62b6540fe23707b8fdaf9684c2c53f56c9d2aa239f562dcf8114819b1876f`  
		Last Modified: Wed, 20 Dec 2023 04:35:58 GMT  
		Size: 134.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:41134d3fe803af9616f21104f36c0fea865f012422cdb5ee22385fcd8d45c268`  
		Last Modified: Wed, 20 Dec 2023 04:35:58 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e6f7bb9fef482dc24c6b08e5cf620046ae348773f1741d8c151bc323403fbd85`  
		Last Modified: Wed, 20 Dec 2023 04:35:59 GMT  
		Size: 3.2 MB (3236769 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c3a709ac1ce78451f210a0e4461f495b5ae27147a41617e9bdebb51f805ffed7`  
		Last Modified: Wed, 20 Dec 2023 04:36:00 GMT  
		Size: 70.3 MB (70266778 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d81dc12d377fb1999d4735dd4c438c0044c5648f3639dd6248c9e9fca2dc704b`  
		Last Modified: Wed, 20 Dec 2023 04:35:59 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:5-alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:9b25bdc94894d3ce768d0cb7a5d83b69124bc2a41d4b8e4a3d0a40e9d603cb3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4599556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e6a343dec61bc9d98faafbf1fceae3015afb890c584e83bc34dcb96795f04ab`

```dockerfile
```

-	Layers:
	-	`sha256:f30a871a8f4e48415ab9cef4af4d10243e0fec7ab78ea5bb0e028995eb4d92ef`  
		Last Modified: Wed, 20 Dec 2023 04:35:57 GMT  
		Size: 4.6 MB (4564572 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:338f2176ba6f9f8fdf3057dc2b1c7df8d082d4466e4e930c7173dd6cbeb38e8d`  
		Last Modified: Wed, 20 Dec 2023 04:35:57 GMT  
		Size: 35.0 KB (34984 bytes)  
		MIME: application/vnd.in-toto+json
