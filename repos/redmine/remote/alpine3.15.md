## `redmine:alpine3.15`

```console
$ docker pull redmine@sha256:004b6a9d31585a21aed1e4cf9cd690e77e950a753b1acccd9faf2ac593bd116b
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
$ docker pull redmine@sha256:cb9e4d4adcec527e61c673140a5742466e77d75ada67ecdb169e2ce143f4bae3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.0 MB (163045967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3feae224004be03257df842266e9224a495e1f444ebf12efd9a14d7ea49aa836`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 09:19:26 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 09:19:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 09:19:27 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 09:28:50 GMT
ENV RUBY_MAJOR=2.7
# Tue, 30 Nov 2021 09:28:50 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 30 Nov 2021 09:28:50 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 30 Nov 2021 09:31:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 09:31:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 09:31:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 09:31:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 09:31:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 09:31:51 GMT
CMD ["irb"]
# Tue, 07 Dec 2021 23:30:49 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 06 Jan 2022 20:44:39 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 06 Jan 2022 20:44:40 GMT
ENV RAILS_ENV=production
# Thu, 06 Jan 2022 20:44:40 GMT
WORKDIR /usr/src/redmine
# Thu, 06 Jan 2022 20:44:41 GMT
ENV HOME=/home/redmine
# Thu, 06 Jan 2022 20:44:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 23 Feb 2022 16:21:15 GMT
ENV REDMINE_VERSION=4.2.4
# Tue, 08 Mar 2022 20:17:18 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Tue, 08 Mar 2022 20:17:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Tue, 08 Mar 2022 20:17:22 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 08 Mar 2022 20:17:22 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 08 Mar 2022 20:19:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 08 Mar 2022 20:19:33 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 08 Mar 2022 20:19:33 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 08 Mar 2022 20:19:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:19:34 GMT
EXPOSE 3000
# Tue, 08 Mar 2022 20:19:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecfdfc99c764bed7ef3f6377b64d99601e47cc4087154ed69e70fa5b8cc8fa92`  
		Last Modified: Tue, 30 Nov 2021 09:37:08 GMT  
		Size: 3.7 MB (3692788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfcec1f1cb7c30b5406814a3edc744a6a23fb0c8c6f304e2a2ca9521daa1da01`  
		Last Modified: Tue, 30 Nov 2021 09:37:08 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6325120d0421d107f6fb86c548859a7963b47119cdea48562eb52ae92d2db394`  
		Last Modified: Tue, 30 Nov 2021 09:38:12 GMT  
		Size: 14.0 MB (13975304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fc6ecdde23b73f357ff270cf30bccccc963199d238c8d64d860419d8d84573`  
		Last Modified: Tue, 30 Nov 2021 09:38:10 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab0ed0407dc35440aa3d19cfdacd5e7c83b212e7ff173d69d6628f1c7668f4d`  
		Last Modified: Tue, 07 Dec 2021 23:45:12 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5447d4c8eab6ae190d4bd60631033f1ceb286650680b76b239e3493c2e43d0`  
		Last Modified: Thu, 06 Jan 2022 20:53:15 GMT  
		Size: 82.2 MB (82230412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70dce1d251ad89dcca0ab1ea324bd714a962470679ede0b5450ad53279660fe`  
		Last Modified: Thu, 06 Jan 2022 20:53:00 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1827e4c73b72c56398e15d114cbdb40d28c47282f4bace7e39912a162b90ccc3`  
		Last Modified: Thu, 06 Jan 2022 20:53:00 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c9ca8f4d3f30e2d056abf91e2f987340b7eb4e99afa1b668ddb3db0b23e0de`  
		Last Modified: Tue, 08 Mar 2022 20:24:49 GMT  
		Size: 3.1 MB (3065433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f9a34bffcdeabc6c1dee2ec941c11615ba8398bf2453c3feb28e2445fb651f`  
		Last Modified: Tue, 08 Mar 2022 20:24:55 GMT  
		Size: 57.3 MB (57259881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7216dcc8a8869c1384248e78f789e4fbbcb4c2afb1a14b376cd31ca644ad956`  
		Last Modified: Tue, 08 Mar 2022 20:24:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; arm variant v6

```console
$ docker pull redmine@sha256:dd043a493e91358b319b3ce1d5b3f4e3eb0e97ea361aff5e1da7711c4617df7c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.2 MB (155159568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:400fccc51651b390a2beca7dbb029ecadc20c380e45ee9e4379fa0e4e19a191b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 10:30:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 17 Mar 2022 10:30:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 10:30:19 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 10:39:50 GMT
ENV RUBY_MAJOR=2.7
# Thu, 17 Mar 2022 10:39:50 GMT
ENV RUBY_VERSION=2.7.5
# Thu, 17 Mar 2022 10:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Thu, 17 Mar 2022 10:43:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 10:43:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 10:43:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 10:43:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 10:43:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 10:43:36 GMT
CMD ["irb"]
# Thu, 17 Mar 2022 14:05:02 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 17 Mar 2022 14:05:34 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 17 Mar 2022 14:05:35 GMT
ENV RAILS_ENV=production
# Thu, 17 Mar 2022 14:05:36 GMT
WORKDIR /usr/src/redmine
# Thu, 17 Mar 2022 14:05:36 GMT
ENV HOME=/home/redmine
# Thu, 17 Mar 2022 14:05:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 17 Mar 2022 14:05:39 GMT
ENV REDMINE_VERSION=4.2.4
# Thu, 17 Mar 2022 14:05:39 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Thu, 17 Mar 2022 14:05:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Thu, 17 Mar 2022 14:05:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 17 Mar 2022 14:05:47 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 17 Mar 2022 14:11:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 17 Mar 2022 14:11:54 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 17 Mar 2022 14:11:55 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Thu, 17 Mar 2022 14:11:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 17 Mar 2022 14:11:56 GMT
EXPOSE 3000
# Thu, 17 Mar 2022 14:11:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d86fb78a99c7d753906b56698b6744862b220df1afa71da7d3136884e3eb5c`  
		Last Modified: Thu, 17 Mar 2022 10:50:41 GMT  
		Size: 3.4 MB (3431374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e167efa5b19ea8438bf77dea2c30de42fd74979c87afffbc36fa4edd5a93d22f`  
		Last Modified: Thu, 17 Mar 2022 10:50:39 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c04fa4fd83c3a9f870a023715b8ccb8536f1ac770f78725ed2d0cff21044a3b`  
		Last Modified: Thu, 17 Mar 2022 10:52:08 GMT  
		Size: 13.4 MB (13411675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ef5862dcc0eee867a99ab647ab37f443232c4f3eccf126e42ebdfae05b9773`  
		Last Modified: Thu, 17 Mar 2022 10:52:00 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dbd2ec139009d44a43553bcca78588be3171e5ea72148eada2a6853d36aa44`  
		Last Modified: Thu, 17 Mar 2022 14:20:05 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc5c7f502f4b33ac3ab9ab874712d011aa7443ce1e0e08f425016b98d0c3dcd1`  
		Last Modified: Thu, 17 Mar 2022 14:20:57 GMT  
		Size: 77.7 MB (77697029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7992a6c48be5293a1e6f03e42652230e5fd7bae74f24100e2e4ebe3343b72b81`  
		Last Modified: Thu, 17 Mar 2022 14:20:03 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f28fe74484fff9b17d0ecf89b5bca4724da05c5a98f26426be3e2ddd854c5d`  
		Last Modified: Thu, 17 Mar 2022 14:20:03 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed535d45b1be1af4fa47729755b211a8fe7bf42b6f26244ee7c83ff9c923862`  
		Last Modified: Thu, 17 Mar 2022 14:20:07 GMT  
		Size: 3.1 MB (3065468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505cdce6a91dec93a572074689b8ef510c2b77c4c16229520f9f4032ce6553c9`  
		Last Modified: Thu, 17 Mar 2022 14:20:27 GMT  
		Size: 54.9 MB (54925311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4e8323b249942696f614a7d8e91d898e1357f7c1ab016014cfda4b807aecbc`  
		Last Modified: Thu, 17 Mar 2022 14:20:03 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; arm variant v7

```console
$ docker pull redmine@sha256:f0d07bc113c64705a3d4a78503ec02083bcf63772a62b1b42fb165e2ef1828ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.2 MB (152168292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc1fc6b3a44bb8ba56bb62cb1659fcb7db58e1efa0b7ad3bb4aaf8406fdf1323`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 12:24:51 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 12:24:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 12:24:53 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 12:35:27 GMT
ENV RUBY_MAJOR=2.7
# Tue, 30 Nov 2021 12:35:28 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 30 Nov 2021 12:35:28 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 30 Nov 2021 12:38:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 12:38:47 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 12:38:47 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 12:38:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 12:38:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 12:38:49 GMT
CMD ["irb"]
# Wed, 08 Dec 2021 01:03:12 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 06 Jan 2022 21:12:33 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 06 Jan 2022 21:12:34 GMT
ENV RAILS_ENV=production
# Thu, 06 Jan 2022 21:12:34 GMT
WORKDIR /usr/src/redmine
# Thu, 06 Jan 2022 21:12:35 GMT
ENV HOME=/home/redmine
# Thu, 06 Jan 2022 21:12:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 23 Feb 2022 16:03:40 GMT
ENV REDMINE_VERSION=4.2.4
# Wed, 09 Mar 2022 00:18:54 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Wed, 09 Mar 2022 00:18:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Wed, 09 Mar 2022 00:19:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 09 Mar 2022 00:19:01 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 09 Mar 2022 00:24:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 09 Mar 2022 00:24:35 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 09 Mar 2022 00:24:35 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 09 Mar 2022 00:24:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 09 Mar 2022 00:24:36 GMT
EXPOSE 3000
# Wed, 09 Mar 2022 00:24:36 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0766915476b7e451e3cc952a46b395425b4c07e87c93c4ea5ce0be7800597263`  
		Last Modified: Tue, 30 Nov 2021 12:51:06 GMT  
		Size: 3.3 MB (3310784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821053590f6e9202e506ce7902441cd142388940813112a3702cf16fb3648711`  
		Last Modified: Tue, 30 Nov 2021 12:51:04 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ce54135e330bb78a1f350a77aab008afa36228e53a141841e703c419e24af7`  
		Last Modified: Tue, 30 Nov 2021 12:53:41 GMT  
		Size: 13.3 MB (13296845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea4dd5eaa461aa8802a5c655f3935818309d263dced3c6b8d9917317bccf349`  
		Last Modified: Tue, 30 Nov 2021 12:53:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdea34265ea815072e08ef89644a85749f87001563eab25e70e2540f1828f70b`  
		Last Modified: Wed, 08 Dec 2021 01:39:16 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742c3e488cf7b80a0883c4c5bbf78f4f6abecd2cc3721136a35fda7c93409d27`  
		Last Modified: Thu, 06 Jan 2022 21:33:51 GMT  
		Size: 74.3 MB (74254995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bab9df1af1ae90f9c7256610422f80a7266e0235afea52e23fe828ee39e29b4f`  
		Last Modified: Thu, 06 Jan 2022 21:33:03 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b72c23c9e85e5aadbf7c864684b509cd401645eda8adb603c1a473ae904cd2b`  
		Last Modified: Thu, 06 Jan 2022 21:33:03 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e214d88a5a4b515f1d77cb5811cab8ab544b904753dfd3b605fbd62a006c21`  
		Last Modified: Wed, 09 Mar 2022 00:39:18 GMT  
		Size: 3.1 MB (3065423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f67f0f0db90effcae70b67bc460aecd00db021a773173c57a6ceebd2d1c5cb`  
		Last Modified: Wed, 09 Mar 2022 00:39:39 GMT  
		Size: 55.8 MB (55801746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15008a44486b19b7bd14eb3607732893fe82edca5591dc9a0729cb676d3a1c5`  
		Last Modified: Wed, 09 Mar 2022 00:39:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:17aee655f9cea2f7ca995459b7784252587b29d835782de59e2befddcd110758
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159714436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c9f6624c3c55550cc01fc0366b0010a896302352a69d991f870dd23e8901b0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:36:33 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 05:36:34 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 05:36:35 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 05:42:50 GMT
ENV RUBY_MAJOR=2.7
# Tue, 30 Nov 2021 05:42:50 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 30 Nov 2021 05:42:51 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 30 Nov 2021 05:44:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 05:44:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 05:44:47 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 05:44:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 05:44:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 05:44:50 GMT
CMD ["irb"]
# Wed, 08 Dec 2021 00:15:04 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 06 Jan 2022 20:27:39 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 06 Jan 2022 20:27:39 GMT
ENV RAILS_ENV=production
# Thu, 06 Jan 2022 20:27:40 GMT
WORKDIR /usr/src/redmine
# Thu, 06 Jan 2022 20:27:41 GMT
ENV HOME=/home/redmine
# Thu, 06 Jan 2022 20:27:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 23 Feb 2022 16:52:44 GMT
ENV REDMINE_VERSION=4.2.4
# Tue, 08 Mar 2022 20:43:50 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Tue, 08 Mar 2022 20:43:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Tue, 08 Mar 2022 20:43:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 08 Mar 2022 20:43:55 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 08 Mar 2022 20:46:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 08 Mar 2022 20:46:23 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 08 Mar 2022 20:46:24 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 08 Mar 2022 20:46:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:46:25 GMT
EXPOSE 3000
# Tue, 08 Mar 2022 20:46:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e12e2c567460b1b6fc7c47caaf0096b83279da72da30d631a78973212f186a`  
		Last Modified: Tue, 30 Nov 2021 05:50:38 GMT  
		Size: 3.7 MB (3657031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd57995982ca19298b043d92ab79f0d14ea093fda2b52a2b4a4a00ea9af2b13`  
		Last Modified: Tue, 30 Nov 2021 05:50:37 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1ddc8f8e3e44b77eb4395c57cbca58e7d8c869e875418b82c7b4e6543c88f3`  
		Last Modified: Tue, 30 Nov 2021 05:52:04 GMT  
		Size: 13.8 MB (13808332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2a0f605291ca229f9999a6bf98a1218f519fa2c885036f9bb7e3192a85d6ec`  
		Last Modified: Tue, 30 Nov 2021 05:52:02 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d722ad9ecc5d37bb372582100bc6603d6ec29df6fc7313190705b362437488c`  
		Last Modified: Wed, 08 Dec 2021 00:30:53 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c08597b70299ce32718d17657f079472af1ffc0f1fec1437e0c94f8d62b290`  
		Last Modified: Thu, 06 Jan 2022 20:37:06 GMT  
		Size: 79.5 MB (79472010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe417c2ee6ebbb2b81b86574a7262bb0431df4bbc65db07bad35c5e0df7cd76`  
		Last Modified: Thu, 06 Jan 2022 20:36:52 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8a3dce255057cb8b35009201eb612c5b8292de880e008faac2892cecd71649`  
		Last Modified: Thu, 06 Jan 2022 20:36:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1b69b8e0a9de750eddfadc114fa0c8d44055ff96beccecdb71f33ccdf43746`  
		Last Modified: Tue, 08 Mar 2022 20:53:00 GMT  
		Size: 3.1 MB (3065416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b333eb0e5ee17dee9ab2e57020f4040f460252585db449e1e0c505a6fa55ae27`  
		Last Modified: Tue, 08 Mar 2022 20:53:05 GMT  
		Size: 57.0 MB (56992599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbb51ca3d8b78b3647e5a6516ed6e42e868a3d5a3baf19a9a5bf67fb7c469d2`  
		Last Modified: Tue, 08 Mar 2022 20:52:59 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; 386

```console
$ docker pull redmine@sha256:0c3f2752967a49f2c345fdf7d396b7454691eb99e10c34c4f7e56cf4fc2fb5ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.2 MB (163205698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21cccd2460ab897112f4e30daa32e6ed645eacaf8f427fdfb517859218b5451e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 08:37:44 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 08:37:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 08:37:47 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 08:53:32 GMT
ENV RUBY_MAJOR=2.7
# Tue, 30 Nov 2021 08:53:33 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 30 Nov 2021 08:53:33 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 30 Nov 2021 08:57:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 08:57:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 08:57:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 08:57:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 08:57:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 08:57:03 GMT
CMD ["irb"]
# Tue, 07 Dec 2021 23:58:43 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 06 Jan 2022 20:14:50 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 06 Jan 2022 20:14:51 GMT
ENV RAILS_ENV=production
# Thu, 06 Jan 2022 20:14:51 GMT
WORKDIR /usr/src/redmine
# Thu, 06 Jan 2022 20:14:52 GMT
ENV HOME=/home/redmine
# Thu, 06 Jan 2022 20:14:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 23 Feb 2022 16:39:55 GMT
ENV REDMINE_VERSION=4.2.4
# Tue, 08 Mar 2022 21:25:32 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Tue, 08 Mar 2022 21:25:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Tue, 08 Mar 2022 21:25:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 08 Mar 2022 21:25:36 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 08 Mar 2022 21:28:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 08 Mar 2022 21:28:03 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 08 Mar 2022 21:28:03 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 08 Mar 2022 21:28:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Mar 2022 21:28:03 GMT
EXPOSE 3000
# Tue, 08 Mar 2022 21:28:03 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae05e47cf02db9a8baff44ce7728fa8e3e4c903d33d017437f9c402d4c448299`  
		Last Modified: Tue, 30 Nov 2021 09:04:59 GMT  
		Size: 3.7 MB (3716923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6021ca2d58b5286b59b232c69e4e1f40cd538b8d4ca8893f2be4420c1198845`  
		Last Modified: Tue, 30 Nov 2021 09:04:57 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172bf44434451a99981eace9b416143d4489ee25252ae1ffb72e0321c919e294`  
		Last Modified: Tue, 30 Nov 2021 09:06:34 GMT  
		Size: 13.3 MB (13287700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56081ff84c4aaca1d51b908dc1a2a4a576a18b7be2b00668ecfc586617a0eb1b`  
		Last Modified: Tue, 30 Nov 2021 09:06:31 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c2a3cd281367f6fdcd47c377278d24ec835d21c07f66f62ea0b44a71dc6db7`  
		Last Modified: Wed, 08 Dec 2021 00:14:05 GMT  
		Size: 1.2 KB (1224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389e7869d425eebeb8b7b0a0b94460623fdbbdbe408e09d9a5d7fd40b9e02a1c`  
		Last Modified: Thu, 06 Jan 2022 20:25:29 GMT  
		Size: 83.8 MB (83832124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1286aa3a555b20230f5003553bffcd5187fd6b3744cf70edcbea2e85fac9816`  
		Last Modified: Thu, 06 Jan 2022 20:25:05 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607b215b548f17cbcb7550d6af27cb36345903c816dfba4f49b0187683a644a8`  
		Last Modified: Thu, 06 Jan 2022 20:25:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c3f0523f1ae3391d5b06daee9f5df2e8abeb9bd5d299c1dc26a46e515699e4`  
		Last Modified: Tue, 08 Mar 2022 21:33:25 GMT  
		Size: 3.1 MB (3065424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b4ccee6af3ee6ac117420d6117bf0f58ad88fc2a5362e271f50df71b3a3ae8`  
		Last Modified: Tue, 08 Mar 2022 21:33:30 GMT  
		Size: 56.5 MB (56472664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c231addab268c6a5c09fdd599bf84acf38cebbfc75f0450a59c4191d9a2c11a8`  
		Last Modified: Tue, 08 Mar 2022 21:33:23 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; ppc64le

```console
$ docker pull redmine@sha256:0ac85cd36ab64a2397d5665abd7dfe24d36402c142eccc9098201a5a1b7047d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.6 MB (164556285 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b73110022638dc57815af5393a77843db0c9c36bf149dbc06a7c0f796704363`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 07:45:57 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 07:46:04 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 07:46:07 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 07:54:22 GMT
ENV RUBY_MAJOR=2.7
# Tue, 30 Nov 2021 07:54:24 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 30 Nov 2021 07:54:27 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 30 Nov 2021 07:57:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 07:57:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 07:57:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 07:57:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 07:57:14 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 07:57:16 GMT
CMD ["irb"]
# Wed, 08 Dec 2021 00:41:19 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 06 Jan 2022 21:14:14 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 06 Jan 2022 21:14:20 GMT
ENV RAILS_ENV=production
# Thu, 06 Jan 2022 21:14:22 GMT
WORKDIR /usr/src/redmine
# Thu, 06 Jan 2022 21:14:26 GMT
ENV HOME=/home/redmine
# Thu, 06 Jan 2022 21:14:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 23 Feb 2022 16:23:26 GMT
ENV REDMINE_VERSION=4.2.4
# Tue, 08 Mar 2022 21:20:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Tue, 08 Mar 2022 21:20:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Tue, 08 Mar 2022 21:20:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 08 Mar 2022 21:20:51 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 08 Mar 2022 21:24:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 08 Mar 2022 21:24:53 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 08 Mar 2022 21:24:56 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 08 Mar 2022 21:24:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Mar 2022 21:25:03 GMT
EXPOSE 3000
# Tue, 08 Mar 2022 21:25:08 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60dfb224d10621897aed06dde46dd5c4c649f159947d6425fc8d43cd1b6437fb`  
		Last Modified: Tue, 30 Nov 2021 08:04:09 GMT  
		Size: 3.8 MB (3810519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a630f14514f37223fa8f0cbd3071c6b038a767df40188168543d2e3d3947ed72`  
		Last Modified: Tue, 30 Nov 2021 08:04:08 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b970574f0a715e05ee81a09fd129ad18794870ea66889f382aa4a6feb44f83`  
		Last Modified: Tue, 30 Nov 2021 08:05:42 GMT  
		Size: 14.4 MB (14416997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebc374dac618510536d9253f21cd980b26db206b99a10521fb7bdf4dbf47de9`  
		Last Modified: Tue, 30 Nov 2021 08:05:39 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4e3e936e2d05a89430ee1b4d3bca046eb2db8f688e479ea61e1ae398ce7eae`  
		Last Modified: Wed, 08 Dec 2021 01:25:09 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918ada81049de73d4c945c196156edc72078aa36b2ddbadd9296b957f7ea81fd`  
		Last Modified: Thu, 06 Jan 2022 21:30:33 GMT  
		Size: 82.5 MB (82474364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a5dd852761daa43f9b94053beb1f921e774b94a0710040cad6f0ead8344434`  
		Last Modified: Thu, 06 Jan 2022 21:30:15 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cda37ba3737b6e1e4193342f581110720c7820ba3f972fe0791b15980686c41`  
		Last Modified: Thu, 06 Jan 2022 21:30:15 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce81fdf03ae25dd1741cd607895a8af75b020fbae40f8ef0278476557b898e6`  
		Last Modified: Tue, 08 Mar 2022 21:37:08 GMT  
		Size: 3.1 MB (3065438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4421eacccd42409e27629f10316761317b77fb1e851e690bc801c4fb85a5db2`  
		Last Modified: Tue, 08 Mar 2022 21:37:15 GMT  
		Size: 58.0 MB (57970443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00bfc6a46d67216e816f4c56ad1fee0c86dbd1c733245233e18046202322824c`  
		Last Modified: Tue, 08 Mar 2022 21:37:07 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.15` - linux; s390x

```console
$ docker pull redmine@sha256:94fbbeaa1cf77711a8e47b192e8219cea936c36727549b8a3e669d75dbb078d8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155116044 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c262c5a359b622c37ac9ded24eb5107f0d848cedc862205ccefe05b62243fa25`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 09:51:07 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 09:51:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 09:51:08 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 09:57:14 GMT
ENV RUBY_MAJOR=2.7
# Tue, 30 Nov 2021 09:57:14 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 30 Nov 2021 09:57:14 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 30 Nov 2021 09:58:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 09:58:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 09:58:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 09:58:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 09:58:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 09:58:51 GMT
CMD ["irb"]
# Wed, 08 Dec 2021 00:03:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 06 Jan 2022 20:13:09 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 06 Jan 2022 20:13:13 GMT
ENV RAILS_ENV=production
# Thu, 06 Jan 2022 20:13:13 GMT
WORKDIR /usr/src/redmine
# Thu, 06 Jan 2022 20:13:13 GMT
ENV HOME=/home/redmine
# Thu, 06 Jan 2022 20:13:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 23 Feb 2022 16:43:37 GMT
ENV REDMINE_VERSION=4.2.4
# Tue, 08 Mar 2022 20:52:14 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Tue, 08 Mar 2022 20:52:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Tue, 08 Mar 2022 20:52:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 08 Mar 2022 20:52:17 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 08 Mar 2022 20:54:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 08 Mar 2022 20:54:03 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 08 Mar 2022 20:54:03 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 08 Mar 2022 20:54:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 08 Mar 2022 20:54:03 GMT
EXPOSE 3000
# Tue, 08 Mar 2022 20:54:03 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7faf48375ad71a3a34aeb82123f04c9dfdba63e9e43a8131a57fb8581ef31e0`  
		Last Modified: Tue, 30 Nov 2021 10:04:36 GMT  
		Size: 3.8 MB (3754915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b691f4487c4a11eb5d8ddb0d557cf1843f5c095ca7b8ac7934cffb1749fda1`  
		Last Modified: Tue, 30 Nov 2021 10:04:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8819eb039be2583d8ac33b58093d22333cf831436578279ec6095a0ed428ba`  
		Last Modified: Tue, 30 Nov 2021 10:05:47 GMT  
		Size: 14.1 MB (14128298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa041a02be98942b939ff817d153c101fb9a53ca998994f2eaafb3be2f684ea3`  
		Last Modified: Tue, 30 Nov 2021 10:05:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee62ec0bfaf1c06f17ea5e32207cccc98c74a922b2fbb4e337acb20920295538`  
		Last Modified: Wed, 08 Dec 2021 00:15:55 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb7a9edf3a4edc8a766785f3c38609492895a70dccecc125cc547c1d854be2e`  
		Last Modified: Thu, 06 Jan 2022 20:21:00 GMT  
		Size: 74.3 MB (74317308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bebba799ae7baf292d5c79a3d9029c7ca25d2de22d900182741b09da361cd7f`  
		Last Modified: Thu, 06 Jan 2022 20:20:50 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf04e39f78ce80ddb65f26ea90f79a60fb39e5896d702499f897e7d90ff90efc`  
		Last Modified: Thu, 06 Jan 2022 20:20:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebac2f2cc8f9520c335444647121563fb058efaf0c13ce9837c7210ad143146c`  
		Last Modified: Tue, 08 Mar 2022 20:59:06 GMT  
		Size: 3.1 MB (3065301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6dcc45ec2b76c6b6021e30f8cbf96c083b0cfdb2f0d8202da3bb4a9ae4ff53c`  
		Last Modified: Tue, 08 Mar 2022 20:59:09 GMT  
		Size: 57.2 MB (57240538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc00925167bd69eede75eccdb1f143d66de519654dff89b38876b190b4818eb`  
		Last Modified: Tue, 08 Mar 2022 20:59:05 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
