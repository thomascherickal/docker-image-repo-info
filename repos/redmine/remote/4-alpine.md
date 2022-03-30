## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:e8b9bdf09ce0deb0298d8b753066c8642f7a8c0143982cee9cd4c46f85401171
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

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:640c03ed07bff8f057aaf5766293e36ebbf54011cb3c615ba4a5f9309973823c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.2 MB (162170702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8454d0eff08018bb8043d0321af239a181a7f79ce0e52729ad0352f297cea82c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:35:33 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 29 Mar 2022 10:35:33 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 10:35:33 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 11:01:12 GMT
ENV RUBY_MAJOR=2.7
# Tue, 29 Mar 2022 11:01:12 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 29 Mar 2022 11:01:12 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 29 Mar 2022 11:03:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 11:03:37 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 11:03:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 11:03:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 11:03:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 11:03:38 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 13:11:30 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 30 Mar 2022 13:11:39 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 30 Mar 2022 13:11:40 GMT
ENV RAILS_ENV=production
# Wed, 30 Mar 2022 13:11:40 GMT
WORKDIR /usr/src/redmine
# Wed, 30 Mar 2022 13:11:40 GMT
ENV HOME=/home/redmine
# Wed, 30 Mar 2022 13:11:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 30 Mar 2022 13:11:41 GMT
ENV REDMINE_VERSION=4.2.5
# Wed, 30 Mar 2022 13:11:41 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Wed, 30 Mar 2022 13:11:41 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Wed, 30 Mar 2022 13:11:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 30 Mar 2022 13:11:44 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 30 Mar 2022 13:13:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 13:13:52 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 30 Mar 2022 13:13:52 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 30 Mar 2022 13:13:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 30 Mar 2022 13:13:52 GMT
EXPOSE 3000
# Wed, 30 Mar 2022 13:13:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b2a498e12b462d1575bb61fd82b4caae729475e170528ca7ee03168e5c06a5`  
		Last Modified: Tue, 29 Mar 2022 11:19:44 GMT  
		Size: 3.7 MB (3683464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b8b47fe2987ab4675b1d9a720c8a7cbb1feb4ffae6ca57063e6447fc661a5c`  
		Last Modified: Tue, 29 Mar 2022 11:19:43 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed9ca28e75aff15c84facdf24940255e77e684417c4c25c3c629b24dfe86f21`  
		Last Modified: Tue, 29 Mar 2022 11:22:06 GMT  
		Size: 14.0 MB (13975193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b79f1b42038a7ac03d884053f96c70cfdaf6c9108dffc3b2f9bf23031fc1b0`  
		Last Modified: Tue, 29 Mar 2022 11:22:04 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1e30216920db06420ec372ac2b50f3fd2de8cbcea675c3b246a09a768b9885`  
		Last Modified: Wed, 30 Mar 2022 13:21:40 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5816582835a6a785065373e25b3f87b3d2860e593acee82df4ae922e69c681b`  
		Last Modified: Wed, 30 Mar 2022 13:21:51 GMT  
		Size: 82.2 MB (82231878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c371fd470e82eb2d103bfdc729f18f1d78e5a6a6ddd43b31d3f9a5cd636f1699`  
		Last Modified: Wed, 30 Mar 2022 13:21:37 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774934ace613cebfff7ce89fe4d92231a5b88ec50a95170dfa890c463aed9bc1`  
		Last Modified: Wed, 30 Mar 2022 13:21:37 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd152b4d54bf53b77b658b03a5d581ff5200ef9e5af212b73fce396ddc7cf43`  
		Last Modified: Wed, 30 Mar 2022 13:21:38 GMT  
		Size: 3.1 MB (3065672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d965c80451d4c7ad910679787236317ea7a7a773b56c3adda3693a22a53d09`  
		Last Modified: Wed, 30 Mar 2022 13:21:42 GMT  
		Size: 56.4 MB (56396242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b0c9fcbc39041cd6d4760191093abb02f3774e1b33b7d53191cab029bc8944`  
		Last Modified: Wed, 30 Mar 2022 13:21:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:034e1fb16eb89c9e6517d415eca4f1a914d1130d165a0ca66311568c82b80dec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.8 MB (155765085 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ffca1c61005f801743c3cd0f599d10f15f823a891b2c71d76776e42fe9430ec`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 12:39:37 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 29 Mar 2022 12:39:39 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 12:39:39 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 12:58:20 GMT
ENV RUBY_MAJOR=2.7
# Tue, 29 Mar 2022 12:58:20 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 29 Mar 2022 12:58:21 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 29 Mar 2022 13:02:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 13:02:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 13:02:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 13:02:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 13:02:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 13:02:09 GMT
CMD ["irb"]
# Tue, 29 Mar 2022 18:56:54 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 29 Mar 2022 18:57:25 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 29 Mar 2022 18:57:26 GMT
ENV RAILS_ENV=production
# Tue, 29 Mar 2022 18:57:27 GMT
WORKDIR /usr/src/redmine
# Tue, 29 Mar 2022 18:57:27 GMT
ENV HOME=/home/redmine
# Tue, 29 Mar 2022 18:57:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 29 Mar 2022 18:57:29 GMT
ENV REDMINE_VERSION=4.2.5
# Tue, 29 Mar 2022 18:57:30 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Tue, 29 Mar 2022 18:57:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Tue, 29 Mar 2022 18:57:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 29 Mar 2022 18:57:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 29 Mar 2022 19:03:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 19:03:50 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 29 Mar 2022 19:03:50 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 29 Mar 2022 19:03:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 29 Mar 2022 19:03:51 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 19:03:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811ade7e739e2c56527c78e00aeeb3537c0c0ffef7a064c294c45e36747f3e01`  
		Last Modified: Tue, 29 Mar 2022 13:17:13 GMT  
		Size: 3.4 MB (3431575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80dc449872e7cfbcaf36411de7f34cc650d461f5cf108ca7308fffac2d627376`  
		Last Modified: Tue, 29 Mar 2022 13:17:10 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859740810b532e83f03ad4b09d1887afb1ebdeea5c74cd1e656ca7de5a801de`  
		Last Modified: Tue, 29 Mar 2022 13:19:32 GMT  
		Size: 13.4 MB (13411663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a85c270d0a5fcf698dabdb4fc0a7581b8b3ab7c2523e65f65aacc201b337880`  
		Last Modified: Tue, 29 Mar 2022 13:19:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:892d63d758e9809c04356eeaa8f0d2468903277f39f6afe209fafaf90f6d95a7`  
		Last Modified: Tue, 29 Mar 2022 19:14:17 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7b1456bd474d635969f33c9b6d56cfb58e41d40255d14964579129f145de003`  
		Last Modified: Tue, 29 Mar 2022 19:15:10 GMT  
		Size: 77.7 MB (77699384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea9ee465fef86cd0136378f660c9b0b43c5f919bc7f018125008977d8f83ed9`  
		Last Modified: Tue, 29 Mar 2022 19:14:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3755caeeac30ae2ad2dfa91c55536aa5289f9dab5b8a56089b588d2a9c748c72`  
		Last Modified: Tue, 29 Mar 2022 19:14:16 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d79db8e09dd8c2172ef333698d1e3efa2441ec1eddc9c6cc11c7982633246d27`  
		Last Modified: Tue, 29 Mar 2022 19:14:20 GMT  
		Size: 3.1 MB (3065700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaf444fff0154752b8ab448409f7cb7f7c2dfd7d7287edfae5b5124d4f5879c`  
		Last Modified: Tue, 29 Mar 2022 19:14:40 GMT  
		Size: 55.5 MB (55531079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938dae1dc112d93edace757fae44a5532914a35518ee445bce7de9e0605c9989`  
		Last Modified: Tue, 29 Mar 2022 19:14:16 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:1419b50412a4315ca6c66325771ef2535215c50e10cf5b9a64f022714a17a39f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.6 MB (151593483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7e15458ca0ec6722c35ed7d1f20ec2e0a812c1e1b40ea9c2fc27032ee10fa1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 02:44:57 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 24 Mar 2022 02:44:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 24 Mar 2022 02:44:59 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 02:55:20 GMT
ENV RUBY_MAJOR=2.7
# Thu, 24 Mar 2022 02:55:21 GMT
ENV RUBY_VERSION=2.7.5
# Thu, 24 Mar 2022 02:55:21 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Thu, 24 Mar 2022 02:58:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 24 Mar 2022 02:58:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 24 Mar 2022 02:58:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 24 Mar 2022 02:58:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 02:58:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 24 Mar 2022 02:58:43 GMT
CMD ["irb"]
# Thu, 24 Mar 2022 08:36:42 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 24 Mar 2022 08:37:10 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 24 Mar 2022 08:37:12 GMT
ENV RAILS_ENV=production
# Thu, 24 Mar 2022 08:37:12 GMT
WORKDIR /usr/src/redmine
# Thu, 24 Mar 2022 08:37:12 GMT
ENV HOME=/home/redmine
# Thu, 24 Mar 2022 08:37:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 29 Mar 2022 01:48:13 GMT
ENV REDMINE_VERSION=4.2.5
# Tue, 29 Mar 2022 01:48:14 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Tue, 29 Mar 2022 01:48:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Tue, 29 Mar 2022 01:48:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 29 Mar 2022 01:48:21 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 29 Mar 2022 01:54:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 01:54:10 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 29 Mar 2022 01:54:11 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 29 Mar 2022 01:54:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 29 Mar 2022 01:54:12 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 01:54:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b270462616d04c8a35ca23e601a7d58556ded2bca12ec3325d65732668faf230`  
		Last Modified: Thu, 24 Mar 2022 03:10:52 GMT  
		Size: 3.3 MB (3301689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26ac7cfef6bde7a810d9169dd8e994444200a8273de973213ead6ad763b2515`  
		Last Modified: Thu, 24 Mar 2022 03:10:49 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ed1e0289ed4353184a2a45684efe87b4cfcb44d8a3fa72ddf365a8405b3844`  
		Last Modified: Thu, 24 Mar 2022 03:13:04 GMT  
		Size: 13.3 MB (13297046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c405679fed60f2981d48a947469a064772a593d633c49198682669eec653a0`  
		Last Modified: Thu, 24 Mar 2022 03:12:57 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9ef84f7df05bcdc7a926a03408feef1f90278bb714e613e0c9846ba989214d`  
		Last Modified: Thu, 24 Mar 2022 08:51:47 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1347161975a1f00f389085b01c0af7aa2a220fe8c70aa0f64cadfbc7836bad5`  
		Last Modified: Thu, 24 Mar 2022 08:52:34 GMT  
		Size: 74.3 MB (74255168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e02200d1b46d51fb12a1f164154d21113fb335ebd1eebcfb1e2762411724d6`  
		Last Modified: Thu, 24 Mar 2022 08:51:45 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbdf9656a129174e7ed2702348795b5d799d65fd3d4370c5ba7cde0d59b79b0`  
		Last Modified: Thu, 24 Mar 2022 08:51:45 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f17eb45ff3c08d735ba44d24151ae869278acf52c3229e1255783ef9ff64f74`  
		Last Modified: Tue, 29 Mar 2022 02:10:35 GMT  
		Size: 3.1 MB (3065668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd09534cee3e2a457bd346f5a82cb91996978e3c1f656c9890b0078908911f65`  
		Last Modified: Tue, 29 Mar 2022 02:10:53 GMT  
		Size: 55.2 MB (55243111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdc93b5720b48fc3d410fbc71fd918da2c96c93de6f82582a52d8ad340d8007`  
		Last Modified: Tue, 29 Mar 2022 02:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:4dbff20c9053bce00b674741bb5a8012fc6e124e86fe022546cf1520f3d17d57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (158957646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9f797946c8d3896771cb6c0c92578e0fec1828db7abae11d66a4f5cc07cee0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:42:10 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 24 Mar 2022 08:42:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 24 Mar 2022 08:42:12 GMT
ENV LANG=C.UTF-8
# Thu, 24 Mar 2022 08:48:05 GMT
ENV RUBY_MAJOR=2.7
# Thu, 24 Mar 2022 08:48:06 GMT
ENV RUBY_VERSION=2.7.5
# Thu, 24 Mar 2022 08:48:07 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Thu, 24 Mar 2022 08:49:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 24 Mar 2022 08:49:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 24 Mar 2022 08:49:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 24 Mar 2022 08:49:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 08:49:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 24 Mar 2022 08:49:58 GMT
CMD ["irb"]
# Thu, 24 Mar 2022 11:58:15 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 24 Mar 2022 11:58:24 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 24 Mar 2022 11:58:25 GMT
ENV RAILS_ENV=production
# Thu, 24 Mar 2022 11:58:26 GMT
WORKDIR /usr/src/redmine
# Thu, 24 Mar 2022 11:58:27 GMT
ENV HOME=/home/redmine
# Thu, 24 Mar 2022 11:58:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 29 Mar 2022 07:36:14 GMT
ENV REDMINE_VERSION=4.2.5
# Tue, 29 Mar 2022 07:36:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Tue, 29 Mar 2022 07:36:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Tue, 29 Mar 2022 07:36:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 29 Mar 2022 07:36:21 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 29 Mar 2022 07:40:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 07:40:54 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 29 Mar 2022 07:40:55 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 29 Mar 2022 07:40:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 29 Mar 2022 07:40:57 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 07:40:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c722564a920253dd5dcde2445f56276e99f12dac9a358b71ac3487d9a1819b64`  
		Last Modified: Thu, 24 Mar 2022 08:55:57 GMT  
		Size: 3.6 MB (3645769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ff54d248faaac88f80e6e593849e246f769cc25beca495f4dc512c2ae68a33`  
		Last Modified: Thu, 24 Mar 2022 08:55:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f8c3ef5ecdd9fb9bb3e064315978e109a80b7405de813e52315d7ccd381392`  
		Last Modified: Thu, 24 Mar 2022 08:57:11 GMT  
		Size: 13.8 MB (13808107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c906c8bfb63d7c64470fb6882678ac07eccd9cedf4018d46b418adecb1dbe1`  
		Last Modified: Thu, 24 Mar 2022 08:57:09 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edfbb1879284183327c570857b6264b4664978ca86890afe17704ebc85dfbed`  
		Last Modified: Thu, 24 Mar 2022 12:05:09 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd08248994a304d7de2af146a7fd10612349a9b312d3c006379b6ac90330037`  
		Last Modified: Thu, 24 Mar 2022 12:05:20 GMT  
		Size: 79.5 MB (79472699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b968afdaac6c3d518d1bc5f4262970ab98ba142eac648b8244fa584a6edee5c`  
		Last Modified: Thu, 24 Mar 2022 12:05:06 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48f21d7d9068a5f1c653afed1534d336db914fdefc821f25250bfc3a767427d`  
		Last Modified: Thu, 24 Mar 2022 12:05:06 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9ba0cfd22e7dd7fe4b72a98f72e1e9608dec09d90f2c778fefe0e7267076dc`  
		Last Modified: Tue, 29 Mar 2022 07:51:54 GMT  
		Size: 3.1 MB (3065802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f55e42f9373a28fc11f39d1aa8958dfbb77ce6c9d7ddfc0f318a05793914c1`  
		Last Modified: Tue, 29 Mar 2022 07:52:00 GMT  
		Size: 56.2 MB (56246935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00790b7bf7d4c5754d84480c137f862167554e5f3aa3933faf46340ad7f33d0e`  
		Last Modified: Tue, 29 Mar 2022 07:51:53 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; 386

```console
$ docker pull redmine@sha256:77d35223437440844fbf7ef9679643a862cc346c47e547505b1e42957c9d4538
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.3 MB (162315518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7477e7af140afb33c607fe194fbb89626acdff00f29210753be9cc4f95b409a6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:32 GMT
ADD file:8d3b249cd4cd9b2fb1888f3efcc06d39c2f56b4c25257ecee645c1be0146f7fd in / 
# Tue, 29 Mar 2022 00:38:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:02:50 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 29 Mar 2022 10:02:51 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 10:02:52 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 10:22:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 29 Mar 2022 10:22:02 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 29 Mar 2022 10:22:03 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 29 Mar 2022 10:23:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 10:23:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 10:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 10:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:23:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 10:23:47 GMT
CMD ["irb"]
# Tue, 29 Mar 2022 22:17:55 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 29 Mar 2022 22:18:03 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 29 Mar 2022 22:18:04 GMT
ENV RAILS_ENV=production
# Tue, 29 Mar 2022 22:18:05 GMT
WORKDIR /usr/src/redmine
# Tue, 29 Mar 2022 22:18:06 GMT
ENV HOME=/home/redmine
# Tue, 29 Mar 2022 22:18:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 29 Mar 2022 22:18:08 GMT
ENV REDMINE_VERSION=4.2.5
# Tue, 29 Mar 2022 22:18:09 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Tue, 29 Mar 2022 22:18:10 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Tue, 29 Mar 2022 22:18:14 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 29 Mar 2022 22:18:15 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 29 Mar 2022 22:20:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 22:20:27 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 29 Mar 2022 22:20:28 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 29 Mar 2022 22:20:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 29 Mar 2022 22:20:29 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 22:20:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:134f45dc6b904419acf27b9807970f271117691bc67b963b86de8965db932175`  
		Last Modified: Tue, 29 Mar 2022 00:39:35 GMT  
		Size: 2.8 MB (2818926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5ee325d25260baf59ce0152181de16fe57bed53bdfc6756992bdfd9d0fb8d1`  
		Last Modified: Tue, 29 Mar 2022 10:39:01 GMT  
		Size: 3.7 MB (3709243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa0ad064c62fec592cb35805134b8bb4da79fe7356d8b445ccb44e91f312b20e`  
		Last Modified: Tue, 29 Mar 2022 10:39:00 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0025b42df9e8dfd4e723d1c1a37f093e3f25872e27594d88f6da8560507bf60`  
		Last Modified: Tue, 29 Mar 2022 10:42:00 GMT  
		Size: 13.3 MB (13282913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56ff6b338651ac3b3f670839a4080be70ae38d988bea886b122dc8607d639ed`  
		Last Modified: Tue, 29 Mar 2022 10:41:58 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d9ea00bb427c346cc78a50f0275fd705492082862ff5a8b548cc0edea7569a`  
		Last Modified: Tue, 29 Mar 2022 22:28:47 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d800bd7293da4fc0127f1383e8afcb814671edc3b827d05f8a1153bc966f1191`  
		Last Modified: Tue, 29 Mar 2022 22:29:03 GMT  
		Size: 83.8 MB (83839520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c9d08e916e639ca2588284d503b4f65f962adce5df8df5044604e4e05989fe`  
		Last Modified: Tue, 29 Mar 2022 22:28:45 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be35b06fa362cf3dfb28960c3282dd17db77703bd02b082b8f6354c7929c1b2`  
		Last Modified: Tue, 29 Mar 2022 22:28:44 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a197654c683c3e691ec8df08c3d0154e9e82950f1757c7fdaae8c656e9459475`  
		Last Modified: Tue, 29 Mar 2022 22:28:45 GMT  
		Size: 3.1 MB (3065804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534d1488f288ea22390f6c2ce215bdf5a138fcb71fb0f4fc55ab21d38d350da7`  
		Last Modified: Tue, 29 Mar 2022 22:28:59 GMT  
		Size: 55.6 MB (55595498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40845cbffc66a91de051222b0f134911afbf1c5f0d067808d81057bfd8442a1f`  
		Last Modified: Tue, 29 Mar 2022 22:28:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; ppc64le

```console
$ docker pull redmine@sha256:4970a345ae920dff022cb462faadef68a7a01391f973054e7755f61dd1b65b98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.8 MB (163760642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0af5ec8d67f0fdbc9c097c9c761bf0a32480091313ae5d48c99513a80e06dc3d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 23:41:41 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 23 Mar 2022 23:42:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Mar 2022 23:42:12 GMT
ENV LANG=C.UTF-8
# Wed, 23 Mar 2022 23:52:27 GMT
ENV RUBY_MAJOR=2.7
# Wed, 23 Mar 2022 23:52:31 GMT
ENV RUBY_VERSION=2.7.5
# Wed, 23 Mar 2022 23:52:33 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Wed, 23 Mar 2022 23:55:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 23 Mar 2022 23:55:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 23 Mar 2022 23:55:17 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 23 Mar 2022 23:55:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 23:55:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 23 Mar 2022 23:55:30 GMT
CMD ["irb"]
# Thu, 24 Mar 2022 09:21:49 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 24 Mar 2022 09:22:40 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 24 Mar 2022 09:22:48 GMT
ENV RAILS_ENV=production
# Thu, 24 Mar 2022 09:22:50 GMT
WORKDIR /usr/src/redmine
# Thu, 24 Mar 2022 09:22:53 GMT
ENV HOME=/home/redmine
# Thu, 24 Mar 2022 09:22:58 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 29 Mar 2022 06:41:10 GMT
ENV REDMINE_VERSION=4.2.5
# Tue, 29 Mar 2022 06:41:16 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Tue, 29 Mar 2022 06:41:20 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Tue, 29 Mar 2022 06:41:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 29 Mar 2022 06:41:36 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 29 Mar 2022 06:45:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 06:45:56 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 29 Mar 2022 06:45:58 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 29 Mar 2022 06:46:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 29 Mar 2022 06:46:05 GMT
EXPOSE 3000
# Tue, 29 Mar 2022 06:46:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23512440f7311d52121132163abd549725d0c38cffe5656ecb4555ae67412de9`  
		Last Modified: Thu, 24 Mar 2022 00:03:06 GMT  
		Size: 3.8 MB (3799994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42eaf40bd085e415b9fb073d24361f33572e069a66fa665630bd71ffddcfecd`  
		Last Modified: Thu, 24 Mar 2022 00:03:05 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68412ea87372b92f00ac7efc0e721ec9c2f101d0d7d17dd9646e1c2250ab4ca8`  
		Last Modified: Thu, 24 Mar 2022 00:04:37 GMT  
		Size: 14.4 MB (14416966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72d5dc4f6f7996e749ef78810ad04d450b5bcd972178bbe28986ca72af66489`  
		Last Modified: Thu, 24 Mar 2022 00:04:35 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8799380759d38654288db024867972dd8822249ec8a0aa22d05ccd8e2fb43138`  
		Last Modified: Thu, 24 Mar 2022 09:36:38 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4a3e46c62a6f9183fe01cdfd38c023490db1a3a0db06c90792e71f26688346`  
		Last Modified: Thu, 24 Mar 2022 09:36:53 GMT  
		Size: 82.5 MB (82475487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60a826f645a8da07e337534f4d93a37b8330eeab87d4dce24bce447e33c5bcd`  
		Last Modified: Thu, 24 Mar 2022 09:36:35 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ad2442228e8e05f93d1e5f8c5b1a325d003a34a5376d85113dbe8685f76ac4`  
		Last Modified: Thu, 24 Mar 2022 09:36:35 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20c9f887b134d434a5169544072fb9c600826b1011ed60797faf56b3cc70c529`  
		Last Modified: Tue, 29 Mar 2022 07:00:45 GMT  
		Size: 3.1 MB (3065677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d99f5dcb2853a5f3320d40472e8278b43d34d0acfd2e1659011f16227fbedc1`  
		Last Modified: Tue, 29 Mar 2022 07:00:52 GMT  
		Size: 57.2 MB (57184734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ee3338487b305079bca1084eb6ca0ea0066515ea6baec5f033a17f484d5abf9`  
		Last Modified: Tue, 29 Mar 2022 07:00:44 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; s390x

```console
$ docker pull redmine@sha256:43287d5d559b9d2fa53e6c13aac35b4309aedb4395cfa4784b0546a2bb0b28d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154504895 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5229991ae316dd30a5d7a48b226d7df3297b86809e81b35f38362226fff76dc5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 23:35:57 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 29 Mar 2022 23:35:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 23:35:58 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 23:53:53 GMT
ENV RUBY_MAJOR=2.7
# Tue, 29 Mar 2022 23:53:53 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 29 Mar 2022 23:53:54 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 29 Mar 2022 23:55:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 23:55:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 23:55:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 23:55:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 23:55:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 23:55:25 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 10:57:24 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 30 Mar 2022 10:57:32 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 30 Mar 2022 10:57:35 GMT
ENV RAILS_ENV=production
# Wed, 30 Mar 2022 10:57:36 GMT
WORKDIR /usr/src/redmine
# Wed, 30 Mar 2022 10:57:36 GMT
ENV HOME=/home/redmine
# Wed, 30 Mar 2022 10:57:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 30 Mar 2022 10:57:36 GMT
ENV REDMINE_VERSION=4.2.5
# Wed, 30 Mar 2022 10:57:36 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Wed, 30 Mar 2022 10:57:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Wed, 30 Mar 2022 10:57:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 30 Mar 2022 10:57:40 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 30 Mar 2022 10:59:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 10:59:28 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 30 Mar 2022 10:59:28 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 30 Mar 2022 10:59:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 30 Mar 2022 10:59:29 GMT
EXPOSE 3000
# Wed, 30 Mar 2022 10:59:29 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfff912c3329c0438dbd0a7d1dd8ac907f25e2f6d63b46d6eb453bf57aed155c`  
		Last Modified: Wed, 30 Mar 2022 00:15:43 GMT  
		Size: 3.7 MB (3746170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed8783ae888173a17001ed61cb1111e1517a033f70b07f66092c6f83cddc744`  
		Last Modified: Wed, 30 Mar 2022 00:15:43 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027252628845ca776def170de9d854e1cf8115f3523a1491cff588c00691f13c`  
		Last Modified: Wed, 30 Mar 2022 00:33:13 GMT  
		Size: 14.1 MB (14128425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0ab64ecf78465a27f7c54ca2a3e9fb36b337297166f65782b2b273d4332719`  
		Last Modified: Wed, 30 Mar 2022 00:33:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b2371259d5bc36caf0a4eb508069a73c17b4c8d2ffee191518262aea1f7478b`  
		Last Modified: Wed, 30 Mar 2022 11:06:15 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03490276ca1eb15ea9ae1707b19a88b41b2f4c181e16a4ca5fad7cc9eb00548a`  
		Last Modified: Wed, 30 Mar 2022 11:06:24 GMT  
		Size: 74.3 MB (74319542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7761922db92510348a28e76d223b1b7eabde02064b256cd2c853315336e045a3`  
		Last Modified: Wed, 30 Mar 2022 11:06:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97108b241827a4d5240ae483bbeb84629e556cf022e2d168b7ab7729f9f7ded`  
		Last Modified: Wed, 30 Mar 2022 11:06:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c071af7596933e17cf3fcd245e392c51db91aafbd21fc41ae9bf0078760d2b5b`  
		Last Modified: Wed, 30 Mar 2022 11:06:14 GMT  
		Size: 3.1 MB (3065660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0ce5bd623e1497ff299e77fcb0e6245fa8b439c48e763faa27a7dcdb3dff23`  
		Last Modified: Wed, 30 Mar 2022 11:06:18 GMT  
		Size: 56.6 MB (56640916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55dfe1bfb4dada23b858c501f84d36b1e432c8c84e990442d2682072860cc7e5`  
		Last Modified: Wed, 30 Mar 2022 11:06:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
