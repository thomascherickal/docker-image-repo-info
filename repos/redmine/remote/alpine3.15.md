## `redmine:alpine3.15`

```console
$ docker pull redmine@sha256:8ba94a9d623cc0cd6d2a7124bbbece3fc562ba95c949aa071feb611d2329c636
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

### `redmine:alpine3.15` - linux; amd64

```console
$ docker pull redmine@sha256:567723df4b10f692331241e3ef6866dc764c6d2450e4ef9a39cb8a8d44c4b33f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191723325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d853d554f8eb58f2ba8b7d7ec83e08254c569360c4c82fd330eb90962db6901`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:09:59 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 05 Apr 2022 03:10:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 05 Apr 2022 03:10:00 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:17:54 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 18:29:47 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 18:29:47 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 18:32:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 18:32:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 18:32:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 18:32:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 18:32:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 18:32:11 GMT
CMD ["irb"]
# Tue, 12 Apr 2022 19:54:12 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 12 Apr 2022 19:54:21 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 12 Apr 2022 19:54:21 GMT
ENV RAILS_ENV=production
# Tue, 12 Apr 2022 19:54:21 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Apr 2022 19:54:22 GMT
ENV HOME=/home/redmine
# Tue, 12 Apr 2022 19:54:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 01:59:11 GMT
ENV REDMINE_VERSION=5.0.2
# Wed, 22 Jun 2022 01:59:11 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Wed, 22 Jun 2022 01:59:11 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Wed, 22 Jun 2022 01:59:14 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 01:59:15 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 02:01:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 02:01:06 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:01:06 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 02:01:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:01:06 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:01:06 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:837e9cfc7e430bf6c3aa43a0b8a8e3d11115abb5b84d75783752c38e06145e85`  
		Last Modified: Tue, 05 Apr 2022 03:46:41 GMT  
		Size: 3.7 MB (3683514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7850f1a8c234d7e3e08596122f1e1bbb5a2b2abedb7d91bb3017697821fe168`  
		Last Modified: Tue, 05 Apr 2022 03:46:40 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0a3cc0f34c0d2743f8af4cdc0e855601dfb95bf12af51a5bf550fe1579b27f`  
		Last Modified: Tue, 12 Apr 2022 19:15:28 GMT  
		Size: 29.5 MB (29529265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81637037ea3a0fb0e48ff953bda883637a1d79671b41a35c4d571a3a29ab0662`  
		Last Modified: Tue, 12 Apr 2022 19:15:24 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2613a8d1f3b917fb6a88bb6283a2e615271c998784ed1c95f532026fe1f2a7cc`  
		Last Modified: Tue, 12 Apr 2022 20:06:36 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf47334f1459082a5d3f879f24a2b4cfa747c1e8a46abd11166f7fdf43487206`  
		Last Modified: Tue, 12 Apr 2022 20:06:48 GMT  
		Size: 82.3 MB (82270498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76dea3945a6af229b487a62bfe51acdb53ba24fe6fa607b6009d8fc079d1f80`  
		Last Modified: Tue, 12 Apr 2022 20:06:34 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcd2c3b15c4016ba5a5f153a79461d46a41c454da764dde90842edc74ca2067`  
		Last Modified: Tue, 12 Apr 2022 20:06:34 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5751c6fca29aa5898f14dacc284ec57496da8f361846c62417f94a88961637e0`  
		Last Modified: Wed, 22 Jun 2022 02:06:07 GMT  
		Size: 3.1 MB (3130614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0565037dd4ee9f3f93b432a827e3e5ad3d2144a4cc4ca91ed83718cbd5406b01`  
		Last Modified: Wed, 22 Jun 2022 02:06:13 GMT  
		Size: 70.3 MB (70291136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eedbec22ece588555231b01bdc774862bc55334a5a1985ea7a4f9a74ae7142`  
		Last Modified: Wed, 22 Jun 2022 02:06:07 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; arm variant v6

```console
$ docker pull redmine@sha256:faedc84c335a295ffd644ef3e8ccc12429d5a13a9d6146d131846630bf543730
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.0 MB (183026266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bd9f3a99d64eb55fb884fa75561d46c2ccc5a3b77a326435b3653689f1fe9a2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 01:44:45 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 05 Apr 2022 01:44:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 05 Apr 2022 01:44:47 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 01:54:12 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 18:50:13 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 18:50:14 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 18:54:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 18:54:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 18:54:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 18:54:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 18:54:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 18:54:48 GMT
CMD ["irb"]
# Tue, 12 Apr 2022 19:48:22 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 12 Apr 2022 19:48:56 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 12 Apr 2022 19:48:57 GMT
ENV RAILS_ENV=production
# Tue, 12 Apr 2022 19:48:58 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Apr 2022 19:48:58 GMT
ENV HOME=/home/redmine
# Tue, 12 Apr 2022 19:49:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 01:51:38 GMT
ENV REDMINE_VERSION=5.0.2
# Wed, 22 Jun 2022 01:51:39 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Wed, 22 Jun 2022 01:51:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Wed, 22 Jun 2022 01:51:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 01:51:46 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 01:56:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 01:57:00 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 01:57:01 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 01:57:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 01:57:01 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 01:57:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7545e7edf1071fc6d7e86f69e37fc26922fd2a788c2b1761abed26fc240f344e`  
		Last Modified: Tue, 05 Apr 2022 02:31:38 GMT  
		Size: 3.4 MB (3431573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036e88143cdec70b29fc4d12ba763c4639f427e24fd43ddb7bacd3111c1ed4a6`  
		Last Modified: Tue, 05 Apr 2022 02:31:36 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43044f33f748d2bc9d4b1f10c313137a6c7487e08ebb547316f44a1b815223d9`  
		Last Modified: Tue, 12 Apr 2022 19:29:17 GMT  
		Size: 28.1 MB (28139227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c74ad76db62931c5370aba43db94e7da8d2a7cc6038a4cc19cbfb667cd82c44`  
		Last Modified: Tue, 12 Apr 2022 19:29:03 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8cfcab0059ee5e0d7eb098fb2fbbfe592f8c192d632487381ce2c5869cfb5`  
		Last Modified: Tue, 12 Apr 2022 20:10:28 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9138c20ebfa73d80427ddf25665c22bb7bdfbe1d4ce5cd215da566d8dba8d380`  
		Last Modified: Tue, 12 Apr 2022 20:11:17 GMT  
		Size: 77.7 MB (77717714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397be0e82ee3933c74ed693c46fcf34db121b66c1a8fb8715fd9fc697d64ffcb`  
		Last Modified: Tue, 12 Apr 2022 20:10:26 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d460c958071ba458802a08636d86bd11e7429f27a1e1c0f2bcc9b72f60ed104a`  
		Last Modified: Tue, 12 Apr 2022 20:10:26 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7280c62233fdb82476c0416f2a9cd3d9347dc69b65a4796226ea86b397b024a7`  
		Last Modified: Wed, 22 Jun 2022 02:05:20 GMT  
		Size: 3.1 MB (3130593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e404045a9bbeddc7b6a7d5ff791bed62652d03a7ece3cc905d5501fb2154a31b`  
		Last Modified: Wed, 22 Jun 2022 02:05:48 GMT  
		Size: 68.0 MB (67981446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021429466ad531ffac09d2377900ef5ad15e42149618bbf55ed63ca416f326d2`  
		Last Modified: Wed, 22 Jun 2022 02:05:16 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; arm variant v7

```console
$ docker pull redmine@sha256:792ce7b7b33798b5d873bb9f2a83f857d2f0f18e05c7abab201ccb7aa9ad8aa9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **178.7 MB (178704757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c08e3265125e29d029ac7fc2c47e172f0a49b6106462856fdf4fc952dc3a3c2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:14:47 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 05 Apr 2022 03:14:49 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 05 Apr 2022 03:14:49 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:24:54 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 19:20:02 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 19:20:03 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 19:24:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:24:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:24:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:24:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:24:14 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:24:14 GMT
CMD ["irb"]
# Wed, 13 Apr 2022 02:40:32 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 13 Apr 2022 02:41:00 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 13 Apr 2022 02:41:02 GMT
ENV RAILS_ENV=production
# Wed, 13 Apr 2022 02:41:02 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Apr 2022 02:41:02 GMT
ENV HOME=/home/redmine
# Wed, 13 Apr 2022 02:41:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 03:37:22 GMT
ENV REDMINE_VERSION=5.0.2
# Wed, 22 Jun 2022 03:37:23 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Wed, 22 Jun 2022 03:37:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Wed, 22 Jun 2022 03:37:30 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 03:37:30 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 03:42:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 03:42:22 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 03:42:23 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 03:42:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 03:42:24 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 03:42:24 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf827bdbeb6803ee356377c29e2dc205b1bde74d175f62f1022266f052435ad0`  
		Last Modified: Tue, 05 Apr 2022 04:08:52 GMT  
		Size: 3.3 MB (3301946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a44b4cdfaacd5e37f9bcb3628c53a09ce87fcef30a5a2a3b3cc27d88b6ae81f`  
		Last Modified: Tue, 05 Apr 2022 04:08:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a545f4fcd6303889ed08bb6f56b48e8b906f79c64befc1c34dd95f185f9bd1b7`  
		Last Modified: Tue, 12 Apr 2022 20:58:27 GMT  
		Size: 28.0 MB (28033895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3748643d23db2ff31fb281b7593a55ac7cf53b599ad7bf2bb4ca88ef87fce5a`  
		Last Modified: Tue, 12 Apr 2022 20:58:19 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95969648f8bbdf35a7bd306b6e088953a6b4424e038a253c13acba81935c204e`  
		Last Modified: Wed, 13 Apr 2022 03:15:57 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fadfecbdee0c73778c20d450ca507e895f5754152fd8f182e5eb8dcbd338cff`  
		Last Modified: Wed, 13 Apr 2022 03:16:45 GMT  
		Size: 74.3 MB (74287386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a6eb800313495a43a27608e8e3aaafd9cf789e27c48865011b2b81911ec259`  
		Last Modified: Wed, 13 Apr 2022 03:15:55 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae84ec9943ac2461d3afbd097a3ede4390135641cd7888473f458aa3e1d8506e`  
		Last Modified: Wed, 13 Apr 2022 03:15:55 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045649609b1149e6bc863b70a7a1856c7c0cc746cd980f6882aa842b3bfdff42`  
		Last Modified: Wed, 22 Jun 2022 03:58:00 GMT  
		Size: 3.1 MB (3130578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d468b203372305e40281d3c79f02ea788024b5d02213a102e4cd6acceebeba3`  
		Last Modified: Wed, 22 Jun 2022 03:58:29 GMT  
		Size: 67.5 MB (67522886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2ff4d7fede929fbd094b4665ab37e0585240b21035b867846e029de7fa94f8`  
		Last Modified: Wed, 22 Jun 2022 03:57:56 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:9857e31bd2ffcc04ae9321b4184f12eb6c1ddde547d5541d7762a0c771953ec2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.3 MB (187341307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f20f1d00c6da3e0f1311ca6a6bf8a68d58d544baa0359f073bc46060b90b591`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 02:11:37 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 05 Apr 2022 02:11:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 05 Apr 2022 02:11:39 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 02:17:22 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 18:50:33 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 18:50:34 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 18:52:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 18:52:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 18:52:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 18:52:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 18:52:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 18:52:57 GMT
CMD ["irb"]
# Tue, 12 Apr 2022 21:45:59 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 12 Apr 2022 21:46:08 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 12 Apr 2022 21:46:09 GMT
ENV RAILS_ENV=production
# Tue, 12 Apr 2022 21:46:09 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Apr 2022 21:46:10 GMT
ENV HOME=/home/redmine
# Tue, 12 Apr 2022 21:46:11 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:55:04 GMT
ENV REDMINE_VERSION=5.0.2
# Wed, 22 Jun 2022 02:55:04 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Wed, 22 Jun 2022 02:55:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Wed, 22 Jun 2022 02:55:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:55:10 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 02:57:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 02:57:25 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:57:27 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 02:57:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:57:28 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:57:29 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d89da37be58749a8406b05be8329f35a79dc8340c20154ca6f30c11a9dfff660`  
		Last Modified: Tue, 05 Apr 2022 02:41:52 GMT  
		Size: 3.6 MB (3646058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6acf1cb6c782f3807bbd741be79c451de92ec7cebf8779a2175a1db05c39647`  
		Last Modified: Tue, 05 Apr 2022 02:41:51 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7881d085357f09b444b52f7dc8e01e93c5e12a5f1f164214de436f68be8b9755`  
		Last Modified: Tue, 12 Apr 2022 19:39:27 GMT  
		Size: 28.9 MB (28894951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b423c0b2db83c094d47a28b9875e406353c7bad292e45bb53c24bc94182353c`  
		Last Modified: Tue, 12 Apr 2022 19:39:24 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dea018ac6d64d2bc3a29ac8ec60d96e6146660e472c89c72e03797ee886f385`  
		Last Modified: Tue, 12 Apr 2022 22:02:17 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9426db5984235625b4dae31b1e327086bbfb529e82aa20b16e821276a5ae7e10`  
		Last Modified: Tue, 12 Apr 2022 22:02:29 GMT  
		Size: 79.5 MB (79499901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a053efe498a5a95ddf83e6a46f8a91b3e06ca287fa1d34203119c0903995d2`  
		Last Modified: Tue, 12 Apr 2022 22:02:15 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76150d26b44b4e7598a0d6e77a007b5ec348b967f857ff5698f2e42f5fde867d`  
		Last Modified: Tue, 12 Apr 2022 22:02:15 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0690494cb873bbc87dd06dd59d8ce590b914bbf4b5067ec5551987916747df67`  
		Last Modified: Wed, 22 Jun 2022 03:03:13 GMT  
		Size: 3.1 MB (3130463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3d5584955f7557443e61a736d39cce08f642aea1dc54f6e7a7482600f27cd6`  
		Last Modified: Wed, 22 Jun 2022 03:03:20 GMT  
		Size: 69.4 MB (69449841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2043c094ec1f4159f829af546952f5cecf6cdfaff5e82da708078c760936a2c5`  
		Last Modified: Wed, 22 Jun 2022 03:03:12 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; 386

```console
$ docker pull redmine@sha256:0d66714647c83dd787b5796434e6635d63cc00649256551c5892687388a008ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.4 MB (190394040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526ca6ec7a3a719659afd9992615fd4be771e53d65436b480f4b09b5830f46b2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 01:44:03 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 05 Apr 2022 01:44:03 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 05 Apr 2022 01:44:04 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 01:49:50 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 18:48:54 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 18:48:55 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 18:51:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 18:51:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 18:51:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 18:51:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 18:51:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 18:51:20 GMT
CMD ["irb"]
# Tue, 12 Apr 2022 21:40:43 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 12 Apr 2022 21:40:55 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 12 Apr 2022 21:40:56 GMT
ENV RAILS_ENV=production
# Tue, 12 Apr 2022 21:40:56 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Apr 2022 21:40:57 GMT
ENV HOME=/home/redmine
# Tue, 12 Apr 2022 21:40:58 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:08:29 GMT
ENV REDMINE_VERSION=5.0.2
# Wed, 22 Jun 2022 02:08:30 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Wed, 22 Jun 2022 02:08:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Wed, 22 Jun 2022 02:08:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:08:35 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 02:10:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 02:10:35 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:10:36 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 02:10:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:10:37 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:10:38 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fb6b86a080a32f16361b400c76199f15ac541d216b540ff71a056643e457e2`  
		Last Modified: Tue, 05 Apr 2022 02:14:23 GMT  
		Size: 3.7 MB (3709251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62ce2c6e49fd9ed5937c71b2a26b34eac8d00f722e3e5bce7e6a93cedd7f58`  
		Last Modified: Tue, 05 Apr 2022 02:14:22 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2333d0b31bf085166f0dfc527ab94d93524940fd856afdf1ccd59c83c4371b48`  
		Last Modified: Tue, 12 Apr 2022 19:37:27 GMT  
		Size: 28.1 MB (28142640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2f7a60a3701de01c12f90f6c9f1216f120f955afdcf4f74d7508ed5e876460`  
		Last Modified: Tue, 12 Apr 2022 19:37:18 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b7c425134801516852d3047213b0c77bb938a22d6d78a3f44d359e24a79a57`  
		Last Modified: Tue, 12 Apr 2022 21:54:08 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d37a4f1085d0c4e506de514df622e70bbbbe0ad1fc9e21bfdb13080eb1c0878`  
		Last Modified: Tue, 12 Apr 2022 21:54:21 GMT  
		Size: 83.9 MB (83880675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d43630c9d077703d07d391734cef31f2128774866f5a001d0690e8b9f30835f`  
		Last Modified: Tue, 12 Apr 2022 21:54:06 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c5ef6f6cec1ba13802fc524e1e94b00231618c904f572b118bba5046f509ca`  
		Last Modified: Tue, 12 Apr 2022 21:54:06 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fcab03986a47b4aca8741b409be44f7d1679fa5a6769a32385ffd3619673786`  
		Last Modified: Wed, 22 Jun 2022 02:16:22 GMT  
		Size: 3.1 MB (3130552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1c19749c1c1bf5a82ba5055b1cd6bb3c8eec431200e5fe8c5c5a2977fdd8bc`  
		Last Modified: Wed, 22 Jun 2022 02:16:36 GMT  
		Size: 68.7 MB (68708336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f7cdd19311900a4eea125d2c57499eea37594026188f0d347c63f25a0e1f6d6`  
		Last Modified: Wed, 22 Jun 2022 02:16:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; ppc64le

```console
$ docker pull redmine@sha256:2ba81418c9e179f5e854a5331b45b175bc92ffafb3b0f074c492854c630dcbf1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.4 MB (192355243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28f9807d3f609d46f3dbc27557eb72ba14b58b8b76b4ef852e396fdd2cd10252`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:41:00 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 05 Apr 2022 05:41:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 05 Apr 2022 05:41:16 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 05:50:39 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 19:20:20 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 19:20:32 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 19:23:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:24:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:24:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:24:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:24:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:24:24 GMT
CMD ["irb"]
# Wed, 13 Apr 2022 01:19:03 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 13 Apr 2022 01:20:09 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 13 Apr 2022 01:20:17 GMT
ENV RAILS_ENV=production
# Wed, 13 Apr 2022 01:20:19 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Apr 2022 01:20:22 GMT
ENV HOME=/home/redmine
# Wed, 13 Apr 2022 01:20:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 04:23:12 GMT
ENV REDMINE_VERSION=5.0.2
# Wed, 22 Jun 2022 04:23:14 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Wed, 22 Jun 2022 04:23:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Wed, 22 Jun 2022 04:23:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 04:23:38 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 04:27:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 04:27:20 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 04:27:25 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 04:27:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 04:27:41 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 04:27:45 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5113171de8d9f33468047c84fbf15e92533f5415e7e83e34dcd641d1ea7eaa09`  
		Last Modified: Tue, 05 Apr 2022 06:29:30 GMT  
		Size: 3.8 MB (3800255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23738be7f844f7748f802982b6ffc1621b25ff1935e11e7062912e4737adbcda`  
		Last Modified: Tue, 05 Apr 2022 06:29:29 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d86129333cfe8d14cf0fcd9dceed9f00e43ceec8183e38e36b663b93f69177`  
		Last Modified: Tue, 12 Apr 2022 21:17:16 GMT  
		Size: 29.6 MB (29578355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0e59c495c2b0700d67b6f2a2840f2f1769c31afb187f5b37dc98e2517293a8`  
		Last Modified: Tue, 12 Apr 2022 21:17:12 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd35bd579ac1bb6e05f0f1388320953fcc3c742be1c4d58404b64ec53ab82fa`  
		Last Modified: Wed, 13 Apr 2022 01:55:56 GMT  
		Size: 1.2 KB (1225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd1a36942f884b5f7aae7eb17d4c1bd2092c2c55479b9cfdecec25b368b6b14`  
		Last Modified: Wed, 13 Apr 2022 01:56:18 GMT  
		Size: 82.5 MB (82517343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc04eeb8271711ff970b4f435791f04f3b72dc527c8229db30cec017c886e3b`  
		Last Modified: Wed, 13 Apr 2022 01:55:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cdf04fcf2fb593c617dc77baaf17ec9f0e0e20e335cd5390efdeca26ac9cc98`  
		Last Modified: Wed, 13 Apr 2022 01:55:53 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f195575b52ef85f1a58bbc0ddb9de9f700ced9d743caa3b58bfbf6da781d640`  
		Last Modified: Wed, 22 Jun 2022 04:40:32 GMT  
		Size: 3.1 MB (3130581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed50e27180b1986fdef767475bfe0e518fc5d167c0b60d3100da8ed7c7478c9`  
		Last Modified: Wed, 22 Jun 2022 04:40:41 GMT  
		Size: 70.5 MB (70513778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690871ee2c4d9b6b50e4132f6af255f88fb86a483f18b17aec17c5d523c4c07b`  
		Last Modified: Wed, 22 Jun 2022 04:40:31 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; s390x

```console
$ docker pull redmine@sha256:402d4d8155a36989d3f7ed349188b7eaae93f500399b23a2c7a77cfa4304af29
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.5 MB (183480400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7352c2b89d8f45ab5e83bb77cdb92ae46e4800995b0c2c949f33697eedfdf11e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:06:05 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 05 Apr 2022 03:06:05 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 05 Apr 2022 03:06:06 GMT
ENV LANG=C.UTF-8
# Tue, 05 Apr 2022 03:11:43 GMT
ENV RUBY_MAJOR=3.1
# Tue, 12 Apr 2022 18:54:34 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 12 Apr 2022 18:54:35 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 12 Apr 2022 18:56:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 18:56:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 18:56:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 18:56:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 18:56:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 18:56:46 GMT
CMD ["irb"]
# Wed, 13 Apr 2022 00:39:34 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 13 Apr 2022 00:39:45 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 13 Apr 2022 00:39:49 GMT
ENV RAILS_ENV=production
# Wed, 13 Apr 2022 00:39:49 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Apr 2022 00:39:49 GMT
ENV HOME=/home/redmine
# Wed, 13 Apr 2022 00:39:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:15:43 GMT
ENV REDMINE_VERSION=5.0.2
# Wed, 22 Jun 2022 02:15:43 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Wed, 22 Jun 2022 02:15:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Wed, 22 Jun 2022 02:15:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:15:46 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 02:17:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 02:17:27 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:17:27 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 02:17:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:17:28 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:17:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484780568a7f85c870bca6482c56710f757b9fd31063067252af05a894e84045`  
		Last Modified: Tue, 05 Apr 2022 03:33:48 GMT  
		Size: 3.7 MB (3746194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44d92e36f1d6302319eff054b88ad602f3893de5945ec41945f11d8e1ffa6ca`  
		Last Modified: Tue, 05 Apr 2022 03:33:47 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223d9e260c5f9a45910eac9c6204f12eaa29268bcd7c855d31ac6e96a3d5899e`  
		Last Modified: Tue, 12 Apr 2022 20:01:32 GMT  
		Size: 29.4 MB (29364776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a472715d8ed4f0edafea3420f8c8ba3da1a15c9502f075ffc7a18927272c917f`  
		Last Modified: Tue, 12 Apr 2022 20:01:29 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a5ad19d546a17d3d49a62a6c3a157df23a9451ba9831c2145a5e101a167655`  
		Last Modified: Wed, 13 Apr 2022 00:52:40 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18a851fb597b97758ef798643f9aa524c066f807651a37293c4ca4c212c66210`  
		Last Modified: Wed, 13 Apr 2022 00:52:51 GMT  
		Size: 74.4 MB (74359309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d367421e26654c6dd344e4fa06a2b79a3a935d484fd56584efcc7dd1266a65`  
		Last Modified: Wed, 13 Apr 2022 00:52:39 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eee578b419584e4e0164c14d4c2efc464e8a211dd442bcb71eb50c70272d6989`  
		Last Modified: Wed, 13 Apr 2022 00:52:39 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a623d6eaae1475fbfdd3403f5d7fa251c867d70a8084327ad8c79427da3ba4`  
		Last Modified: Wed, 22 Jun 2022 02:23:00 GMT  
		Size: 3.1 MB (3130581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5494beb2f0434e9279ff15f5e261e46b4e2cc9e939469da6876dd9519a9802b9`  
		Last Modified: Wed, 22 Jun 2022 02:23:05 GMT  
		Size: 70.3 MB (70275425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463ce277c5d4e1bc89d643c5a40b96f2671f809594ea861d68e8edf71e770689`  
		Last Modified: Wed, 22 Jun 2022 02:22:59 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
