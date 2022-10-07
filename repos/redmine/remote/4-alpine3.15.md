## `redmine:4-alpine3.15`

```console
$ docker pull redmine@sha256:1cb82a46a148a6c8c664ea733f9fd3d7787d9ff015f88980bfc8f970259b4d3e
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

### `redmine:4-alpine3.15` - linux; amd64

```console
$ docker pull redmine@sha256:4d71583127dd2a8f4a0ac72ef4de085d3a7c9fe925c8971a82159a49b2e28aae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.3 MB (160265587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cc480f5a35e5aa8c5f44742e23e757409092bd9ecfeeb3d5f4caabcb4217aec`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 03:39:38 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 07 Oct 2022 03:39:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 07 Oct 2022 03:39:39 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 03:54:52 GMT
ENV RUBY_MAJOR=2.7
# Fri, 07 Oct 2022 03:54:52 GMT
ENV RUBY_VERSION=2.7.6
# Fri, 07 Oct 2022 03:54:52 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Fri, 07 Oct 2022 03:56:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 03:56:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 03:56:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 03:56:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 03:56:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 03:56:37 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 08:43:58 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 08:44:08 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 08:44:09 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 08:44:09 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 08:44:09 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 08:44:10 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 08:44:10 GMT
ENV REDMINE_VERSION=4.2.8
# Fri, 07 Oct 2022 08:44:10 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.8.tar.gz
# Fri, 07 Oct 2022 08:44:10 GMT
ENV REDMINE_DOWNLOAD_SHA256=0b431c052d8fd36b93201dafaf3615cdb8d03460efcf2400e7d32662b2ab6272
# Fri, 07 Oct 2022 08:44:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 08:44:14 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 08:46:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 08:46:23 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 08:46:23 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 08:46:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 08:46:23 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 08:46:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21fafba7b6adda1d48ec07e3047626a3c4f4340db51965fa495db75fdbbd2266`  
		Last Modified: Fri, 07 Oct 2022 03:58:32 GMT  
		Size: 3.7 MB (3694985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a3439ad63dfb217b7df7acc43ed7bca7e070f0b3dbef395fa12ae2b67892b7`  
		Last Modified: Fri, 07 Oct 2022 03:58:31 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cff0669ea43a8e0cdd6787da3297ecc442f9eb55921e0dd944bcc9599e86c7`  
		Last Modified: Fri, 07 Oct 2022 04:00:44 GMT  
		Size: 14.0 MB (13981883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffff2cdafbf5f066e8e0361116e785fbe1762e874e07a9e13c1ef1d0edb35475`  
		Last Modified: Fri, 07 Oct 2022 04:00:42 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:550a231a144f88813f0584b360f0db050380e7aa62f3bbb95c15ede464b82797`  
		Last Modified: Fri, 07 Oct 2022 08:47:58 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf826cdc70912f5522fa083f05d3e93e33cecf14aa51198255505df11dbb6d27`  
		Last Modified: Fri, 07 Oct 2022 08:48:10 GMT  
		Size: 83.0 MB (82976903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2086169fc814bf3f6ec23ad2f520b5c0e2f273c8166205a6e3b776b0cc927e61`  
		Last Modified: Fri, 07 Oct 2022 08:47:55 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6264f541b62d7c70f759426f1e98c20118a6c9ddac4a3f9410ac03d0e1978520`  
		Last Modified: Fri, 07 Oct 2022 08:47:55 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388da81e7f2c836c679bc9d325800987c2ce960e9261c9d50f7ea0c605006f3f`  
		Last Modified: Fri, 07 Oct 2022 08:47:56 GMT  
		Size: 3.1 MB (3067696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba4799930df032461568e1e435186506c8ce898d542dcd3690b4510ab3d3398`  
		Last Modified: Fri, 07 Oct 2022 08:48:01 GMT  
		Size: 53.7 MB (53716811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bf1e2598ead17cf03b5b971b8540c2883cf842bee395debafcc00ce5df78e76`  
		Last Modified: Fri, 07 Oct 2022 08:47:55 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; arm variant v6

```console
$ docker pull redmine@sha256:66f7c6b41d6d97232a36d67111378e1e23b32f55e0897dd1b770cad4a1de2a8e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153848694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b03dbfbacdac6c435c56c4fd57765625880c77519968d857808771629aaecd2f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:05:57 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 11 Aug 2022 00:05:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 11 Aug 2022 00:05:58 GMT
ENV LANG=C.UTF-8
# Thu, 11 Aug 2022 00:30:22 GMT
ENV RUBY_MAJOR=2.7
# Thu, 11 Aug 2022 00:30:22 GMT
ENV RUBY_VERSION=2.7.6
# Thu, 11 Aug 2022 00:30:22 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Thu, 11 Aug 2022 00:33:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 11 Aug 2022 00:33:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 11 Aug 2022 00:33:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 11 Aug 2022 00:33:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 00:33:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 11 Aug 2022 00:33:23 GMT
CMD ["irb"]
# Thu, 11 Aug 2022 03:33:10 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 11 Aug 2022 03:33:21 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 11 Aug 2022 03:33:21 GMT
ENV RAILS_ENV=production
# Thu, 11 Aug 2022 03:33:22 GMT
WORKDIR /usr/src/redmine
# Thu, 11 Aug 2022 03:33:22 GMT
ENV HOME=/home/redmine
# Thu, 11 Aug 2022 03:33:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 03 Oct 2022 22:54:24 GMT
ENV REDMINE_VERSION=4.2.8
# Mon, 03 Oct 2022 22:54:24 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.8.tar.gz
# Mon, 03 Oct 2022 22:54:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=0b431c052d8fd36b93201dafaf3615cdb8d03460efcf2400e7d32662b2ab6272
# Mon, 03 Oct 2022 22:54:28 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 03 Oct 2022 22:54:28 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 03 Oct 2022 22:56:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 03 Oct 2022 22:56:55 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 03 Oct 2022 22:56:55 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Mon, 03 Oct 2022 22:56:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 03 Oct 2022 22:56:55 GMT
EXPOSE 3000
# Mon, 03 Oct 2022 22:56:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f0faeca6fc43556638629d0f153cb1dff00d20faab037472a85b6de0bd0b65`  
		Last Modified: Thu, 11 Aug 2022 00:35:11 GMT  
		Size: 3.4 MB (3445570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2d399ece95e132732436ca91a06692e33758533e1f84766a8f23de833aee16`  
		Last Modified: Thu, 11 Aug 2022 00:35:10 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e9727f40711d3d483867b60147613443c804bb9c4dd7b158bd2f7a492041cf`  
		Last Modified: Thu, 11 Aug 2022 00:37:20 GMT  
		Size: 13.4 MB (13412581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99897172c8d6b317c3a07b7bbf665b34657e25fb28905d9f906a06891bbae505`  
		Last Modified: Thu, 11 Aug 2022 00:37:19 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20edcf82b7f27a710d5c3b4b3c1f88e91ac28bebf1977ae6675acadac2e303ed`  
		Last Modified: Thu, 11 Aug 2022 03:38:05 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d4c4021870a77fbd969e9e8d017b5d14768f8e1107b6b808a8a877f8b9b756`  
		Last Modified: Thu, 11 Aug 2022 03:38:19 GMT  
		Size: 78.4 MB (78447211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c188c0531e542fb8a1c256863215e562a1a3d5dbc2d708e661d833b446d0ca2d`  
		Last Modified: Thu, 11 Aug 2022 03:38:02 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d7f54934fcfa4fa1b26460f51a2688b1252af2d13e9380b1c99b2a703228068`  
		Last Modified: Thu, 11 Aug 2022 03:38:03 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1ab79a63e63e9a7cba52b86273fcf72fcc58408af1ba43efca229ea3461854`  
		Last Modified: Mon, 03 Oct 2022 22:58:27 GMT  
		Size: 3.1 MB (3067484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb15fa773efa9c92076e4808d5c25cdb6de2280c698b86f6cc8c4bb44a69e80`  
		Last Modified: Mon, 03 Oct 2022 22:58:33 GMT  
		Size: 52.8 MB (52840921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9954e20ea624345b0ef3e672139fddca4874b96ccb44309574bdbd593769b3ee`  
		Last Modified: Mon, 03 Oct 2022 22:58:26 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; arm variant v7

```console
$ docker pull redmine@sha256:5cbaa4eaecdea58ce1e4e367336e60fb7bc15e5619b3ea15d38525fe19d2abf3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.6 MB (149619641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81fc414495b556fe02bde20b42293ff6545175de9a91a0287582b2c529be9d80`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 04:01:39 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 07 Oct 2022 04:01:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 07 Oct 2022 04:01:40 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 04:49:51 GMT
ENV RUBY_MAJOR=2.7
# Fri, 07 Oct 2022 04:49:51 GMT
ENV RUBY_VERSION=2.7.6
# Fri, 07 Oct 2022 04:49:51 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Fri, 07 Oct 2022 04:55:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 04:55:37 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 04:55:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 04:55:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 04:55:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 04:55:39 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 05:17:24 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 05:17:41 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 05:17:41 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 05:17:41 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 05:17:42 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 05:17:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 05:17:42 GMT
ENV REDMINE_VERSION=4.2.8
# Fri, 07 Oct 2022 05:17:43 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.8.tar.gz
# Fri, 07 Oct 2022 05:17:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=0b431c052d8fd36b93201dafaf3615cdb8d03460efcf2400e7d32662b2ab6272
# Fri, 07 Oct 2022 05:17:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 05:17:48 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 05:20:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 05:20:36 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 05:20:36 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 05:20:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 05:20:37 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 05:20:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366f8010a5765a25a9f0c12e1f2a2d93c6a7a289614ce8083bbbac2140ac80b2`  
		Last Modified: Fri, 07 Oct 2022 05:00:48 GMT  
		Size: 3.3 MB (3313772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1958e36ea2c2b8149803190a22d52d486cb8e3ff698c65c2f3e884cd84573c81`  
		Last Modified: Fri, 07 Oct 2022 05:00:46 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6bb7b80bcc978f52ba33586e05d53a80cf88305460e7b328aee3371893025b`  
		Last Modified: Fri, 07 Oct 2022 05:04:05 GMT  
		Size: 13.3 MB (13302194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed28074dca384ab7bcbcc5b5a0b0ecf6178cde6db099911505b5e94c575e6fb`  
		Last Modified: Fri, 07 Oct 2022 05:04:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a4c42677173636cf4429db3b4b0d3f993090379d37622b1c4ed19ca4a8f1afe`  
		Last Modified: Fri, 07 Oct 2022 05:25:27 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6c73c68a07c21ab4532de87f95dd3a1e5e6977fa8d250422ed2324cd0d9369`  
		Last Modified: Fri, 07 Oct 2022 05:25:47 GMT  
		Size: 75.0 MB (74983447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52464e2c0efca9f26a44371aa2a0716ac099bc3ca4665ff178e4eb7d0f45443`  
		Last Modified: Fri, 07 Oct 2022 05:25:24 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2a75ae711d75e836d6628c43b2df516ddb8ebc28b989a87ebfcfb8b7e17927`  
		Last Modified: Fri, 07 Oct 2022 05:25:24 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09ff0eeb09352b2d27116f94d138fbfd0bd0b6443d7fc7c23d6c0c070d88766`  
		Last Modified: Fri, 07 Oct 2022 05:25:26 GMT  
		Size: 3.1 MB (3067661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a45c6f3069742d505cc8e77c84443b434dbfa223a485b6e19e62afcf4153d84`  
		Last Modified: Fri, 07 Oct 2022 05:25:39 GMT  
		Size: 52.5 MB (52513673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08970407c3c32bc2fa6dba8d2b5e6af2bfb858b1a699120b51537e38c1c5b38`  
		Last Modified: Fri, 07 Oct 2022 05:25:24 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:033543efd1cdae792198afad3844d7dda61e2eddd6dfb94f8c13634807a3e06c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.0 MB (157017026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fd6b226c56d9fbdbcbbb698b9ab72d047c5365b0642daf929a692d8d6aa4f09`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:08:10 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 07 Oct 2022 07:08:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 07 Oct 2022 07:08:12 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 07:24:38 GMT
ENV RUBY_MAJOR=2.7
# Fri, 07 Oct 2022 07:24:39 GMT
ENV RUBY_VERSION=2.7.6
# Fri, 07 Oct 2022 07:24:40 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Fri, 07 Oct 2022 07:26:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 07:26:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 07:26:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 07:26:30 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 07:26:31 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 07:26:32 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 11:36:59 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 11:37:06 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 11:37:07 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 11:37:07 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 11:37:08 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 11:37:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 11:37:10 GMT
ENV REDMINE_VERSION=4.2.8
# Fri, 07 Oct 2022 11:37:11 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.8.tar.gz
# Fri, 07 Oct 2022 11:37:12 GMT
ENV REDMINE_DOWNLOAD_SHA256=0b431c052d8fd36b93201dafaf3615cdb8d03460efcf2400e7d32662b2ab6272
# Fri, 07 Oct 2022 11:37:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 11:37:17 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 11:39:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 11:39:50 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 11:39:51 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 11:39:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 11:39:53 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 11:39:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed552f1aa304f5a195814a26da6aa7fdd32470f2ff2eb352848ecd58aea72c7c`  
		Last Modified: Fri, 07 Oct 2022 07:30:03 GMT  
		Size: 3.7 MB (3658845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f078e52ac32aca9b217a7ced0e8df665d3ac552de1cb9453a94f8949f0761ea0`  
		Last Modified: Fri, 07 Oct 2022 07:30:02 GMT  
		Size: 195.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42856222aeee2384929a4684aed755fe22c8b6b301d7009d264aba5a800ac3f5`  
		Last Modified: Fri, 07 Oct 2022 07:32:43 GMT  
		Size: 13.8 MB (13814127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb9ed1bd659ef64452943fb29271df675d3eb005746a8c0c08810b415829a36`  
		Last Modified: Fri, 07 Oct 2022 07:32:41 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185399378afcd24c89531caa95a97e30f052ebef742658ba3b92422dba9a8348`  
		Last Modified: Fri, 07 Oct 2022 11:41:56 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcab120cb28d0b308f384dc07a3b248c39629830e74957dcb3ba34459dddc861`  
		Last Modified: Fri, 07 Oct 2022 11:42:08 GMT  
		Size: 80.2 MB (80225842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e7c033e6045a6d8ee19d5a70d649bb2ffa56d6fb5d702562c080b6330ab6cc`  
		Last Modified: Fri, 07 Oct 2022 11:41:54 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed28647ec2acd1483806f3cd02b1bce793adc485aa8a26d36e5c1a8e030675d`  
		Last Modified: Fri, 07 Oct 2022 11:41:54 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c721d7ad7dea0ba80f421a86f46343db59f9f2f602b1510a4387db640b4f41e`  
		Last Modified: Fri, 07 Oct 2022 11:41:55 GMT  
		Size: 3.1 MB (3068211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ac7c0c9496f7e933e23ba0c690579ea55b777229296a8252fb80adaa30b1eaa`  
		Last Modified: Fri, 07 Oct 2022 11:42:01 GMT  
		Size: 53.5 MB (53527888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca3af741cc3c500f29521c6e4922c462594d22d08cb43b9f5843d7d447d64ee`  
		Last Modified: Fri, 07 Oct 2022 11:41:54 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; 386

```console
$ docker pull redmine@sha256:1f312689fd2c179729be0dc838095631eae514b70075c4e828ec08a621019ed6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.5 MB (160490652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:816d9af7a94eee24633247f638605908931938212b336e18ddef7ba27127e7e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 01:40:50 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 07 Oct 2022 01:40:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 07 Oct 2022 01:40:51 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 01:57:32 GMT
ENV RUBY_MAJOR=2.7
# Fri, 07 Oct 2022 01:57:33 GMT
ENV RUBY_VERSION=2.7.6
# Fri, 07 Oct 2022 01:57:34 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Fri, 07 Oct 2022 01:59:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 01:59:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 01:59:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 01:59:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 01:59:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 01:59:20 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 05:28:10 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 05:28:20 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 05:28:20 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 05:28:21 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 05:28:22 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 05:28:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 05:28:24 GMT
ENV REDMINE_VERSION=4.2.8
# Fri, 07 Oct 2022 05:28:25 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.8.tar.gz
# Fri, 07 Oct 2022 05:28:26 GMT
ENV REDMINE_DOWNLOAD_SHA256=0b431c052d8fd36b93201dafaf3615cdb8d03460efcf2400e7d32662b2ab6272
# Fri, 07 Oct 2022 05:28:30 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 05:28:31 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 05:30:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 05:30:46 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 05:30:47 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 05:30:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 05:30:48 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 05:30:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0aa2901a089c9a0c54a1fb84d9f5d6edf4b7f798371f2183ae8c777741da79`  
		Last Modified: Fri, 07 Oct 2022 02:03:06 GMT  
		Size: 3.7 MB (3719459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fb7ac5a4afdf7c282e3816d9decbd40e75b8a41de2f28691478694713828d7`  
		Last Modified: Fri, 07 Oct 2022 02:03:05 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dee9f40f03794ece70b5ff6b6b6aec4697b8621bc848efa40fe6388fd826f92`  
		Last Modified: Fri, 07 Oct 2022 02:06:01 GMT  
		Size: 13.3 MB (13294067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03de802ab834ecf872b766fffe7da967640255c1a50beab0a77ad2b63299073d`  
		Last Modified: Fri, 07 Oct 2022 02:05:59 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a214acc089d21670165270da1ec3cb9c65809e1c74e7843d94fa64059c1fc6e2`  
		Last Modified: Fri, 07 Oct 2022 05:33:00 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32263270683cb72ef1d04428f1e03aa91bed46b9de2382ee8b282790c18bb3a1`  
		Last Modified: Fri, 07 Oct 2022 05:33:11 GMT  
		Size: 84.6 MB (84599313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99036237d3296f06505486be3c1125b3474ad9c6a85b2a36c90bb438f15293b4`  
		Last Modified: Fri, 07 Oct 2022 05:32:57 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f6ed1935460a6c8807fbc3579081b303954437760437fd82bb2bf763522f9a`  
		Last Modified: Fri, 07 Oct 2022 05:32:57 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6420d6dd77b9abd4150409373849dea6ab02a8f9e3978683bd73123798573785`  
		Last Modified: Fri, 07 Oct 2022 05:32:58 GMT  
		Size: 3.1 MB (3067861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d879049062c0cb1d970c8b3a43b7916d3a9381d1dca961a7a48cfd184db0620`  
		Last Modified: Fri, 07 Oct 2022 05:33:03 GMT  
		Size: 53.0 MB (52977762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e16a2d78a3acf9f3c899cb5ba1222a568ce0b81bcb27a917f32384015109248`  
		Last Modified: Fri, 07 Oct 2022 05:32:58 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; ppc64le

```console
$ docker pull redmine@sha256:4564279a3e19206088587f57c552dbe157e3e7bcc36a4c35867cdc64633808bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.8 MB (161848062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71a089cff127332d9200539c24dd5d3de28b8d38851a87487a7e90d1d6eafc9b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 07:07:31 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 07 Oct 2022 07:07:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 07 Oct 2022 07:07:32 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 07:27:51 GMT
ENV RUBY_MAJOR=2.7
# Fri, 07 Oct 2022 07:27:51 GMT
ENV RUBY_VERSION=2.7.6
# Fri, 07 Oct 2022 07:27:51 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Fri, 07 Oct 2022 07:30:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 07:30:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 07:30:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 07:30:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 07:30:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 07:30:22 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 11:49:38 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 11:49:57 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 11:50:00 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 11:50:00 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 11:50:01 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 11:50:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 11:50:02 GMT
ENV REDMINE_VERSION=4.2.8
# Fri, 07 Oct 2022 11:50:02 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.8.tar.gz
# Fri, 07 Oct 2022 11:50:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=0b431c052d8fd36b93201dafaf3615cdb8d03460efcf2400e7d32662b2ab6272
# Fri, 07 Oct 2022 11:50:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 11:50:09 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 11:54:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 11:54:47 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 11:54:47 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 11:54:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 11:54:48 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 11:54:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fb7b02600ebb33ddcead21d73d553ff80a455347c9e2bd3bbd14f99edd8527`  
		Last Modified: Fri, 07 Oct 2022 07:33:33 GMT  
		Size: 3.8 MB (3811858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e62d80154ad9015765af6f308dbf009674606d326e963fe296ed5f53b2b6ea`  
		Last Modified: Fri, 07 Oct 2022 07:33:32 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6100240466364da34a60cac7a7b8e9427770f1057807b0f16bd7227e1da3192a`  
		Last Modified: Fri, 07 Oct 2022 07:36:22 GMT  
		Size: 14.4 MB (14420390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc433d0e4b9eca9038bcfb24019d6812d902743ec9cbaa41741664181ae1568`  
		Last Modified: Fri, 07 Oct 2022 07:36:19 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55606bb9f601ce927c05f8db67578f4bd4ce9a46cab137705bbdeecf8178856`  
		Last Modified: Fri, 07 Oct 2022 11:57:14 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5080ed8f60eceeaa674c8d021b96ce82abfdce0a960c28f27a1bece4f873f018`  
		Last Modified: Fri, 07 Oct 2022 11:57:35 GMT  
		Size: 83.2 MB (83227857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6f5900df0fb1cf7869fc710f97b6283cf344c258e62916a96ed659e06ca586`  
		Last Modified: Fri, 07 Oct 2022 11:57:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ae21af14effeeef60015e448ef09ef4c0349b745cb5da76ebfd7045be630e8`  
		Last Modified: Fri, 07 Oct 2022 11:57:11 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8702e2ee5534d98705512499d55730e3ebbcd1dbc02bccf749fb208831266a32`  
		Last Modified: Fri, 07 Oct 2022 11:57:12 GMT  
		Size: 3.1 MB (3067682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d40d97c9345a18c8d78048ec6555be806b8662a746b53fff6f22df6eb0a5d50`  
		Last Modified: Fri, 07 Oct 2022 11:57:20 GMT  
		Size: 54.5 MB (54503489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988d7e1639ddc896d7c56167edd2e6e470e0cf4213762a62dc8299e220b19632`  
		Last Modified: Fri, 07 Oct 2022 11:57:11 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; s390x

```console
$ docker pull redmine@sha256:666176dfdeed3ccb0d10db3c280328ae0053512e132e7620fe52baa510629433
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152665101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a82f6e8975f003079d0384854dd4a443abc867aef85fd03b547136d516e39423`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 09:27:48 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 07 Oct 2022 09:27:51 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 07 Oct 2022 09:27:52 GMT
ENV LANG=C.UTF-8
# Fri, 07 Oct 2022 09:47:24 GMT
ENV RUBY_MAJOR=2.7
# Fri, 07 Oct 2022 09:47:24 GMT
ENV RUBY_VERSION=2.7.6
# Fri, 07 Oct 2022 09:47:25 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Fri, 07 Oct 2022 09:49:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 09:49:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 09:49:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 09:49:44 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:49:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 09:49:45 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 13:06:04 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 13:06:20 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 13:06:31 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 13:06:32 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 13:06:32 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 13:06:33 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 13:06:33 GMT
ENV REDMINE_VERSION=4.2.8
# Fri, 07 Oct 2022 13:06:33 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.8.tar.gz
# Fri, 07 Oct 2022 13:06:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=0b431c052d8fd36b93201dafaf3615cdb8d03460efcf2400e7d32662b2ab6272
# Fri, 07 Oct 2022 13:06:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 13:06:37 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 13:08:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 13:08:41 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 13:08:41 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 13:08:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 13:08:42 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 13:08:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801566b41285bc62a4c848d683d0b9fabae4177173e56695d80f3737461c8776`  
		Last Modified: Fri, 07 Oct 2022 09:53:15 GMT  
		Size: 3.8 MB (3758581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff7293ff7e2d74ddaa950ef10ebfa081c1d51d20ddd1bbe625e1447ae32704`  
		Last Modified: Fri, 07 Oct 2022 09:53:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb03da9606cc20fb2b42f3bcae64761a140575d88c413308432422cd2ede8d23`  
		Last Modified: Fri, 07 Oct 2022 09:55:13 GMT  
		Size: 14.1 MB (14127074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ae06eb04d1245b77da520f2c3b99b59a283167c58722c117553376d00e4460`  
		Last Modified: Fri, 07 Oct 2022 09:55:12 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4936f7e801a8e96b65019958a820c10622362e7e13b95afbd63aba2a0bf1ad5`  
		Last Modified: Fri, 07 Oct 2022 13:10:32 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b55e3d8ed1accdb62685b80ac47f254470a2260da7f01c03e2c12502f7d96ec`  
		Last Modified: Fri, 07 Oct 2022 13:10:41 GMT  
		Size: 75.1 MB (75084427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3216dcb8017b9b16cd9474262b06435e45994c7c08ea88985eb28205efc0829`  
		Last Modified: Fri, 07 Oct 2022 13:10:31 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a76df8f02d81ddf7f429b8fa5ea226ea2ff5caea6b525513af69e22d78a4a2`  
		Last Modified: Fri, 07 Oct 2022 13:10:31 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa66d140498237aab5629a9f6bccb84eb2208761cb0a5382635f8be9f769cfb3`  
		Last Modified: Fri, 07 Oct 2022 13:10:31 GMT  
		Size: 3.1 MB (3067657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc405e1f1710b0ba927d5f1d3231be06c12b761f4f6c45227e605d15567a546`  
		Last Modified: Fri, 07 Oct 2022 13:10:36 GMT  
		Size: 54.0 MB (54017472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2f445ed444d9664d5ab2d153aedd00ba78cfd1a05990bc303e7cf0811febeef`  
		Last Modified: Fri, 07 Oct 2022 13:10:31 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
