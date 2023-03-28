## `redmine:5-alpine`

```console
$ docker pull redmine@sha256:8fddda8b90e466cfa5ac36b0a8ccec166224485ad3358566a6c2c00c1d540b8d
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
$ docker pull redmine@sha256:5f7bfebbf66b4d0b4b84b5cde0a9aaaa0e4b2708e24cb333e8bffce7d17e7588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.8 MB (199791392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60e1646a33d195bcec8bdaf1c703c733e4d069dc09ffde583b72ca8de96a9554`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 13:34:26 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 11 Feb 2023 13:34:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 11 Feb 2023 13:34:27 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 13:40:20 GMT
ENV RUBY_MAJOR=3.1
# Sat, 11 Feb 2023 13:40:20 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 11 Feb 2023 13:40:20 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 11 Feb 2023 13:42:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 13:42:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 13:42:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 13:42:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 13:42:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 11 Feb 2023 13:42:51 GMT
CMD ["irb"]
# Sat, 11 Feb 2023 17:13:50 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 11 Feb 2023 17:13:58 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 11 Feb 2023 17:13:59 GMT
ENV RAILS_ENV=production
# Sat, 11 Feb 2023 17:13:59 GMT
WORKDIR /usr/src/redmine
# Sat, 11 Feb 2023 17:13:59 GMT
ENV HOME=/home/redmine
# Sat, 11 Feb 2023 17:14:00 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 06 Mar 2023 23:22:53 GMT
ENV REDMINE_VERSION=5.0.5
# Mon, 06 Mar 2023 23:22:53 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Mon, 06 Mar 2023 23:22:53 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Mon, 06 Mar 2023 23:22:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 06 Mar 2023 23:22:57 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 06 Mar 2023 23:24:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 06 Mar 2023 23:24:53 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 06 Mar 2023 23:24:53 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Mon, 06 Mar 2023 23:24:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Mar 2023 23:24:53 GMT
EXPOSE 3000
# Mon, 06 Mar 2023 23:24:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4e7d65ccdcf8803658fd95287533dcaeab1267d1c6f5675ba0d3c8ee08148e`  
		Last Modified: Sat, 11 Feb 2023 13:49:20 GMT  
		Size: 3.9 MB (3851507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923958f2c001452ff5d4adb46921384aa6f4e085ca364ec30ca4055fea99eec0`  
		Last Modified: Sat, 11 Feb 2023 13:49:19 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4255ad62eacbd87e5b5242ba5ae0bbc392244979e1a9bfea966e4aa1f65dea58`  
		Last Modified: Sat, 11 Feb 2023 13:49:59 GMT  
		Size: 29.3 MB (29318962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b0161c835d42b16d6249cf235d0814cadc501abefa302ee8c929cf259c771c`  
		Last Modified: Sat, 11 Feb 2023 13:49:56 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25812b6945b6e62ba35136b5784ea2eeb52fa25657782b45ac445ce34c3b6604`  
		Last Modified: Sat, 11 Feb 2023 17:19:12 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600d6d21020f13bb31144f05ea85b31f506f5b0669ee20e4a3936c5116a45586`  
		Last Modified: Sat, 11 Feb 2023 17:19:26 GMT  
		Size: 90.4 MB (90427713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462d1612167bc16ac24588a8aded45df27a4159e332114d94891c7a6657419f7`  
		Last Modified: Sat, 11 Feb 2023 17:19:10 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74eacda2c4b5b1fb59a87c84d3a621a83d808dfbae4f8824e058b4187cc5fba`  
		Last Modified: Sat, 11 Feb 2023 17:19:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386bea0e08e95ffdc7825865fe156979bc5342fa1e1333c94031e448a0dc2df`  
		Last Modified: Mon, 06 Mar 2023 23:29:47 GMT  
		Size: 3.1 MB (3145747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff8d86945551d9ea943e240d4a85882d3102d3f2457f59872f879214c597c1c`  
		Last Modified: Mon, 06 Mar 2023 23:29:53 GMT  
		Size: 70.2 MB (70235765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a69b9cf113f271f516489eeef269b36e291600a647923ca89c5bfee9f2b49f`  
		Last Modified: Mon, 06 Mar 2023 23:29:46 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:0f62b0f79850b30e50eb1c7013fbaa5414f3e3006c4f1ae7572df670f9b8c9d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190073558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:343e3fdeafaac84d869c9b4444129fa8c9892cea6b210cc1cc27cbe5d606ca27`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:48 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Mon, 13 Mar 2023 16:12:48 GMT
CMD ["/bin/sh"]
# Tue, 14 Mar 2023 01:14:18 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 14 Mar 2023 01:14:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 14 Mar 2023 01:14:19 GMT
ENV LANG=C.UTF-8
# Tue, 14 Mar 2023 01:19:50 GMT
ENV RUBY_MAJOR=3.1
# Tue, 14 Mar 2023 01:19:50 GMT
ENV RUBY_VERSION=3.1.3
# Tue, 14 Mar 2023 01:19:50 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Tue, 14 Mar 2023 01:22:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 14 Mar 2023 01:22:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 14 Mar 2023 01:22:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 14 Mar 2023 01:22:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Mar 2023 01:22:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 14 Mar 2023 01:22:09 GMT
CMD ["irb"]
# Tue, 14 Mar 2023 03:43:39 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 14 Mar 2023 03:43:50 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 14 Mar 2023 03:43:51 GMT
ENV RAILS_ENV=production
# Tue, 14 Mar 2023 03:43:51 GMT
WORKDIR /usr/src/redmine
# Tue, 14 Mar 2023 03:43:51 GMT
ENV HOME=/home/redmine
# Tue, 14 Mar 2023 03:43:52 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 14 Mar 2023 03:43:52 GMT
ENV REDMINE_VERSION=5.0.5
# Tue, 14 Mar 2023 03:43:52 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Tue, 14 Mar 2023 03:43:52 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Tue, 14 Mar 2023 03:43:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 14 Mar 2023 03:43:56 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 14 Mar 2023 03:45:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 14 Mar 2023 03:45:52 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 14 Mar 2023 03:45:52 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Tue, 14 Mar 2023 03:45:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 14 Mar 2023 03:45:52 GMT
EXPOSE 3000
# Tue, 14 Mar 2023 03:45:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0132b5bdd126bb1b7576ddcef71a13a530565fd53458494aeca9480ad96f9cc8`  
		Last Modified: Tue, 14 Mar 2023 01:28:37 GMT  
		Size: 3.6 MB (3593973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb87de5934988da7629054ce766b99def9ba6732354c326e725105e3086fff6`  
		Last Modified: Tue, 14 Mar 2023 01:28:36 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cace38b98b5db48114d438de4c0b179205e86f0992c06150cda65b79cf2b466a`  
		Last Modified: Tue, 14 Mar 2023 01:29:18 GMT  
		Size: 28.3 MB (28266753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c479a24e2932180b5086d6e624b38467892a3280f89a68efcc9f90741bd452`  
		Last Modified: Tue, 14 Mar 2023 01:29:14 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d68210b9c353a121fd344b0b82f660836ac9ca3e74fea6606c1ab085b395b7a`  
		Last Modified: Tue, 14 Mar 2023 03:49:16 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bafd854f4991243773e98c1265fbba9f728428028fa89d6969c4a7b9f56a82d2`  
		Last Modified: Tue, 14 Mar 2023 03:49:29 GMT  
		Size: 83.9 MB (83937031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865cbe12f5d65778a41fbff6b5de1a572f12142ba94906b256fdd68450c4ce0d`  
		Last Modified: Tue, 14 Mar 2023 03:49:14 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:925c297b9837f8b94836ba240fc24aa7b587881e5ec27de4df3fa6e5aa091320`  
		Last Modified: Tue, 14 Mar 2023 03:49:14 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7910c65652b0608ea44c315631bea668011f33f56cf112df9d08528e70eec9f8`  
		Last Modified: Tue, 14 Mar 2023 03:49:15 GMT  
		Size: 3.1 MB (3146035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:418f4843f633d11748c880caed05154aa7e9a474db0132d79f61551fcc5e3433`  
		Last Modified: Tue, 14 Mar 2023 03:49:22 GMT  
		Size: 68.5 MB (68509051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82506b0925368f0e82d2aa08b327cd3dfa43af6896b47d4ce76f5545fdcabf1b`  
		Last Modified: Tue, 14 Mar 2023 03:49:14 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:f9f56a4cf790139685acf1b445d7c4ae28f4456ad791a7f0becac7d6c962898d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187360933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6b99b3a4dc0f2483ce2fc055ff8a8fce26e47298d52487c9897007978571677`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 16:04:56 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Mar 2023 16:04:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Mar 2023 16:04:57 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 16:17:35 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Mar 2023 16:17:35 GMT
ENV RUBY_VERSION=3.1.3
# Wed, 01 Mar 2023 16:17:35 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Wed, 01 Mar 2023 16:19:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Mar 2023 16:19:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Mar 2023 16:19:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Mar 2023 16:19:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 16:19:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Mar 2023 16:19:40 GMT
CMD ["irb"]
# Thu, 02 Mar 2023 06:02:16 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 02 Mar 2023 06:02:31 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 02 Mar 2023 06:02:32 GMT
ENV RAILS_ENV=production
# Thu, 02 Mar 2023 06:02:32 GMT
WORKDIR /usr/src/redmine
# Thu, 02 Mar 2023 06:02:32 GMT
ENV HOME=/home/redmine
# Thu, 02 Mar 2023 06:02:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 06 Mar 2023 23:02:24 GMT
ENV REDMINE_VERSION=5.0.5
# Mon, 06 Mar 2023 23:02:24 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Mon, 06 Mar 2023 23:02:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Mon, 06 Mar 2023 23:02:28 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 06 Mar 2023 23:02:28 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 06 Mar 2023 23:04:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 06 Mar 2023 23:04:23 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 06 Mar 2023 23:04:23 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Mon, 06 Mar 2023 23:04:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Mar 2023 23:04:24 GMT
EXPOSE 3000
# Mon, 06 Mar 2023 23:04:24 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214aac296163a38eb76bb616c6d1d2dc5367a08bd74eb49d89d48c962a6b8d47`  
		Last Modified: Wed, 01 Mar 2023 16:43:49 GMT  
		Size: 3.5 MB (3461759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4b7b1669714566580ec7dd80dba5dff277b86af15cd3ec65587be7eb872bb6`  
		Last Modified: Wed, 01 Mar 2023 16:43:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef46c43dc463386a82aedaf4169282f6eda9c6b3a1a1ccacc0361d829c9b3541`  
		Last Modified: Wed, 01 Mar 2023 16:45:37 GMT  
		Size: 28.1 MB (28145581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389f27ad2c4e7fee3795404459bbd1a27b9fb7eb0afdb454894f5af11ed90972`  
		Last Modified: Wed, 01 Mar 2023 16:45:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de8d4cbb810a24671e05d4d8ce23747d2742961cfa53b20d1068c8be4b5f96a`  
		Last Modified: Thu, 02 Mar 2023 06:11:38 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d8eb7726f2c3d7d9db062789fb1b1661a89ab3648f1dad72d0efa328cfa891`  
		Last Modified: Thu, 02 Mar 2023 06:11:50 GMT  
		Size: 82.1 MB (82058975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34789e3967333a8c844316a53bf88b72d4d28b6cf03cb8db29fd74275c02af7d`  
		Last Modified: Thu, 02 Mar 2023 06:11:35 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f6a77f31fe7ee53f1b8e2fd82d15782bead651beefd21e0af4215082c71a96`  
		Last Modified: Thu, 02 Mar 2023 06:11:35 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f9f3ef69d888c97808371870f208ccb030f69087fde6c662519bd9ed37a625`  
		Last Modified: Mon, 06 Mar 2023 23:10:59 GMT  
		Size: 3.1 MB (3145785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b718ba8111c7f50ae43197141582fc83fb082705c61117af5a60a7d44646ac60`  
		Last Modified: Mon, 06 Mar 2023 23:11:05 GMT  
		Size: 68.1 MB (68124404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca339d3ecb98c1e36dc9df8d7ee7ddd55f155a5fc85b57e4221dd9bb665e6179`  
		Last Modified: Mon, 06 Mar 2023 23:10:58 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:5034d73a104cc693058c30b43e00f95a563012ac74acc78b4a0e2c8063e4c7a5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.6 MB (195563491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4f8f39aabef3fb8ade43ce4617b1b0d59d4a2b7f0d4e49f8a0aa8abdaea9c2e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:24:39 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 11 Feb 2023 05:24:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 11 Feb 2023 05:24:40 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 05:29:01 GMT
ENV RUBY_MAJOR=3.1
# Sat, 11 Feb 2023 05:29:01 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 11 Feb 2023 05:29:01 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 11 Feb 2023 05:30:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 05:30:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 05:30:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 05:30:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:30:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 11 Feb 2023 05:30:47 GMT
CMD ["irb"]
# Sat, 11 Feb 2023 08:47:33 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 11 Feb 2023 08:47:40 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 11 Feb 2023 08:47:41 GMT
ENV RAILS_ENV=production
# Sat, 11 Feb 2023 08:47:42 GMT
WORKDIR /usr/src/redmine
# Sat, 11 Feb 2023 08:47:42 GMT
ENV HOME=/home/redmine
# Sat, 11 Feb 2023 08:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 06 Mar 2023 23:49:33 GMT
ENV REDMINE_VERSION=5.0.5
# Mon, 06 Mar 2023 23:49:33 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Mon, 06 Mar 2023 23:49:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Mon, 06 Mar 2023 23:49:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 06 Mar 2023 23:49:36 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 06 Mar 2023 23:51:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 06 Mar 2023 23:51:15 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 06 Mar 2023 23:51:15 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Mon, 06 Mar 2023 23:51:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Mar 2023 23:51:15 GMT
EXPOSE 3000
# Mon, 06 Mar 2023 23:51:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ae7b7f5917829253477e9642f2e3c23ec4e6a33f1ae179614c91f494467276`  
		Last Modified: Sat, 11 Feb 2023 05:36:32 GMT  
		Size: 3.8 MB (3821424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6b4911b6d1550a57612d9b499d0be2d7a2118c74eb55879e24b81293e1598c`  
		Last Modified: Sat, 11 Feb 2023 05:36:32 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c51d6d874baf488729dfe61bbdce951d31f6260d36d4ce5daab30a3879ef096`  
		Last Modified: Sat, 11 Feb 2023 05:37:09 GMT  
		Size: 28.7 MB (28704392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88b191d91f98afa72d4fbf85fd9f1f589571b0888591d855eaf8e69d7fea41da`  
		Last Modified: Sat, 11 Feb 2023 05:37:06 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d0077d6f6189e0c3efbca9d4dc9ad1792ec95dbe3ebb0e34ce017f7595295f`  
		Last Modified: Sat, 11 Feb 2023 08:52:23 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135a1b0a2518e1d97c1a12ef83c36f243633e8be64b592c738660d1391530b2a`  
		Last Modified: Sat, 11 Feb 2023 08:52:32 GMT  
		Size: 87.3 MB (87292751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2506857d1f04329a0725a514a747b5f5fce679027a07604cd8de827acd61dc27`  
		Last Modified: Sat, 11 Feb 2023 08:52:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf0dcb764cdac1a39add787f8d3cd6c37fee6869ab688780346777571b858bf`  
		Last Modified: Sat, 11 Feb 2023 08:52:21 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec95b5f9ac5718abc8825e0ea2e6716c1e9674f546ea5fef7d31b238df60ff7d`  
		Last Modified: Mon, 06 Mar 2023 23:55:24 GMT  
		Size: 3.1 MB (3145789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5d4c97660a3b0474f9f2e1a2c1112dbdfc14123bed9f7761f5cb144106ef50f`  
		Last Modified: Mon, 06 Mar 2023 23:55:29 GMT  
		Size: 69.9 MB (69885693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8769b12ec0e12c2dec31df5b8d9aae53ecf8a219163ed082619a8635915fa39`  
		Last Modified: Mon, 06 Mar 2023 23:55:24 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; 386

```console
$ docker pull redmine@sha256:c2245df7eb393f97098042d96959a97b16a5c77df0100ca2a5b57209d76bd29b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.1 MB (197077684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a10f4966ef0091c3d762c5b6a96b74f83ffa907766ceca1cd0b7c9286d410323`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:29 GMT
ADD file:59ac1f8f33f9b9727892b7e45b33f54ef3c20d9d876c49d6a4c057641821d68f in / 
# Fri, 10 Feb 2023 21:24:29 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 08:09:16 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Mar 2023 08:09:17 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Mar 2023 08:09:17 GMT
ENV LANG=C.UTF-8
# Wed, 01 Mar 2023 08:31:24 GMT
ENV RUBY_MAJOR=3.1
# Wed, 01 Mar 2023 08:31:24 GMT
ENV RUBY_VERSION=3.1.3
# Wed, 01 Mar 2023 08:31:24 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Wed, 01 Mar 2023 08:35:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Mar 2023 08:35:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Mar 2023 08:35:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Mar 2023 08:35:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 08:35:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Mar 2023 08:35:54 GMT
CMD ["irb"]
# Thu, 02 Mar 2023 05:30:38 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 02 Mar 2023 05:30:54 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 02 Mar 2023 05:30:55 GMT
ENV RAILS_ENV=production
# Thu, 02 Mar 2023 05:30:55 GMT
WORKDIR /usr/src/redmine
# Thu, 02 Mar 2023 05:30:55 GMT
ENV HOME=/home/redmine
# Thu, 02 Mar 2023 05:30:56 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 06 Mar 2023 23:45:45 GMT
ENV REDMINE_VERSION=5.0.5
# Mon, 06 Mar 2023 23:45:45 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Mon, 06 Mar 2023 23:45:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Mon, 06 Mar 2023 23:45:49 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 06 Mar 2023 23:45:49 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 06 Mar 2023 23:58:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 06 Mar 2023 23:58:41 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 06 Mar 2023 23:58:41 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Mon, 06 Mar 2023 23:58:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Mar 2023 23:58:41 GMT
EXPOSE 3000
# Mon, 06 Mar 2023 23:58:41 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0987f51cd58a7d03bc7d6ff0a3a0a843c1a3fefcd41e3c8adc3999ddde7441e8`  
		Last Modified: Fri, 10 Feb 2023 21:25:30 GMT  
		Size: 2.8 MB (2810653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb12ab4bddc203e01d991aaa7e219d7cf59308ea03a841856dadb2eb766a5fb`  
		Last Modified: Wed, 01 Mar 2023 09:12:27 GMT  
		Size: 3.9 MB (3886739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662c6bb99b5e3818a910af731b41c1ee06abfac00cfc2ac5bbbed96103772ac4`  
		Last Modified: Wed, 01 Mar 2023 09:12:26 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b27ee94b1520cbb9de3ca15d0eb2215a4c59ae0f34ec971e25846bf8a50591ef`  
		Last Modified: Wed, 01 Mar 2023 09:14:14 GMT  
		Size: 28.1 MB (28119168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9765f341e98667e0752b93702526a4704f44c07c4012f37c69e6574f978262bd`  
		Last Modified: Wed, 01 Mar 2023 09:14:10 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0ba32b7e61830ac8d24e56ce4f07c5b44aca020a82137a75fb54ca5db79d8d`  
		Last Modified: Thu, 02 Mar 2023 05:40:30 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80af23114920d9f563537297dc73da7899d020565469f3fb88e9db3727061f95`  
		Last Modified: Thu, 02 Mar 2023 05:40:49 GMT  
		Size: 90.3 MB (90301871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17648fa9a947a071cc609ff242fe3b56a36365f823e4984cf4ea21295ea83de3`  
		Last Modified: Thu, 02 Mar 2023 05:40:28 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55027addb98b66b5f233b60c8871f232b56105a48a16cca893856221cb5dd0f`  
		Last Modified: Thu, 02 Mar 2023 05:40:28 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92840650204b3a11f49ebc7650829f8b596015a7e0c93760b47195c42b9bdc99`  
		Last Modified: Tue, 07 Mar 2023 00:04:27 GMT  
		Size: 3.1 MB (3145818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e202eaeb442a5c2dc4955dca72ccb785f531b0003ad6b173077cd3440a13b06`  
		Last Modified: Tue, 07 Mar 2023 00:04:34 GMT  
		Size: 68.8 MB (68809495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8517a5ea3c787a7c9cb6e6ce127025c70c37c2d99203a31552f42980d7be78`  
		Last Modified: Tue, 07 Mar 2023 00:04:26 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; ppc64le

```console
$ docker pull redmine@sha256:7dc1066891a6b7014b9730fe8a8371250b92f0f34c222b749870cfc380e044ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.8 MB (206817187 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b97d5da11caa721e1711b06c9b141cff17fa785f045609f74a17710b9c4ebb40`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:07:34 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 11 Feb 2023 05:07:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 11 Feb 2023 05:07:37 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 05:15:47 GMT
ENV RUBY_MAJOR=3.1
# Sat, 11 Feb 2023 05:15:48 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 11 Feb 2023 05:15:48 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 11 Feb 2023 05:19:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 05:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 05:19:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 05:19:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:19:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 11 Feb 2023 05:19:55 GMT
CMD ["irb"]
# Sat, 11 Feb 2023 12:53:49 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 11 Feb 2023 12:54:19 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 11 Feb 2023 12:54:23 GMT
ENV RAILS_ENV=production
# Sat, 11 Feb 2023 12:54:23 GMT
WORKDIR /usr/src/redmine
# Sat, 11 Feb 2023 12:54:24 GMT
ENV HOME=/home/redmine
# Sat, 11 Feb 2023 12:54:25 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 06 Mar 2023 23:22:48 GMT
ENV REDMINE_VERSION=5.0.5
# Mon, 06 Mar 2023 23:22:48 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Mon, 06 Mar 2023 23:22:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Mon, 06 Mar 2023 23:22:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 06 Mar 2023 23:22:58 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 06 Mar 2023 23:27:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 06 Mar 2023 23:27:10 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 06 Mar 2023 23:27:10 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Mon, 06 Mar 2023 23:27:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Mar 2023 23:27:11 GMT
EXPOSE 3000
# Mon, 06 Mar 2023 23:27:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d1835bdc86ca722641491b8c05548ca1f17a52cc1d2d4f0aeb4abcc43cea0`  
		Last Modified: Sat, 11 Feb 2023 05:31:35 GMT  
		Size: 4.0 MB (3973616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1cd4eb351e56ba7e4fbe068d8f88ebb2fa8b6fc8b162f8896fbb12f5baf3dc`  
		Last Modified: Sat, 11 Feb 2023 05:31:33 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f59468b845721d3f7d411c9ee83aef16b26bc6790535520a5242a0d9ae2c35a`  
		Last Modified: Sat, 11 Feb 2023 05:32:32 GMT  
		Size: 29.5 MB (29517487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45df66a1d71856e3cac53e9e15e404719c6b60f77a9d8fdadf86d1dd30311259`  
		Last Modified: Sat, 11 Feb 2023 05:32:26 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73bcbd47603460add4c7423a07973950c38e2bf2e310a03a74555659a6da5bc3`  
		Last Modified: Sat, 11 Feb 2023 13:05:19 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a33833b9c8729972df1ad4bfe6f3c874e5fc5bf70d19f3cd5ee7bd418986e02`  
		Last Modified: Sat, 11 Feb 2023 13:05:43 GMT  
		Size: 96.3 MB (96318022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69189681e3f0f084375722142f17fcf76da532258cae113d76d965dfe0557771`  
		Last Modified: Sat, 11 Feb 2023 13:05:16 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5f33d0c40ba5e732d391fad4d05b8ff8b5adf6d716ca1de350ea98c587399`  
		Last Modified: Sat, 11 Feb 2023 13:05:16 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:483dc1b3e0db6836e9526de5eecd304462a76e1c7da92cb3796db872b010221f`  
		Last Modified: Mon, 06 Mar 2023 23:38:46 GMT  
		Size: 3.1 MB (3145840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe76161a6ae4998a1ed91d3c2ce19e3c491b52623c9741d58d0ec68fa93f229`  
		Last Modified: Mon, 06 Mar 2023 23:38:57 GMT  
		Size: 71.1 MB (71053659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492b42f3cb1bc5a92841840bf835aa34441a77fe5a1964a378a49e7eaf953dbd`  
		Last Modified: Mon, 06 Mar 2023 23:38:45 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; s390x

```console
$ docker pull redmine@sha256:6879b525ac458bde4bf66b2be469ac97265b5c213bd547b112321f76de437c3e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.3 MB (191300603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:accf4ce94fbe2a596ec1cd0a8604d61019d3fa53778bbb8c0c8a6e549529ff98`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:50:29 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 11 Feb 2023 10:50:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 11 Feb 2023 10:50:30 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 10:56:36 GMT
ENV RUBY_MAJOR=3.1
# Sat, 11 Feb 2023 10:56:37 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 11 Feb 2023 10:56:38 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 11 Feb 2023 11:00:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 11:00:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 11:00:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 11:00:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 28 Mar 2023 00:12:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Tue, 28 Mar 2023 00:12:22 GMT
CMD ["irb"]
# Tue, 28 Mar 2023 02:43:16 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 28 Mar 2023 02:43:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 28 Mar 2023 02:43:33 GMT
ENV RAILS_ENV=production
# Tue, 28 Mar 2023 02:43:33 GMT
WORKDIR /usr/src/redmine
# Tue, 28 Mar 2023 02:43:33 GMT
ENV HOME=/home/redmine
# Tue, 28 Mar 2023 02:43:33 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 28 Mar 2023 02:43:33 GMT
ENV REDMINE_VERSION=5.0.5
# Tue, 28 Mar 2023 02:43:34 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Tue, 28 Mar 2023 02:43:34 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Tue, 28 Mar 2023 02:43:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 28 Mar 2023 02:43:38 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 28 Mar 2023 02:45:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 28 Mar 2023 02:45:25 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 28 Mar 2023 02:45:25 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Tue, 28 Mar 2023 02:45:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 28 Mar 2023 02:45:26 GMT
EXPOSE 3000
# Tue, 28 Mar 2023 02:45:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efdc9ea63066cf1780bbe5fb37efb05fc41715ccf7d1d4ada643b9980615fb10`  
		Last Modified: Sat, 11 Feb 2023 11:08:24 GMT  
		Size: 3.9 MB (3941065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b409ba260ab77b4a8e266f8ecc6dbe5fed29ada1c062c2a6195dd869bbc20e94`  
		Last Modified: Sat, 11 Feb 2023 11:08:23 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad51e92f4adea8480df38fc926f55cebec15a6449ba559d1a01836c7b02b852`  
		Last Modified: Sat, 11 Feb 2023 11:08:57 GMT  
		Size: 28.9 MB (28925746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015fdbf921b55243bceabf5f85148a771ba6deddb1249a4d3fd14dc68f3f1237`  
		Last Modified: Tue, 28 Mar 2023 00:14:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098cb608e358db84f30d9c812b4d18d263181b93e542a4ca2160b44cc0dc0551`  
		Last Modified: Tue, 28 Mar 2023 02:50:41 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dad3e4027882d360dd11d516082c92501ee9e31f1c9cc803463bdb712db5c45`  
		Last Modified: Tue, 28 Mar 2023 02:50:51 GMT  
		Size: 80.9 MB (80871002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f579539f3010bf1292485d78360f8030aa1bff644292de006df49f29726927`  
		Last Modified: Tue, 28 Mar 2023 02:50:40 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77b7b4a43708a0f4dc98dcef6857322a33a9d2e65a6a5007eb5a541f6dd4a12`  
		Last Modified: Tue, 28 Mar 2023 02:50:40 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd6a80c748a80330e0dcd68651f054c890dcce055de0d6541665b87a174b96d`  
		Last Modified: Tue, 28 Mar 2023 02:50:40 GMT  
		Size: 3.1 MB (3145977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43738f1c5ca1c217bc8ccb4bf9cb399228aae78981c4863675a6b3cd6e90941`  
		Last Modified: Tue, 28 Mar 2023 02:50:46 GMT  
		Size: 71.8 MB (71819290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c4c04f7e4d5f638c023fba17fc72568203a118211c705f0e3de6dd4ee93846`  
		Last Modified: Tue, 28 Mar 2023 02:50:40 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
