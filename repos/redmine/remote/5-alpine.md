## `redmine:5-alpine`

```console
$ docker pull redmine@sha256:9727757d3b61ca02965de2432c0d8f15b4d9d2dcc80a700b80870c0166b3f327
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

### `redmine:5-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:27e2d1391d024eb936ff80fd4c4ff38394baa4f80cb072e4f77e0e3e08a29bfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.9 MB (190927385 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af823d1d44c5463975dc07c07b2d7c502059c80f95aae3e937e3db9d0950df99`
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
# Fri, 07 Oct 2022 03:45:03 GMT
ENV RUBY_MAJOR=3.1
# Fri, 07 Oct 2022 03:45:03 GMT
ENV RUBY_VERSION=3.1.2
# Fri, 07 Oct 2022 03:45:03 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Fri, 07 Oct 2022 03:47:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 03:47:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 03:47:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 03:47:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 03:47:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 03:47:29 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 08:41:31 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 08:41:41 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 08:41:42 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 08:41:42 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 08:41:42 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 08:41:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 08:41:42 GMT
ENV REDMINE_VERSION=5.0.3
# Fri, 07 Oct 2022 08:41:43 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Fri, 07 Oct 2022 08:41:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Fri, 07 Oct 2022 08:41:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 08:41:46 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 08:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 08:43:37 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 08:43:37 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 08:43:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 08:43:37 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 08:43:37 GMT
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
	-	`sha256:e14d080185efc14b694993705b4c2aa793338873e156e253f30de285ab0b6ec6`  
		Last Modified: Fri, 07 Oct 2022 03:59:26 GMT  
		Size: 29.5 MB (29528305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caae273acc14b6604dd1272fdc3ec3a136e2a1f0a496d4eec7d5f8d46addfbb8`  
		Last Modified: Fri, 07 Oct 2022 03:59:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be60cba9ef1b1e0a2cfc4a89778c6fa62d527e174e9cdb22c6ed04b2727deee1`  
		Last Modified: Fri, 07 Oct 2022 08:47:11 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f59d2e09c25fe2765f5f6662f21bb43be95bab45e7b070d053a53aa07b2ed49`  
		Last Modified: Fri, 07 Oct 2022 08:47:23 GMT  
		Size: 83.0 MB (83006130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a8ba4df2bafbb49bba6a6399847c7c864c1ae93ac9081f846b9c2f188a368b`  
		Last Modified: Fri, 07 Oct 2022 08:47:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed3caed3e2f148fd60e4ec479f54a48d304bb0a5d735191ce631be262c49e79`  
		Last Modified: Fri, 07 Oct 2022 08:47:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dd41ced259b5d25224851bf019eb0a040f57b113db559e243c481bbed5e802`  
		Last Modified: Fri, 07 Oct 2022 08:47:09 GMT  
		Size: 3.1 MB (3142558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51db92799ba97ea5cd1be5e79ffa4703f539dd2cc13be7c5b69053fa0328600e`  
		Last Modified: Fri, 07 Oct 2022 08:47:15 GMT  
		Size: 68.7 MB (68728095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9f03ce74b7831ca5ad5d8ff9f57debe9fbc9219ebd9429cdb1dd755b8e32856`  
		Last Modified: Fri, 07 Oct 2022 08:47:08 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:d1e52b00847f238bbe450278e4dfed5144b722f6fe159b8a53201ada52d24ef5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.5 MB (182535647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4926720ed9ba13e8e33be943a817b3bf2bc814d3db1fe53b38e8694ddf9cd8f6`
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
# Thu, 11 Aug 2022 00:14:44 GMT
ENV RUBY_MAJOR=3.1
# Thu, 11 Aug 2022 00:14:44 GMT
ENV RUBY_VERSION=3.1.2
# Thu, 11 Aug 2022 00:14:44 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Thu, 11 Aug 2022 00:18:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 11 Aug 2022 00:18:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 11 Aug 2022 00:18:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 11 Aug 2022 00:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 Aug 2022 00:18:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 11 Aug 2022 00:18:45 GMT
CMD ["irb"]
# Thu, 11 Aug 2022 03:29:16 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 11 Aug 2022 03:29:35 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 11 Aug 2022 03:29:35 GMT
ENV RAILS_ENV=production
# Thu, 11 Aug 2022 03:29:35 GMT
WORKDIR /usr/src/redmine
# Thu, 11 Aug 2022 03:29:35 GMT
ENV HOME=/home/redmine
# Thu, 11 Aug 2022 03:29:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 03 Oct 2022 22:51:15 GMT
ENV REDMINE_VERSION=5.0.3
# Mon, 03 Oct 2022 22:51:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Mon, 03 Oct 2022 22:51:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Mon, 03 Oct 2022 22:51:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 03 Oct 2022 22:51:19 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 03 Oct 2022 22:54:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 03 Oct 2022 22:54:08 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 03 Oct 2022 22:54:08 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Mon, 03 Oct 2022 22:54:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 03 Oct 2022 22:54:09 GMT
EXPOSE 3000
# Mon, 03 Oct 2022 22:54:09 GMT
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
	-	`sha256:753d7126e6fb6a1423a6d789d4c79596bb3f5e519564fd62e573f92b10fa4e80`  
		Last Modified: Thu, 11 Aug 2022 00:36:02 GMT  
		Size: 28.1 MB (28140479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0215941e27b8cf63c81d1c451f4b4a8c4abeed936e6198c053ed0683d643761d`  
		Last Modified: Thu, 11 Aug 2022 00:35:59 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437c3d7952f8704e8f9d50cd070893d2bb1c351e93cf1451ce77ada69a163e2f`  
		Last Modified: Thu, 11 Aug 2022 03:37:00 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeda5e8751dc8b7e5d4e51f70cdf9e7f72a5c5a5ba677dde1711166460314cc`  
		Last Modified: Thu, 11 Aug 2022 03:37:26 GMT  
		Size: 78.5 MB (78476779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f4d7473301e200b3d3257b658e90a794f88cbf6c492154b8316fd498903d3d`  
		Last Modified: Thu, 11 Aug 2022 03:36:56 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154a01d8d94b1a80b3de48f9230238225cac200e8c406b395bf542f96f90d348`  
		Last Modified: Thu, 11 Aug 2022 03:36:56 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c62488992c01e33a097841baee420d0b3eb37d2bc3a322abd6e32f8d07677c1`  
		Last Modified: Mon, 03 Oct 2022 22:57:41 GMT  
		Size: 3.1 MB (3142597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea411926ebfaff96de2f0dd3c5f97953a4c3476643f075c5446a7a91ad491fd`  
		Last Modified: Mon, 03 Oct 2022 22:57:51 GMT  
		Size: 66.7 MB (66695294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014eaa9a756a02a85aa3cf3a229f808a72d92daa59b2a234380ad06013dbffa0`  
		Last Modified: Mon, 03 Oct 2022 22:57:39 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:9253d2409e89fcdd3e63f5815e824c5cbf2552be3e1e37416a6858f3c8664583
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.2 MB (178249523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b8e9917141556e2114d2f94e0c42202ff7e7bdee7a31a9a88b988ee6c351de4`
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
# Fri, 07 Oct 2022 04:18:54 GMT
ENV RUBY_MAJOR=3.1
# Fri, 07 Oct 2022 04:18:55 GMT
ENV RUBY_VERSION=3.1.2
# Fri, 07 Oct 2022 04:18:55 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Fri, 07 Oct 2022 04:26:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 04:26:51 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 04:26:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 04:26:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 04:26:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 04:26:52 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 05:10:06 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 05:10:24 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 05:10:25 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 05:10:25 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 05:10:25 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 05:10:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 05:10:26 GMT
ENV REDMINE_VERSION=5.0.3
# Fri, 07 Oct 2022 05:10:26 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Fri, 07 Oct 2022 05:10:26 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Fri, 07 Oct 2022 05:10:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 05:10:31 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 05:13:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 05:13:43 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 05:13:44 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 05:13:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 05:13:44 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 05:13:44 GMT
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
	-	`sha256:fe3d3f9c1767bf1f806b7bb6eb4567f17952da186e89de67d2eb97f7a917a0ec`  
		Last Modified: Fri, 07 Oct 2022 05:02:08 GMT  
		Size: 28.0 MB (28035543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952d3cb12fb678e4173049299705caf49594d0fff7cb6fc08b7d3c33b51db45a`  
		Last Modified: Fri, 07 Oct 2022 05:02:03 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3aea38a8b19ed1c38d77a1103c1444d21ae4c665765a36fd58b48bcde41142d`  
		Last Modified: Fri, 07 Oct 2022 05:23:21 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016c525f35fd1751d32e3f5f54a4c58f7dd257f66a86fce7b07df7868496e5e1`  
		Last Modified: Fri, 07 Oct 2022 05:23:46 GMT  
		Size: 75.0 MB (75005455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c07c948427eea19cc8d2c2483e604c82c8604ea3ec452ca35ac4da84a0b856`  
		Last Modified: Fri, 07 Oct 2022 05:23:18 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e75e1aa43443a88f846016575963473ebef2a5e7be105b30e7ce25959339bc`  
		Last Modified: Fri, 07 Oct 2022 05:23:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b672ccc73e0af7bed32a10411d7b8c6a6e57d059ffbd571843817a77fc3f7492`  
		Last Modified: Fri, 07 Oct 2022 05:23:20 GMT  
		Size: 3.1 MB (3142556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e23df4936da00d1b6cae804703e8bb96b9cd5717901c5d54051e80939b5f2a64`  
		Last Modified: Fri, 07 Oct 2022 05:23:39 GMT  
		Size: 66.3 MB (66313306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a40e0c6b0a8910e00cec7f499d91f736a99df82c40a6fe8e2ef573f2a0b9440`  
		Last Modified: Fri, 07 Oct 2022 05:23:18 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:80c97807806e944208a8fdfb12f38dd4ab27b751c46986b5164fdb46a09df4e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.7 MB (186745672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:615952870b44c36f0b47b4e010114e157abfba1be692522d54f3f22434c8326c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 05:44:43 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 10 Aug 2022 05:44:44 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 10 Aug 2022 05:44:45 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 05:50:29 GMT
ENV RUBY_MAJOR=3.1
# Wed, 10 Aug 2022 05:50:30 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 10 Aug 2022 05:50:31 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 10 Aug 2022 05:52:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 10 Aug 2022 05:52:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 10 Aug 2022 05:52:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 10 Aug 2022 05:52:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 05:52:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 10 Aug 2022 05:52:54 GMT
CMD ["irb"]
# Wed, 10 Aug 2022 09:26:03 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 10 Aug 2022 09:26:14 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 10 Aug 2022 09:26:15 GMT
ENV RAILS_ENV=production
# Wed, 10 Aug 2022 09:26:15 GMT
WORKDIR /usr/src/redmine
# Wed, 10 Aug 2022 09:26:16 GMT
ENV HOME=/home/redmine
# Wed, 10 Aug 2022 09:26:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 04 Oct 2022 01:27:43 GMT
ENV REDMINE_VERSION=5.0.3
# Tue, 04 Oct 2022 01:27:44 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Tue, 04 Oct 2022 01:27:44 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Tue, 04 Oct 2022 01:27:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 04 Oct 2022 01:27:49 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 04 Oct 2022 01:29:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 04 Oct 2022 01:29:57 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 04 Oct 2022 01:29:58 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Tue, 04 Oct 2022 01:29:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 04 Oct 2022 01:29:59 GMT
EXPOSE 3000
# Tue, 04 Oct 2022 01:30:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abc92ef883894fabdd3fc874d1c24f6870bfc2ab0e778b30282239686ac9715`  
		Last Modified: Wed, 10 Aug 2022 06:06:39 GMT  
		Size: 3.7 MB (3658884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0144bd30e9f35671acd67f21ca794b05df5602b519f4f3af1f45c23aaef341`  
		Last Modified: Wed, 10 Aug 2022 06:06:38 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9f673a18671db4297452df161bae50166ce69d9698618b9fbf5ea16a880e0d`  
		Last Modified: Wed, 10 Aug 2022 06:07:40 GMT  
		Size: 28.9 MB (28895783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36051e022e8acf8076a128a3ef24fc97e5b10df3f2d82142f25bc94f3785778`  
		Last Modified: Wed, 10 Aug 2022 06:07:37 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c48a88132c6673e0b3c9f792446cae509829bfa76016bc449e673ddc75d3796`  
		Last Modified: Wed, 10 Aug 2022 09:32:59 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd957bce79cb5121c450762f7aa5de62fa33c816933f8aaf39be21c6e7fdbd05`  
		Last Modified: Wed, 10 Aug 2022 09:33:10 GMT  
		Size: 80.3 MB (80262991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9e2b82a9611f667809b79941b781254ff8273ac833d83e13a6f7261a98ba06`  
		Last Modified: Wed, 10 Aug 2022 09:32:57 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5137a41817bdcb0b63fcbee9d00bdbd114db1b677f6c375dc25da1f9c3b3d30`  
		Last Modified: Wed, 10 Aug 2022 09:32:57 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1c0754ab120b2a4157dbea1a35a41b8bff861c36d8469ba23ba9c981494224`  
		Last Modified: Tue, 04 Oct 2022 01:35:44 GMT  
		Size: 3.1 MB (3142299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205523f77b467b5f18224a4bf067c53fe59dbc9b457b7d8f52cfb114ab423b3e`  
		Last Modified: Tue, 04 Oct 2022 01:35:51 GMT  
		Size: 68.1 MB (68063600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd449b8342e90c7c33b8031c40961ebb27a1b0d6eb372926e6325a3773c64f3b`  
		Last Modified: Tue, 04 Oct 2022 01:35:44 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; 386

```console
$ docker pull redmine@sha256:fabe4ee2014d949ea9aa458194e50862cdb770722dcb5102de3e1f128ba49206
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189625430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af420408668c8f3463b2af8b4206cfb899cda0ff04c66b74a136c0c23f336a50`
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
# Fri, 07 Oct 2022 01:46:51 GMT
ENV RUBY_MAJOR=3.1
# Fri, 07 Oct 2022 01:46:52 GMT
ENV RUBY_VERSION=3.1.2
# Fri, 07 Oct 2022 01:46:53 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Fri, 07 Oct 2022 01:49:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 01:49:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 01:49:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 01:49:17 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 01:49:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 01:49:19 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 05:25:22 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 05:25:37 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 05:25:38 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 05:25:38 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 05:25:39 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 05:25:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 05:25:41 GMT
ENV REDMINE_VERSION=5.0.3
# Fri, 07 Oct 2022 05:25:42 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Fri, 07 Oct 2022 05:25:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Fri, 07 Oct 2022 05:25:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 05:25:48 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 05:27:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 05:27:45 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 05:27:46 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Fri, 07 Oct 2022 05:27:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 05:27:47 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 05:27:48 GMT
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
	-	`sha256:067126924841b8d1edfae72ef23c0af3f1c449c417871035ed11eaf126eeac41`  
		Last Modified: Fri, 07 Oct 2022 02:04:13 GMT  
		Size: 28.1 MB (28143528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bd9cb09fd980b7e594334a44ec0a100f700fd570d00a1dc621404f30858b62`  
		Last Modified: Fri, 07 Oct 2022 02:04:10 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07dfe9d696c464f5d956327b5f666afab93174d47a97d4d6051b129a3e4f9a5f`  
		Last Modified: Fri, 07 Oct 2022 05:32:08 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120506f3643b0e45356a0bfab200a34a3129fe69b25ff7e9b5c8d926e7e2dcf2`  
		Last Modified: Fri, 07 Oct 2022 05:32:20 GMT  
		Size: 84.6 MB (84636245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df91841ab0040d46d4d2e9c82655a983766668060f22b31175d189ae4579214`  
		Last Modified: Fri, 07 Oct 2022 05:32:05 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14fbf7042aff873e963de1fc9965dd34129e6c6aee246816bd598af20d37986d`  
		Last Modified: Fri, 07 Oct 2022 05:32:06 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a59c86e38dd350bf9662e352cb7cfbb21f107b783967e56ff5687233d592b8`  
		Last Modified: Fri, 07 Oct 2022 05:32:06 GMT  
		Size: 3.1 MB (3142347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7926c2a3d401a9a3082292149f8686e54292a58431d70a892c7e329b54e670`  
		Last Modified: Fri, 07 Oct 2022 05:32:13 GMT  
		Size: 67.2 MB (67151662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008cdc914c9e9ff2baee81cf7ac6dfffb48d69df35cdb1aa220c925985a20f49`  
		Last Modified: Fri, 07 Oct 2022 05:32:06 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; ppc64le

```console
$ docker pull redmine@sha256:8e002f8797340cee5d5eb1a4062bf464e212154376f536d94956eb25b7486ca4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191670773 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254ed4e32435d07b517f58bca4ea6a041a25a7afbf92752d9875f1c4ebe393c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:23:40 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 10 Aug 2022 02:23:41 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 10 Aug 2022 02:23:42 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 02:31:21 GMT
ENV RUBY_MAJOR=3.1
# Wed, 10 Aug 2022 02:31:22 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 10 Aug 2022 02:31:22 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 10 Aug 2022 02:34:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 10 Aug 2022 02:34:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 10 Aug 2022 02:34:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 10 Aug 2022 02:34:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 02:34:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 10 Aug 2022 02:34:42 GMT
CMD ["irb"]
# Wed, 10 Aug 2022 09:21:31 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 10 Aug 2022 09:22:00 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 10 Aug 2022 09:22:04 GMT
ENV RAILS_ENV=production
# Wed, 10 Aug 2022 09:22:04 GMT
WORKDIR /usr/src/redmine
# Wed, 10 Aug 2022 09:22:04 GMT
ENV HOME=/home/redmine
# Wed, 10 Aug 2022 09:22:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 03 Oct 2022 23:20:39 GMT
ENV REDMINE_VERSION=5.0.3
# Mon, 03 Oct 2022 23:20:39 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Mon, 03 Oct 2022 23:20:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Mon, 03 Oct 2022 23:20:45 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 03 Oct 2022 23:20:46 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 03 Oct 2022 23:24:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 03 Oct 2022 23:24:46 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 03 Oct 2022 23:24:47 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Mon, 03 Oct 2022 23:24:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 03 Oct 2022 23:24:47 GMT
EXPOSE 3000
# Mon, 03 Oct 2022 23:24:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e566db40e1e30abb0430a26de27510925e5d144de0005a3e46bd2bdffc5620`  
		Last Modified: Wed, 10 Aug 2022 02:51:43 GMT  
		Size: 3.8 MB (3811885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75443bd8838a6f027d7523b1fb3812b64bde28fb9b2aac189be3b739f0223d9d`  
		Last Modified: Wed, 10 Aug 2022 02:51:42 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d0ae0504df30b7aac1e21624926f53bcf229f558c22d6f113355dd633ceb191`  
		Last Modified: Wed, 10 Aug 2022 02:52:57 GMT  
		Size: 29.6 MB (29578751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eecc763f9b016d5ea067021d550737b41f71ceb418d882ea856d0f4d5968bff`  
		Last Modified: Wed, 10 Aug 2022 02:52:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b25c2af4ae9bcb9effad925fc822e2d02b2caa81c98ae74280fc47f2b53206d`  
		Last Modified: Wed, 10 Aug 2022 09:33:02 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae0a1a7ca3f906bde6bccd12383d3a225541c8a25ee2bf715d849819913271f`  
		Last Modified: Wed, 10 Aug 2022 09:33:24 GMT  
		Size: 83.3 MB (83262724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824ad83c2901c394e1f5e13176923f4ce615bb49c5e3365a31bf54b2273cda53`  
		Last Modified: Wed, 10 Aug 2022 09:33:00 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d8c4c1a92e034dd720a217cc4177db6e74e598e5d2a12398eb06bcbacdaddd`  
		Last Modified: Wed, 10 Aug 2022 09:33:00 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2709f92020fd0b2de4fda020bed46be3fd2f81af7d0a027eb72a62ba48232160`  
		Last Modified: Mon, 03 Oct 2022 23:36:00 GMT  
		Size: 3.1 MB (3142584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85356fbab4e5bac66874558f9542615a706112c5d8e72ddb0d2c6d0f8d8ab5c7`  
		Last Modified: Mon, 03 Oct 2022 23:36:11 GMT  
		Size: 69.1 MB (69058038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43f9e399924da4b95fae32b623188ce60438725ff1091d5df9a7d2e5c2a70aa`  
		Last Modified: Mon, 03 Oct 2022 23:35:59 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; s390x

```console
$ docker pull redmine@sha256:3284c521ea2e2d7c7407f2e03877900a920f4c4139e45138fa0fbdfb37938cb3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.0 MB (182992010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0de8512f244ccfe4ff197924e47e5f25b8a92b198ec04e797ee059a6435921eb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 06:34:21 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 10 Aug 2022 06:34:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 10 Aug 2022 06:34:21 GMT
ENV LANG=C.UTF-8
# Wed, 10 Aug 2022 06:39:41 GMT
ENV RUBY_MAJOR=3.1
# Wed, 10 Aug 2022 06:39:41 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 10 Aug 2022 06:39:41 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 10 Aug 2022 06:41:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 10 Aug 2022 06:41:51 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 10 Aug 2022 06:41:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 10 Aug 2022 06:41:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 10 Aug 2022 06:41:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 10 Aug 2022 06:41:52 GMT
CMD ["irb"]
# Wed, 10 Aug 2022 14:22:37 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 10 Aug 2022 14:22:47 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 10 Aug 2022 14:22:50 GMT
ENV RAILS_ENV=production
# Wed, 10 Aug 2022 14:22:50 GMT
WORKDIR /usr/src/redmine
# Wed, 10 Aug 2022 14:22:50 GMT
ENV HOME=/home/redmine
# Wed, 10 Aug 2022 14:22:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 03 Oct 2022 22:48:36 GMT
ENV REDMINE_VERSION=5.0.3
# Mon, 03 Oct 2022 22:48:36 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Mon, 03 Oct 2022 22:48:36 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Mon, 03 Oct 2022 22:48:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 03 Oct 2022 22:48:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 03 Oct 2022 22:50:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 03 Oct 2022 22:50:24 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 03 Oct 2022 22:50:24 GMT
COPY file:ec5edc991e6c7f0c678e0703e1db651c89473a4619b1fd7c6e950c773cedccf4 in / 
# Mon, 03 Oct 2022 22:50:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 03 Oct 2022 22:50:25 GMT
EXPOSE 3000
# Mon, 03 Oct 2022 22:50:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244962f9bae0cce37ebf44340bd5a4c572892474dd2d9bdd0be5276b26bd936a`  
		Last Modified: Wed, 10 Aug 2022 06:56:56 GMT  
		Size: 3.8 MB (3758572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c923c29356794980774ed165563e95be535bd8cc20bcf7a8f53cac31b454bb79`  
		Last Modified: Wed, 10 Aug 2022 06:56:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66a58f67ca05527a90eba59c66de509c61933221f76550992c09833a528d8f3`  
		Last Modified: Wed, 10 Aug 2022 07:02:27 GMT  
		Size: 29.4 MB (29366298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5d8bd5ceddacefe4bc7f2e6f6aa56c732097e5000528d3743d2b0682235012`  
		Last Modified: Wed, 10 Aug 2022 07:02:27 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6880a88291851df691564df80fdf6688e7d3e2cce0cce31a73ca9c9afa9751`  
		Last Modified: Wed, 10 Aug 2022 14:28:59 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c33be76500cccc1322705300fe7442627c6fb1165eddd22aa2fa0d75a684b79`  
		Last Modified: Wed, 10 Aug 2022 14:29:03 GMT  
		Size: 75.1 MB (75113441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d26d1884198d3c2b99d65cd56695f8022dc212e795f98939322081b53b298fe`  
		Last Modified: Wed, 10 Aug 2022 14:28:41 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca7c86a30be24d9fd41a6200b2743eab8f549b3fb87d1ce0cdcc498495f1342`  
		Last Modified: Wed, 10 Aug 2022 14:28:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745955803276b3a2ea02a951e5400023be4862e5f896104fe2c042f8c79dbb87`  
		Last Modified: Mon, 03 Oct 2022 22:55:56 GMT  
		Size: 3.1 MB (3142582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5f6fbf627cde9e4be6f391d235038317dbb03643512a7c499c218f3ef55ffe`  
		Last Modified: Mon, 03 Oct 2022 22:56:02 GMT  
		Size: 69.0 MB (69001231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeefcf1ee36656e3fb3e15414a0c340dc1ae551b1cb388abedf700595f2af32b`  
		Last Modified: Mon, 03 Oct 2022 22:55:56 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
