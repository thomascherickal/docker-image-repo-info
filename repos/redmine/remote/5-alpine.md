## `redmine:5-alpine`

```console
$ docker pull redmine@sha256:754bd3843c37e97ade78ba5a8c814455cf326794d276d30542ccf032e5bb4a94
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
$ docker pull redmine@sha256:d5ed91fbf1faf2b35c72a64ad00285ff61ad8b6f3c83d9d9e55572c5e1e61de6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.1 MB (200064471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:588a1e6fa99e7da2a71a602e5056d4bf3fd0c96a68ec47817ca7fc498d00834c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 22:37:25 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 11 May 2023 22:37:26 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 11 May 2023 22:37:26 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:40:25 GMT
ENV RUBY_MAJOR=3.1
# Thu, 11 May 2023 22:40:25 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 11 May 2023 22:40:25 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 11 May 2023 22:42:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 11 May 2023 22:42:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 11 May 2023 22:42:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 11 May 2023 22:42:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 22:42:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 11 May 2023 22:42:38 GMT
CMD ["irb"]
# Tue, 13 Jun 2023 23:23:59 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 13 Jun 2023 23:24:07 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 13 Jun 2023 23:24:08 GMT
ENV RAILS_ENV=production
# Tue, 13 Jun 2023 23:24:08 GMT
WORKDIR /usr/src/redmine
# Tue, 13 Jun 2023 23:24:08 GMT
ENV HOME=/home/redmine
# Tue, 13 Jun 2023 23:24:08 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 13 Jun 2023 23:24:08 GMT
ENV REDMINE_VERSION=5.0.5
# Tue, 13 Jun 2023 23:24:08 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Tue, 13 Jun 2023 23:24:09 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Tue, 13 Jun 2023 23:24:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 13 Jun 2023 23:24:12 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 13 Jun 2023 23:25:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 13 Jun 2023 23:25:53 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 13 Jun 2023 23:25:53 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Tue, 13 Jun 2023 23:25:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 23:25:53 GMT
EXPOSE 3000
# Tue, 13 Jun 2023 23:25:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3d25e339e798c7606304d1a00cff7f31a5876c66dec58866278476db2c83ea`  
		Last Modified: Thu, 11 May 2023 22:43:34 GMT  
		Size: 4.1 MB (4129286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75dd67f3ccc89561ff13877120b513941dc1e14c5ab32c4ce6d5585ee6ef9189`  
		Last Modified: Thu, 11 May 2023 22:43:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8543f06a28fde480630d4b61f2b1a367b6e3bd3684cd09179aa18914936d957c`  
		Last Modified: Thu, 11 May 2023 22:44:02 GMT  
		Size: 29.5 MB (29484606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b2a3a3ef6eecb7f8a8575ebae60d72ab5b63a312eaf2da612c224585984271`  
		Last Modified: Thu, 11 May 2023 22:44:00 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c866d729282323bb0e8c7376ad123c006a7ed0ba61fe7724aa1e59e9dd38b99b`  
		Last Modified: Tue, 13 Jun 2023 23:27:06 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b062cb80585e759b846f39f568f2889ad0f2ce436c0cdc4b90aa282679670e86`  
		Last Modified: Tue, 13 Jun 2023 23:27:17 GMT  
		Size: 87.3 MB (87272169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdda3125257f8cf7f2033d95b0e3ef5f032f55254d1ac5a7d854ebd324a2eee0`  
		Last Modified: Tue, 13 Jun 2023 23:27:04 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b85e285fed7517fb03f18d1e88d66641387e0bee4e756e94e75c55725903829`  
		Last Modified: Tue, 13 Jun 2023 23:27:04 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27b8c816ab2fdabcefc80d6eefec08ba09ccc575c3e6290bcd5621f80eae6186`  
		Last Modified: Tue, 13 Jun 2023 23:27:05 GMT  
		Size: 3.1 MB (3146026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11dec60283eda91aeeb91327a7f546d187b3c1fe35233004d103907b407116bb`  
		Last Modified: Tue, 13 Jun 2023 23:27:11 GMT  
		Size: 72.6 MB (72630955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af2db0b322fdf19ee29cb68f0b64816c7e153237f44a5f7af77fcf5a2455892`  
		Last Modified: Tue, 13 Jun 2023 23:27:04 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:99f798fe9898ae5b337b8e784cc1a48528b74e57ac86c1c997d28e4728d7dbb7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191855517 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25b0d1426eb1217b54b73c2e5bf533d388e039cd9730263a87cf4d923c5fb89`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 20:38:54 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 11 May 2023 20:38:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 11 May 2023 20:38:55 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 20:41:14 GMT
ENV RUBY_MAJOR=3.1
# Thu, 11 May 2023 20:41:14 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 11 May 2023 20:41:15 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 11 May 2023 20:43:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 11 May 2023 20:43:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 11 May 2023 20:43:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 11 May 2023 20:43:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:43:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 11 May 2023 20:43:19 GMT
CMD ["irb"]
# Tue, 13 Jun 2023 19:02:31 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 13 Jun 2023 19:02:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 13 Jun 2023 19:02:49 GMT
ENV RAILS_ENV=production
# Tue, 13 Jun 2023 19:02:49 GMT
WORKDIR /usr/src/redmine
# Tue, 13 Jun 2023 19:02:49 GMT
ENV HOME=/home/redmine
# Tue, 13 Jun 2023 19:02:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 13 Jun 2023 19:02:50 GMT
ENV REDMINE_VERSION=5.0.5
# Tue, 13 Jun 2023 19:02:50 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Tue, 13 Jun 2023 19:02:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Tue, 13 Jun 2023 19:02:53 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 13 Jun 2023 19:02:54 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 13 Jun 2023 19:04:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 13 Jun 2023 19:04:45 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 13 Jun 2023 19:04:45 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Tue, 13 Jun 2023 19:04:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 19:04:45 GMT
EXPOSE 3000
# Tue, 13 Jun 2023 19:04:46 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68626ddb38dbc0142d1a5c8199d67f7f230526d101faa64e1bdf1509a7ffd74`  
		Last Modified: Thu, 11 May 2023 20:43:40 GMT  
		Size: 3.8 MB (3805958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6dd69f2c8ad0227681b2c090d7e8e2fb833d2ad4bd82f028f734ac33200adb`  
		Last Modified: Thu, 11 May 2023 20:43:39 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c480a7bd894094f1d32bcc3a7f2f5b29cf7e0cb0482d7b8fb361d03b2a3d67`  
		Last Modified: Thu, 11 May 2023 20:44:09 GMT  
		Size: 28.4 MB (28356572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffed02495c755ee9a5f3326ceefbffbce9324bd9a0b4852da73890dff4935442`  
		Last Modified: Thu, 11 May 2023 20:44:05 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4fb6c4c7561741017fc24da3fd0d3353aee439e54e710b9d08454e84f4a8fc`  
		Last Modified: Tue, 13 Jun 2023 19:05:05 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2964d92f56bf382942d38cede92cbed1c7da27ac1828c841d86b178bac71d0e`  
		Last Modified: Tue, 13 Jun 2023 19:05:18 GMT  
		Size: 82.8 MB (82842093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7db88cdb524abfbe6f5e077da836d4ecdcb5826a995e730c78badcf7a6004d`  
		Last Modified: Tue, 13 Jun 2023 19:05:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c21706ab52fdaaff3a05d1ba4af372a4385d67ef8720df22e2307c6b0e1e61d`  
		Last Modified: Tue, 13 Jun 2023 19:05:02 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbfba301e39d043abca092a30c2e7149af4944ed8acfe0bf43690f450dd1350`  
		Last Modified: Tue, 13 Jun 2023 19:05:04 GMT  
		Size: 3.1 MB (3146051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ea2d23b7b1c39cb3b534d16321155a4900e08a51775dec2ccd6b9b93aa5659`  
		Last Modified: Tue, 13 Jun 2023 19:05:11 GMT  
		Size: 70.5 MB (70545229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f571c08182677116ec966d24c6c2ba49fea913941cf75da2b34ece8e6c84b3`  
		Last Modified: Tue, 13 Jun 2023 19:05:02 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:da786a1e6c8546d878b944daf938553601a33f8b117af2b9e7ede057917e432e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.5 MB (187455811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cb0f914aa5fff4ba99b5204132e4f1910f90bd4c8aa6269314ecfee3329b2bd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 23:12:39 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 11 May 2023 23:12:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 11 May 2023 23:12:39 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 23:14:49 GMT
ENV RUBY_MAJOR=3.1
# Thu, 11 May 2023 23:14:49 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 11 May 2023 23:14:50 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 11 May 2023 23:17:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 11 May 2023 23:17:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 11 May 2023 23:17:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 11 May 2023 23:17:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 23:17:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 11 May 2023 23:17:05 GMT
CMD ["irb"]
# Wed, 14 Jun 2023 01:10:39 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jun 2023 01:10:57 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 14 Jun 2023 01:10:58 GMT
ENV RAILS_ENV=production
# Wed, 14 Jun 2023 01:10:58 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jun 2023 01:10:59 GMT
ENV HOME=/home/redmine
# Wed, 14 Jun 2023 01:10:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jun 2023 01:10:59 GMT
ENV REDMINE_VERSION=5.0.5
# Wed, 14 Jun 2023 01:10:59 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Wed, 14 Jun 2023 01:10:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Wed, 14 Jun 2023 01:11:03 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jun 2023 01:11:03 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jun 2023 01:12:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jun 2023 01:12:52 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jun 2023 01:12:52 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Wed, 14 Jun 2023 01:12:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jun 2023 01:12:52 GMT
EXPOSE 3000
# Wed, 14 Jun 2023 01:12:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:881d5f89893194c7fe70e85fd230198fafa38ffb9668ec9b4488d19e60c3ffc6`  
		Last Modified: Thu, 11 May 2023 23:17:52 GMT  
		Size: 3.7 MB (3716134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b4804443f53674e374cb1a523509e7576f62016b760325acc63987c6a75cbc4`  
		Last Modified: Thu, 11 May 2023 23:17:51 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8105abaa3d63fc7483e76b937f318e7540bd5a94a690913eb675661733f7fe67`  
		Last Modified: Thu, 11 May 2023 23:18:22 GMT  
		Size: 28.2 MB (28226833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710dd8736f8e99c0a8523a9d934198ba1df08d517beea9447e946bb738a74b2b`  
		Last Modified: Thu, 11 May 2023 23:18:19 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438fa6d61c85e445c51fbe36d9c027dbc910c0047b653f421310827a5cc8483b`  
		Last Modified: Wed, 14 Jun 2023 01:13:55 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45809f2be32997b5a56ea42d19843913b6761b3190a00b1f7c94b1ff56e6631`  
		Last Modified: Wed, 14 Jun 2023 01:14:07 GMT  
		Size: 79.5 MB (79454925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fda916b43b6b365c975411121f2ed9859f8390ec8480644960411698ed8ff09`  
		Last Modified: Wed, 14 Jun 2023 01:13:53 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873ea320b604c063b0118d368078465166f8093400396ef831042311332ef7b6`  
		Last Modified: Wed, 14 Jun 2023 01:13:54 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc409487ac46ef8c57ce53b6f61cee5b360053151cb9ab52a9855b0c5d953f99`  
		Last Modified: Wed, 14 Jun 2023 01:13:54 GMT  
		Size: 3.1 MB (3145988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15c83da2ae951dcefdd9fddf72031f992c9a31719f4d9e716583dc869d77df0`  
		Last Modified: Wed, 14 Jun 2023 01:14:01 GMT  
		Size: 70.0 MB (69996876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b82c4ed083b80f72259c995ef6f4b7d9411604ec94ec831e69a962102112fe`  
		Last Modified: Wed, 14 Jun 2023 01:13:53 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:9f2d2e104c4b178d4893233b68c018a1754e51524788b912e6cc1661b7c6c4f0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.4 MB (198351356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c90dd779be8e1b7bbf0f70d7a6957071c192ddc0f30faa32f60f71adb3a45e79`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 23:08:56 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 11 May 2023 23:08:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 11 May 2023 23:08:57 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 23:11:08 GMT
ENV RUBY_MAJOR=3.1
# Thu, 11 May 2023 23:11:08 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 11 May 2023 23:11:08 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 11 May 2023 23:12:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 11 May 2023 23:12:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 11 May 2023 23:12:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 11 May 2023 23:12:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 23:12:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 11 May 2023 23:12:39 GMT
CMD ["irb"]
# Tue, 13 Jun 2023 21:56:32 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 13 Jun 2023 21:56:40 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 13 Jun 2023 21:56:41 GMT
ENV RAILS_ENV=production
# Tue, 13 Jun 2023 21:56:41 GMT
WORKDIR /usr/src/redmine
# Tue, 13 Jun 2023 21:56:41 GMT
ENV HOME=/home/redmine
# Tue, 13 Jun 2023 21:56:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 13 Jun 2023 21:56:42 GMT
ENV REDMINE_VERSION=5.0.5
# Tue, 13 Jun 2023 21:56:42 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Tue, 13 Jun 2023 21:56:42 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Tue, 13 Jun 2023 21:56:45 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 13 Jun 2023 21:56:46 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 13 Jun 2023 21:58:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 13 Jun 2023 21:58:11 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 13 Jun 2023 21:58:11 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Tue, 13 Jun 2023 21:58:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 21:58:12 GMT
EXPOSE 3000
# Tue, 13 Jun 2023 21:58:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8d08b30450c12a72939d3227c817154531f453653453d46d7d2a0708f4497d`  
		Last Modified: Thu, 11 May 2023 23:13:25 GMT  
		Size: 4.1 MB (4059781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b492009e1697af0a35d8344ae929d156f9d5e2d3ba72b1853aaee24f6bfa95`  
		Last Modified: Thu, 11 May 2023 23:13:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831bb4769cd713dde88dccba20919c346eb5a49bdeebfb7b2d034c667bec9ea3`  
		Last Modified: Thu, 11 May 2023 23:13:52 GMT  
		Size: 28.9 MB (28934219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c904c85f639aee0f916c284937bc4e2cf9cf883319456c954a23f6f9e4c99f3e`  
		Last Modified: Thu, 11 May 2023 23:13:50 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbb3dbc2ce27bbf0acd8666a9b76c0b4a17da9fee29992d7f5ade172e6caa8`  
		Last Modified: Tue, 13 Jun 2023 21:59:12 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4082d90641f15245fbf2b1b041d637d1d6d1738098c052ef0addbd8dd211ce1d`  
		Last Modified: Tue, 13 Jun 2023 21:59:21 GMT  
		Size: 86.7 MB (86721046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75b191bb97ae8b14b59242a63d5453350ecf0ade6fc09465b1ad99a8d9ce267`  
		Last Modified: Tue, 13 Jun 2023 21:59:10 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1f89bedca2a7f69323c903d5e9930b6fbf857d8fbac5b16f013660429a5cd8`  
		Last Modified: Tue, 13 Jun 2023 21:59:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d70f2bff8b92065c822df1db30fbc66ccb50d2d284712af01c7477554d67f5`  
		Last Modified: Tue, 13 Jun 2023 21:59:11 GMT  
		Size: 3.1 MB (3146031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b19a207be89f6ccdb335be12b8ce1952334978170b7130faa389fc486e784b6`  
		Last Modified: Tue, 13 Jun 2023 21:59:16 GMT  
		Size: 72.1 MB (72143493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a0216428cc8e22e6e41150fc7a83b06542c1f65dc6eaa7988610fc23adeb8a`  
		Last Modified: Tue, 13 Jun 2023 21:59:10 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; 386

```console
$ docker pull redmine@sha256:381bcb9dd318bfa0dbe2385dfc1af5045365ff3e9bad278186385b48d1cd6510
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.7 MB (193682999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9e57c4b840973786bcec35178bb23a4f1e0f833d6e648da9c4c3b3c7cd4b02e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 May 2023 23:11:03 GMT
ADD file:cfe47ebe49c4a75094234cafa52aa13aa26abcdad49b89293585884b3a8faeae in / 
# Tue, 09 May 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 12 May 2023 02:11:05 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 12 May 2023 02:11:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 12 May 2023 02:11:06 GMT
ENV LANG=C.UTF-8
# Fri, 12 May 2023 02:15:01 GMT
ENV RUBY_MAJOR=3.1
# Fri, 12 May 2023 02:15:01 GMT
ENV RUBY_VERSION=3.1.4
# Fri, 12 May 2023 02:15:01 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Fri, 12 May 2023 02:18:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 12 May 2023 02:18:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 12 May 2023 02:18:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 12 May 2023 02:18:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 12 May 2023 02:18:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Fri, 12 May 2023 02:18:38 GMT
CMD ["irb"]
# Tue, 13 Jun 2023 20:28:19 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 13 Jun 2023 20:28:34 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 13 Jun 2023 20:28:35 GMT
ENV RAILS_ENV=production
# Tue, 13 Jun 2023 20:28:35 GMT
WORKDIR /usr/src/redmine
# Tue, 13 Jun 2023 20:28:35 GMT
ENV HOME=/home/redmine
# Tue, 13 Jun 2023 20:28:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 13 Jun 2023 20:28:36 GMT
ENV REDMINE_VERSION=5.0.5
# Tue, 13 Jun 2023 20:28:36 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Tue, 13 Jun 2023 20:28:36 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Tue, 13 Jun 2023 20:28:40 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 13 Jun 2023 20:28:40 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 13 Jun 2023 20:30:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 13 Jun 2023 20:30:54 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 13 Jun 2023 20:30:54 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Tue, 13 Jun 2023 20:30:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Jun 2023 20:30:54 GMT
EXPOSE 3000
# Tue, 13 Jun 2023 20:30:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:613767c5530f4016482e81288d0efdca4e58c62031252130d8fccd6f6260a068`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.3 MB (3264862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2f7e49e02f6174cdf9fe877eb626bc516cc2ce9092dd72efa85af4770789e4`  
		Last Modified: Fri, 12 May 2023 02:19:38 GMT  
		Size: 4.1 MB (4135645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ec237fc1f4321ff6e992637bd34d973547180c8c744ba94a34baa08a9f2abc`  
		Last Modified: Fri, 12 May 2023 02:19:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e00675d16689b698ce84c8a4747335bdfcf1671302fd90be6e179eca46de38b`  
		Last Modified: Fri, 12 May 2023 02:20:10 GMT  
		Size: 28.2 MB (28226692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b55d5622dba8b538a13eba2ba3fcb72cedf9b510018c12b9e199af0fc3950ad`  
		Last Modified: Fri, 12 May 2023 02:20:06 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b83c6ae4c8e2a15026ea294b60cd8cdcae164d97b7a31ae07dc51dda5d6f6b0`  
		Last Modified: Tue, 13 Jun 2023 20:33:46 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dcbf9186f06a84b2532c5dd5f4477b46eae87de63261cb7ef86bcc854d1847b`  
		Last Modified: Tue, 13 Jun 2023 20:34:04 GMT  
		Size: 84.1 MB (84092983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddfe19c82062fbe88b4a79206c3cc1e8fe5395ef065715899bc343f32c1dc5b`  
		Last Modified: Tue, 13 Jun 2023 20:33:44 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47964f76106b0a7a257b782b010709343cd27c99b089174278fe80f9429ab54`  
		Last Modified: Tue, 13 Jun 2023 20:33:44 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f37021d983913478e019b47077a3944deaf0a343d2b8e0c40df0605d3b22b42`  
		Last Modified: Tue, 13 Jun 2023 20:33:46 GMT  
		Size: 3.1 MB (3146090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052308f1e2310d0f22407b9a3bd4945d4e47e1e38dcccee780380d1a7a84ed50`  
		Last Modified: Tue, 13 Jun 2023 20:33:55 GMT  
		Size: 70.8 MB (70812792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d759c8deba66997d46cbd416e0374c240e7ca132f90f283ee0102731f09e305`  
		Last Modified: Tue, 13 Jun 2023 20:33:55 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; ppc64le

```console
$ docker pull redmine@sha256:e1d8db54df6cb8de2c971bdce197ff38e11bc7d7b53e5cd9c17579df6ef9985f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.8 MB (206811389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0a38b4588a9714d5509f51117d0cc9d569bf1171ab8c72beca0241ba5aa28a1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:10:41 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 30 Mar 2023 04:10:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 30 Mar 2023 04:10:46 GMT
ENV LANG=C.UTF-8
# Thu, 30 Mar 2023 04:18:15 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 19:41:12 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:41:12 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:44:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:44:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:44:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:44:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:44:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:44:44 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 20:29:32 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 20:29:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 20:29:52 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 20:29:53 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 20:29:54 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 20:29:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 20:29:55 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 20:29:56 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 20:29:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 20:30:02 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 20:30:03 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 20:33:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 20:33:56 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 20:33:56 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 20:33:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 20:33:57 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 20:33:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98c697220ffba9acde6d37fcb16b5ccfd5f094e8f730ed282a01e7c2d7c2211`  
		Last Modified: Thu, 30 Mar 2023 04:30:46 GMT  
		Size: 4.0 MB (3973663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:493ec3a3209b2375deda630e78152d62b67aac8d3792af5404c85570ff55ffd2`  
		Last Modified: Thu, 30 Mar 2023 04:30:45 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a404b6a00c90f93250f37e19a96dc111bf1441c4d86ed43763569a8aaf2bbf2`  
		Last Modified: Thu, 30 Mar 2023 20:07:19 GMT  
		Size: 29.5 MB (29520666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6479310faba4821e8bdb6e8a1d5ed24bdd823f37ff28725ea8dd153756c5264b`  
		Last Modified: Thu, 30 Mar 2023 20:07:13 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1882df7c78964a106af80c3600a813d749615cc067a6ba233fa3e023e096be`  
		Last Modified: Thu, 30 Mar 2023 20:45:56 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd97506b5c9e9de08438d1b9e9d2044ffd85bc778cf0b4c6b704b3e0f5490da6`  
		Last Modified: Thu, 30 Mar 2023 20:46:19 GMT  
		Size: 96.3 MB (96318072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb5f81550f72bf85a0f59a34bcdbdaa081163e6881a6999707602d5a41b87c5`  
		Last Modified: Thu, 30 Mar 2023 20:45:54 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0da497c838cfbd2a13ff978b2d8a70a4aa15242017de99e62f92cecf859ec9e`  
		Last Modified: Thu, 30 Mar 2023 20:45:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c304f3bdd2a53671a36ea7fa7a4adb4aabf531999118481a61abe0be47e5067e`  
		Last Modified: Thu, 30 Mar 2023 20:45:55 GMT  
		Size: 3.1 MB (3146006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a37d8a816541c6472311ed4d07ec5d1b853c836b3fc4acf7f26ba1096812b81`  
		Last Modified: Thu, 30 Mar 2023 20:46:08 GMT  
		Size: 71.0 MB (71044374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10034c55d05a1728e9384bc210ffdce7171b069ee2649b502a185095935ee75d`  
		Last Modified: Thu, 30 Mar 2023 20:45:53 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; s390x

```console
$ docker pull redmine@sha256:605f71cfd75ae08af10dbdac384a764405424ac6b48312a77f6ab73341e9cd05
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.9 MB (198877808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9a53daedeeaf39465336d91e7e481a0e82431e2b7c7b9ba34da71040f1dba7f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Thu, 11 May 2023 22:39:42 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 11 May 2023 22:39:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 11 May 2023 22:39:43 GMT
ENV LANG=C.UTF-8
# Thu, 11 May 2023 22:42:13 GMT
ENV RUBY_MAJOR=3.1
# Thu, 11 May 2023 22:42:13 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 11 May 2023 22:42:13 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 11 May 2023 22:44:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 11 May 2023 22:44:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 11 May 2023 22:44:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 11 May 2023 22:44:13 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 22:44:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 11 May 2023 22:44:13 GMT
CMD ["irb"]
# Wed, 14 Jun 2023 03:12:34 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jun 2023 03:12:49 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 14 Jun 2023 03:12:53 GMT
ENV RAILS_ENV=production
# Wed, 14 Jun 2023 03:12:54 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jun 2023 03:12:54 GMT
ENV HOME=/home/redmine
# Wed, 14 Jun 2023 03:12:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jun 2023 03:12:54 GMT
ENV REDMINE_VERSION=5.0.5
# Wed, 14 Jun 2023 03:12:54 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Wed, 14 Jun 2023 03:12:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Wed, 14 Jun 2023 03:12:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jun 2023 03:12:58 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jun 2023 03:14:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jun 2023 03:14:32 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jun 2023 03:14:32 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Wed, 14 Jun 2023 03:14:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jun 2023 03:14:33 GMT
EXPOSE 3000
# Wed, 14 Jun 2023 03:14:33 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a3d778cffb165fd64c47f19c4f3272ee3f3bed03ad3a09316a6fe63b460402`  
		Last Modified: Thu, 11 May 2023 22:45:19 GMT  
		Size: 4.2 MB (4234696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80b3006327da4ee73698ff4a5a5f7fd17842684d810020d5587f27517457bef`  
		Last Modified: Thu, 11 May 2023 22:45:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d79385ec93ad93b8179ed6e8ebf793e667de3eaf1f93744d7e182cc4956e053`  
		Last Modified: Thu, 11 May 2023 22:45:38 GMT  
		Size: 29.1 MB (29092221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369e9b7fccdbbf5dc9d65853f17af301210cf61cb2dfa25571f4b59f1158f4b9`  
		Last Modified: Thu, 11 May 2023 22:45:36 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2e83590c481c308d4db768f50c0dd45d7009b55c502f58b437f9da00113502`  
		Last Modified: Wed, 14 Jun 2023 03:15:23 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a77bd7dd4d1823c33015e169d56742df5dbef4a39ac59cdc9e75295f63c66e`  
		Last Modified: Wed, 14 Jun 2023 03:15:34 GMT  
		Size: 86.6 MB (86626728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641d9c61a393bbb1d3ded87ee9977f6711a3d5dcc83cdca6125a070de25cc29f`  
		Last Modified: Wed, 14 Jun 2023 03:15:22 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bec82c4632d17f7952be0a0950c01fdd65037d606a1c9c14559b0ce2472ac1`  
		Last Modified: Wed, 14 Jun 2023 03:15:22 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fc3512b8e6e7a98ca1b07405f0fc3f8603cff66c01900c839c78655e2e4cbd`  
		Last Modified: Wed, 14 Jun 2023 03:15:23 GMT  
		Size: 3.1 MB (3145991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe8018e061361019f08db0d1111f61e77be53644abf9872421bb61c67dd5dbe`  
		Last Modified: Wed, 14 Jun 2023 03:15:29 GMT  
		Size: 72.5 MB (72547933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91f9a087ed22113364aea6566c95a723b3aff6a11a7682ceb709c143e18461b`  
		Last Modified: Wed, 14 Jun 2023 03:15:22 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
