## `redmine:4-alpine3.16`

```console
$ docker pull redmine@sha256:6bdf478f71c614a8be6e6a2fa104677775c0f608331c284feef7f372560d0404
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

### `redmine:4-alpine3.16` - linux; amd64

```console
$ docker pull redmine@sha256:3953fe2a3dc6855592b5df2f1be57eae3efc49e43f2790fbbadc04ca8b0ffc1c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.9 MB (166925992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18416909653da5e522a0e714588bd17975eca5315e3ce82bebfce1d4bbdaeaae`
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
# Sat, 11 Feb 2023 13:45:37 GMT
ENV RUBY_MAJOR=2.7
# Sat, 11 Feb 2023 13:45:37 GMT
ENV RUBY_VERSION=2.7.7
# Sat, 11 Feb 2023 13:45:37 GMT
ENV RUBY_DOWNLOAD_SHA256=b38dff2e1f8ce6e5b7d433f8758752987a6b2adfd9bc7571dbc42ea5d04e3e4c
# Sat, 11 Feb 2023 13:47:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 13:47:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 13:47:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 13:47:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 13:47:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 11 Feb 2023 13:47:23 GMT
CMD ["irb"]
# Sat, 11 Feb 2023 17:16:03 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 11 Feb 2023 17:16:10 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 11 Feb 2023 17:16:11 GMT
ENV RAILS_ENV=production
# Sat, 11 Feb 2023 17:16:11 GMT
WORKDIR /usr/src/redmine
# Sat, 11 Feb 2023 17:16:11 GMT
ENV HOME=/home/redmine
# Sat, 11 Feb 2023 17:16:12 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 11 Feb 2023 17:16:12 GMT
ENV REDMINE_VERSION=4.2.9
# Sat, 11 Feb 2023 17:16:12 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.9.tar.gz
# Sat, 11 Feb 2023 17:16:12 GMT
ENV REDMINE_DOWNLOAD_SHA256=d38741345f6efd10c079898093b259d8dc4dcd8e41dfc4f64649685ae7a8cb1e
# Sat, 11 Feb 2023 17:16:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 11 Feb 2023 17:16:16 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 11 Feb 2023 17:18:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 11 Feb 2023 17:18:25 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 11 Feb 2023 17:18:26 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 11 Feb 2023 17:18:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 17:18:26 GMT
EXPOSE 3000
# Sat, 11 Feb 2023 17:18:26 GMT
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
	-	`sha256:e9fa8f51bd592dcb91d0ad4808468306c751ab1a99ea37bf632e00c66a8614e3`  
		Last Modified: Sat, 11 Feb 2023 13:50:37 GMT  
		Size: 13.9 MB (13898435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0472e55d35bcdb3be2756b642c711f1d39c587b61bdde12895ae69e86ab3bb5e`  
		Last Modified: Sat, 11 Feb 2023 13:50:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcde6bcd69f9a01832a86244944e96d3bd3db19e3cdd3ef6ebfde7d33c36e882`  
		Last Modified: Sat, 11 Feb 2023 17:19:55 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aaeda168638e17a49bad65aa6e2f457867230f2793ed5683fc3e34e2a79e4d`  
		Last Modified: Sat, 11 Feb 2023 17:20:08 GMT  
		Size: 90.4 MB (90398382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088f13dbd3efb35b6ce23240a0e61478cac2424da6630332071fc61671527f5e`  
		Last Modified: Sat, 11 Feb 2023 17:19:53 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294779fc2b5e06130227af238d6717084821e9e6fdd67bd02634591b7d36c65f`  
		Last Modified: Sat, 11 Feb 2023 17:19:53 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50e42a44a700fe0cd719a1ae1991d99d09b65e4eef0c5ef39234dae2acaad7e`  
		Last Modified: Sat, 11 Feb 2023 17:19:54 GMT  
		Size: 3.1 MB (3069002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e44340155eb481f836d4313851c77375609d075569d1e0a9475788b63f3452d2`  
		Last Modified: Sat, 11 Feb 2023 17:20:03 GMT  
		Size: 52.9 MB (52896966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2929f313f01cf63f607e2b6f4198afda088ab78843c09f86b212e93c2ed1a67f`  
		Last Modified: Sat, 11 Feb 2023 17:19:53 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.16` - linux; arm variant v6

```console
$ docker pull redmine@sha256:29342ec1f10393154b6d720db689facde9be09670fd467dcec0195eb392d9897
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.8 MB (158758078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fd2be2edf017f73d787ae7194304474936152fd0fe843a274f38e95278eaa1b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 06:54:50 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 11 Feb 2023 06:54:51 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 11 Feb 2023 06:54:51 GMT
ENV LANG=C.UTF-8
# Sat, 11 Feb 2023 07:07:24 GMT
ENV RUBY_MAJOR=2.7
# Sat, 11 Feb 2023 07:07:24 GMT
ENV RUBY_VERSION=2.7.7
# Sat, 11 Feb 2023 07:07:24 GMT
ENV RUBY_DOWNLOAD_SHA256=b38dff2e1f8ce6e5b7d433f8758752987a6b2adfd9bc7571dbc42ea5d04e3e4c
# Sat, 11 Feb 2023 07:10:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 07:10:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 07:10:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 07:10:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 07:10:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 11 Feb 2023 07:10:05 GMT
CMD ["irb"]
# Sat, 11 Feb 2023 10:05:46 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 11 Feb 2023 10:06:01 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 11 Feb 2023 10:06:02 GMT
ENV RAILS_ENV=production
# Sat, 11 Feb 2023 10:06:02 GMT
WORKDIR /usr/src/redmine
# Sat, 11 Feb 2023 10:06:03 GMT
ENV HOME=/home/redmine
# Sat, 11 Feb 2023 10:06:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 11 Feb 2023 10:06:04 GMT
ENV REDMINE_VERSION=4.2.9
# Sat, 11 Feb 2023 10:06:05 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.9.tar.gz
# Sat, 11 Feb 2023 10:06:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=d38741345f6efd10c079898093b259d8dc4dcd8e41dfc4f64649685ae7a8cb1e
# Sat, 11 Feb 2023 10:06:10 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 11 Feb 2023 10:06:10 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 11 Feb 2023 10:09:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 11 Feb 2023 10:09:25 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 11 Feb 2023 10:09:25 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 11 Feb 2023 10:09:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 10:09:26 GMT
EXPOSE 3000
# Sat, 11 Feb 2023 10:09:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d088b1a6f43566b0657c1a55e6469cc5165dd2c567849208462acae1059c82`  
		Last Modified: Sat, 11 Feb 2023 07:12:17 GMT  
		Size: 3.6 MB (3593789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174cb3777a786b751b7b330c4a84fe5bd3b428c2613f392498d33cf9ac5f6e7d`  
		Last Modified: Sat, 11 Feb 2023 07:12:15 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a56e73c0dcb4a6bbb9fbf635eac9cac374f4696fdc059258f8a5b80cb66cbb8`  
		Last Modified: Sat, 11 Feb 2023 07:13:35 GMT  
		Size: 13.4 MB (13439666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9104cb2deda1cf01fb1fa6632deea1ce7567c17d8cd1106e6ee8837d31e0e966`  
		Last Modified: Sat, 11 Feb 2023 07:13:33 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbf723c8223a3247285c5ff3cd71e54e1433b7553f90d44d7c12df900ca6350`  
		Last Modified: Sat, 11 Feb 2023 10:11:35 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb7712868c113aac166c7058ca2b86b199a5db6ffcd5eee340a67e3f1c968fa`  
		Last Modified: Sat, 11 Feb 2023 10:11:55 GMT  
		Size: 83.9 MB (83907774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ac8ef05e7362e52337edad87730c78248d9b10bf6dcb83e6fab54f265f44ce`  
		Last Modified: Sat, 11 Feb 2023 10:11:33 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6525bf4e0a071a484c4cecbb49bb3fb9a10295613b2462370b11282d33312c`  
		Last Modified: Sat, 11 Feb 2023 10:11:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7325bb1c634ae3f3e2e8ab2f6cd9c766845fec46a198172a049bfcc39b949172`  
		Last Modified: Sat, 11 Feb 2023 10:11:34 GMT  
		Size: 3.1 MB (3068327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaaaa03f8edcbdccb3695016462c2b0faffc4dc34d529f7e05d3ecbc01218fb3`  
		Last Modified: Sat, 11 Feb 2023 10:11:43 GMT  
		Size: 52.1 MB (52127933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa50a6c259f4eb9988b56ac6a9ca3ebd9c5653ef5ef83d36aa95963ebffee77b`  
		Last Modified: Sat, 11 Feb 2023 10:11:33 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.16` - linux; arm variant v7

```console
$ docker pull redmine@sha256:b34e5f80419ac3d50e1d3a4641c2666ef3796777378542d9a2d40cf3c3e34fc6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156089180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3bd574f04bd15a36270ef59468a0e372c94d7b16533d5e51d682ff6a301639`
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
# Wed, 01 Mar 2023 16:36:23 GMT
ENV RUBY_MAJOR=2.7
# Wed, 01 Mar 2023 16:36:23 GMT
ENV RUBY_VERSION=2.7.7
# Wed, 01 Mar 2023 16:36:23 GMT
ENV RUBY_DOWNLOAD_SHA256=b38dff2e1f8ce6e5b7d433f8758752987a6b2adfd9bc7571dbc42ea5d04e3e4c
# Wed, 01 Mar 2023 16:38:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Mar 2023 16:38:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Mar 2023 16:38:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Mar 2023 16:38:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 16:38:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Mar 2023 16:38:03 GMT
CMD ["irb"]
# Thu, 02 Mar 2023 06:07:05 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 02 Mar 2023 06:07:13 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 02 Mar 2023 06:07:14 GMT
ENV RAILS_ENV=production
# Thu, 02 Mar 2023 06:07:14 GMT
WORKDIR /usr/src/redmine
# Thu, 02 Mar 2023 06:07:15 GMT
ENV HOME=/home/redmine
# Thu, 02 Mar 2023 06:07:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 02 Mar 2023 06:07:15 GMT
ENV REDMINE_VERSION=4.2.9
# Thu, 02 Mar 2023 06:07:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.9.tar.gz
# Thu, 02 Mar 2023 06:07:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=d38741345f6efd10c079898093b259d8dc4dcd8e41dfc4f64649685ae7a8cb1e
# Thu, 02 Mar 2023 06:07:18 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 02 Mar 2023 06:07:19 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 02 Mar 2023 06:09:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 02 Mar 2023 06:09:38 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 02 Mar 2023 06:09:38 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 02 Mar 2023 06:09:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 02 Mar 2023 06:09:38 GMT
EXPOSE 3000
# Thu, 02 Mar 2023 06:09:38 GMT
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
	-	`sha256:be74b43bb833c6432c31f15dd61d34bd4470c7773c77aef1fb2bc20b14fa7377`  
		Last Modified: Wed, 01 Mar 2023 16:48:30 GMT  
		Size: 13.3 MB (13305722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ccf78f4d468c7c10d5a50b7773cf3d9811df3b3c7d681225e7cb0620c3be79d`  
		Last Modified: Wed, 01 Mar 2023 16:48:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6106a4f3d6a3b9a0152c10fd152bee0a836f635401b2a9022666a4cb5f7315e7`  
		Last Modified: Thu, 02 Mar 2023 06:13:04 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:810fb3b3e576dc9972bff557bab87a9fcf681e30114c0cbca6af61b12f635bf2`  
		Last Modified: Thu, 02 Mar 2023 06:13:16 GMT  
		Size: 82.0 MB (82022707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9449276894251644e59b5cdcc7bffe52ac6d113917f57ad598f7e7f580079c73`  
		Last Modified: Thu, 02 Mar 2023 06:13:02 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433d11b571875d61c2b7e166fcf56329b1164404b7f79d126f1466cb1e33f758`  
		Last Modified: Thu, 02 Mar 2023 06:13:02 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aaa829ac3e3407cffad265b50b89e5f26b3879fed16d2615b11ab5238bfcae`  
		Last Modified: Thu, 02 Mar 2023 06:13:03 GMT  
		Size: 3.1 MB (3068873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762bc626fc91fc694f16146430f9720cf60597f847ace2e01d08106299ee2462`  
		Last Modified: Thu, 02 Mar 2023 06:13:07 GMT  
		Size: 51.8 MB (51805689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7be27aa7be5ff9c0ddc276bbd8484b536c68c4dfa66b0a418a95cc1fde64cc`  
		Last Modified: Thu, 02 Mar 2023 06:13:02 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:1d8f703a200f3202963d4291ce64edf362313e56ba34520152cb11048f231b4f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.3 MB (163307072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28ee15c2b0ef11b5e01fe709d832093d4279112a1d7a2c0cebfabff0cd41af6c`
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
# Sat, 11 Feb 2023 05:33:00 GMT
ENV RUBY_MAJOR=2.7
# Sat, 11 Feb 2023 05:33:01 GMT
ENV RUBY_VERSION=2.7.7
# Sat, 11 Feb 2023 05:33:01 GMT
ENV RUBY_DOWNLOAD_SHA256=b38dff2e1f8ce6e5b7d433f8758752987a6b2adfd9bc7571dbc42ea5d04e3e4c
# Sat, 11 Feb 2023 05:34:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 05:34:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 05:34:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 05:34:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:34:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 11 Feb 2023 05:34:22 GMT
CMD ["irb"]
# Sat, 11 Feb 2023 08:49:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 11 Feb 2023 08:49:33 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 11 Feb 2023 08:49:35 GMT
ENV RAILS_ENV=production
# Sat, 11 Feb 2023 08:49:35 GMT
WORKDIR /usr/src/redmine
# Sat, 11 Feb 2023 08:49:35 GMT
ENV HOME=/home/redmine
# Sat, 11 Feb 2023 08:49:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 11 Feb 2023 08:49:35 GMT
ENV REDMINE_VERSION=4.2.9
# Sat, 11 Feb 2023 08:49:35 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.9.tar.gz
# Sat, 11 Feb 2023 08:49:35 GMT
ENV REDMINE_DOWNLOAD_SHA256=d38741345f6efd10c079898093b259d8dc4dcd8e41dfc4f64649685ae7a8cb1e
# Sat, 11 Feb 2023 08:49:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 11 Feb 2023 08:49:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 11 Feb 2023 08:51:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 11 Feb 2023 08:51:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 11 Feb 2023 08:51:37 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 11 Feb 2023 08:51:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 08:51:37 GMT
EXPOSE 3000
# Sat, 11 Feb 2023 08:51:37 GMT
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
	-	`sha256:e7a60a395fe9caee05bb8aa07c22380f843ef32a8bbc8b60d0ffe172dc4b8448`  
		Last Modified: Sat, 11 Feb 2023 05:37:44 GMT  
		Size: 13.7 MB (13739558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a644c40157e7c87d4b62227999a92338f4b12df8e0174e57af9b82c0b21b4ab0`  
		Last Modified: Sat, 11 Feb 2023 05:37:43 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132025542dbeb4b71243f3e6d7ea0a4f31853451d06b5277e0e584a1e6d1f5d7`  
		Last Modified: Sat, 11 Feb 2023 08:53:01 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31551108e43bea180e9372c1f3d1c8c4e13679a22c4ca9db9b27e7af2f3cafdc`  
		Last Modified: Sat, 11 Feb 2023 08:53:11 GMT  
		Size: 87.3 MB (87258894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf2ab863422c0c1c27f2011dd7422673babf4835b6f2cc6150fc499adbb720e`  
		Last Modified: Sat, 11 Feb 2023 08:52:59 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ccf954418cdfe9e31b3f4bfe7f3374129b512428ae8970a34d4fd897a04599`  
		Last Modified: Sat, 11 Feb 2023 08:52:59 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff330a54123317db2d79f44972e04a0a977e03574dcbebbeae57f1c633e3312`  
		Last Modified: Sat, 11 Feb 2023 08:53:00 GMT  
		Size: 3.1 MB (3068934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab4bdfc867e76604d011b3e4b30046078b332de40f5697243578b984b8a226e`  
		Last Modified: Sat, 11 Feb 2023 08:53:03 GMT  
		Size: 52.7 MB (52704821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f74564c752a21ac2cd3bc48f1d017897d599924d63d65c19660ffcb4636b34d1`  
		Last Modified: Sat, 11 Feb 2023 08:52:59 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.16` - linux; 386

```console
$ docker pull redmine@sha256:65a8eddc392c2716f0e1bee3af5b251690e6ae6fdb0bb5a2992c108bef28987c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.6 MB (165573345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a17f99561f228760183dcaf20babd4855b82d79f3ba028991ba137efe72744dd`
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
# Wed, 01 Mar 2023 09:03:39 GMT
ENV RUBY_MAJOR=2.7
# Wed, 01 Mar 2023 09:03:40 GMT
ENV RUBY_VERSION=2.7.7
# Wed, 01 Mar 2023 09:03:40 GMT
ENV RUBY_DOWNLOAD_SHA256=b38dff2e1f8ce6e5b7d433f8758752987a6b2adfd9bc7571dbc42ea5d04e3e4c
# Wed, 01 Mar 2023 09:06:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Mar 2023 09:06:51 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Mar 2023 09:06:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Mar 2023 09:06:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 09:06:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Mar 2023 09:06:52 GMT
CMD ["irb"]
# Thu, 02 Mar 2023 05:35:26 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 02 Mar 2023 05:35:36 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 02 Mar 2023 05:35:37 GMT
ENV RAILS_ENV=production
# Thu, 02 Mar 2023 05:35:37 GMT
WORKDIR /usr/src/redmine
# Thu, 02 Mar 2023 05:35:37 GMT
ENV HOME=/home/redmine
# Thu, 02 Mar 2023 05:35:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 02 Mar 2023 05:35:38 GMT
ENV REDMINE_VERSION=4.2.9
# Thu, 02 Mar 2023 05:35:38 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.9.tar.gz
# Thu, 02 Mar 2023 05:35:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=d38741345f6efd10c079898093b259d8dc4dcd8e41dfc4f64649685ae7a8cb1e
# Thu, 02 Mar 2023 05:35:42 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 02 Mar 2023 05:35:42 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 02 Mar 2023 05:38:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 02 Mar 2023 05:38:21 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 02 Mar 2023 05:38:21 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 02 Mar 2023 05:38:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 02 Mar 2023 05:38:22 GMT
EXPOSE 3000
# Thu, 02 Mar 2023 05:38:22 GMT
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
	-	`sha256:44e877ba7082517095372e290a95ab270a609b5d5c53043004007be930c825c1`  
		Last Modified: Wed, 01 Mar 2023 09:17:08 GMT  
		Size: 13.3 MB (13318931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed5107a538f87a8468f9914ed5c60e83f29aea79c4a6ec6943785312efa804b`  
		Last Modified: Wed, 01 Mar 2023 09:17:05 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9937e48d5af69910f1e922a0a31ee7b53605d9db5b90f6b997b9ec69ec94988b`  
		Last Modified: Thu, 02 Mar 2023 05:42:08 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9225750e00098ae9f10eda80327c1f46de5cacd2cef8f2c2527766d39b4683b`  
		Last Modified: Thu, 02 Mar 2023 05:42:26 GMT  
		Size: 90.3 MB (90264839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e2a047e1807fe405e3a4fd1753aa262b535cd9756d93ede2d7660d114fcd0a`  
		Last Modified: Thu, 02 Mar 2023 05:42:06 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40f08124b03363e7fbab25ac83afb70509076bb799081e4ee7180106be407af`  
		Last Modified: Thu, 02 Mar 2023 05:42:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a489593c27dfcf8741375fc684d87c61c61fb59e9bae10e9f233313e27e7a1e6`  
		Last Modified: Thu, 02 Mar 2023 05:42:07 GMT  
		Size: 3.1 MB (3068915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99acf0e5aeab881bd04e703a0dc98dc996b36bc6aac64a35da1e12709593620`  
		Last Modified: Thu, 02 Mar 2023 05:42:14 GMT  
		Size: 52.2 MB (52219328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e66b3bdfa8d9ab2fe1d38819d8bc18ebb7a7922b607e8783e26164f0b479385`  
		Last Modified: Thu, 02 Mar 2023 05:42:06 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.16` - linux; ppc64le

```console
$ docker pull redmine@sha256:46f7b374fcf23b983d37cc6adcbd5ea1b7947a07db2f5b43410d8c200ffc7c06
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174268879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5718119e15e232b6fc379d8be3504dccfcbc7f6dae14a59923e98e87efc56f7f`
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
# Sat, 11 Feb 2023 05:24:44 GMT
ENV RUBY_MAJOR=2.7
# Sat, 11 Feb 2023 05:24:45 GMT
ENV RUBY_VERSION=2.7.7
# Sat, 11 Feb 2023 05:24:45 GMT
ENV RUBY_DOWNLOAD_SHA256=b38dff2e1f8ce6e5b7d433f8758752987a6b2adfd9bc7571dbc42ea5d04e3e4c
# Sat, 11 Feb 2023 05:27:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 05:27:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 05:27:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 05:27:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 05:27:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 11 Feb 2023 05:27:55 GMT
CMD ["irb"]
# Sat, 11 Feb 2023 12:58:50 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 11 Feb 2023 12:59:06 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 11 Feb 2023 12:59:11 GMT
ENV RAILS_ENV=production
# Sat, 11 Feb 2023 12:59:11 GMT
WORKDIR /usr/src/redmine
# Sat, 11 Feb 2023 12:59:12 GMT
ENV HOME=/home/redmine
# Sat, 11 Feb 2023 12:59:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 11 Feb 2023 12:59:13 GMT
ENV REDMINE_VERSION=4.2.9
# Sat, 11 Feb 2023 12:59:14 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.9.tar.gz
# Sat, 11 Feb 2023 12:59:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=d38741345f6efd10c079898093b259d8dc4dcd8e41dfc4f64649685ae7a8cb1e
# Sat, 11 Feb 2023 12:59:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 11 Feb 2023 12:59:20 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 11 Feb 2023 13:03:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 11 Feb 2023 13:04:00 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 11 Feb 2023 13:04:01 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 11 Feb 2023 13:04:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 13:04:02 GMT
EXPOSE 3000
# Sat, 11 Feb 2023 13:04:03 GMT
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
	-	`sha256:05182a5900b0c1ee365734648bbdb9aeb049e0f392cecadc171fb363b01f42a7`  
		Last Modified: Sat, 11 Feb 2023 05:33:26 GMT  
		Size: 14.4 MB (14399210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b3fa43f7e373185842955dcdaa38392f269dfd47713150e8b6f3b0a37028d2`  
		Last Modified: Sat, 11 Feb 2023 05:33:22 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2ae6b6ddfa2165c17b06e363f2919968e3544e5e4eff18e48298ffdb8bec3b`  
		Last Modified: Sat, 11 Feb 2023 13:06:21 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfaafd369918ae134b8245b64fe579d3f2509f7e8dd7d64368a6e75c8af2500`  
		Last Modified: Sat, 11 Feb 2023 13:06:46 GMT  
		Size: 96.3 MB (96275778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83da2169b374cf16c1053678245266655ee7f166d7d38025b57aa56aa2cf9c38`  
		Last Modified: Sat, 11 Feb 2023 13:06:19 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d8abd2d4d0eadb0f2d4c5dd5fd28d47fb0c2b5da40029be4469afbfac04413`  
		Last Modified: Sat, 11 Feb 2023 13:06:19 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e64ff486acfb7da3f0c853e81efb34fe807ae07130877b4738bec9acdb179f`  
		Last Modified: Sat, 11 Feb 2023 13:06:21 GMT  
		Size: 3.1 MB (3068942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551a25d2058912622f3b1fd37411b3b99167a8de75e3e15644c3365590819498`  
		Last Modified: Sat, 11 Feb 2023 13:06:29 GMT  
		Size: 53.7 MB (53742766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d190c6a6cd5197e88f17328546171c232b8eeeb838e2e97ff5847713a164c9`  
		Last Modified: Sat, 11 Feb 2023 13:06:19 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.16` - linux; s390x

```console
$ docker pull redmine@sha256:ace6d49e6672a3c4a51d4a8074ca0bd80454a25b769bf6cb73fda3a41dc22602
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.1 MB (157140022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72e29dac024c95d7146e2d6ab1b768301b6af0a5c104ee3222e41be5c2ec13ce`
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
# Sat, 11 Feb 2023 11:03:44 GMT
ENV RUBY_MAJOR=2.7
# Sat, 11 Feb 2023 11:03:45 GMT
ENV RUBY_VERSION=2.7.7
# Sat, 11 Feb 2023 11:03:45 GMT
ENV RUBY_DOWNLOAD_SHA256=b38dff2e1f8ce6e5b7d433f8758752987a6b2adfd9bc7571dbc42ea5d04e3e4c
# Sat, 11 Feb 2023 11:05:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 11 Feb 2023 11:05:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 11 Feb 2023 11:05:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 11 Feb 2023 11:05:20 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 11:05:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 11 Feb 2023 11:05:20 GMT
CMD ["irb"]
# Sat, 11 Feb 2023 12:58:54 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 11 Feb 2023 12:59:01 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 11 Feb 2023 12:59:05 GMT
ENV RAILS_ENV=production
# Sat, 11 Feb 2023 12:59:05 GMT
WORKDIR /usr/src/redmine
# Sat, 11 Feb 2023 12:59:05 GMT
ENV HOME=/home/redmine
# Sat, 11 Feb 2023 12:59:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 11 Feb 2023 12:59:06 GMT
ENV REDMINE_VERSION=4.2.9
# Sat, 11 Feb 2023 12:59:06 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.9.tar.gz
# Sat, 11 Feb 2023 12:59:06 GMT
ENV REDMINE_DOWNLOAD_SHA256=d38741345f6efd10c079898093b259d8dc4dcd8e41dfc4f64649685ae7a8cb1e
# Sat, 11 Feb 2023 12:59:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 11 Feb 2023 12:59:09 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 11 Feb 2023 13:00:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 11 Feb 2023 13:01:00 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 11 Feb 2023 13:01:00 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 11 Feb 2023 13:01:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 11 Feb 2023 13:01:00 GMT
EXPOSE 3000
# Sat, 11 Feb 2023 13:01:00 GMT
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
	-	`sha256:e84dd382957a4fab35f797d2008bc2dc2761f77ebc7792bd29d30b04a7669188`  
		Last Modified: Sat, 11 Feb 2023 11:09:35 GMT  
		Size: 13.8 MB (13825210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1bf5f20c2a79e0d80362142742cdea4614781c6e7b9a3c44193ce7a7101fc30`  
		Last Modified: Sat, 11 Feb 2023 11:09:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f7359f1d66477a1794fffa88428ae664fa33cf870257b989f0a5777bdb4304`  
		Last Modified: Sat, 11 Feb 2023 13:02:46 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5f4df3aa1304fba99123206cef7e58133b4a5430806cdd85a59e3705798fe9`  
		Last Modified: Sat, 11 Feb 2023 13:02:56 GMT  
		Size: 80.8 MB (80835852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e7273a9702b04455f5ca2c4ea1d8632d8c0fec4c1227f8308956aede11f5b`  
		Last Modified: Sat, 11 Feb 2023 13:02:45 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f456143d07185d771d367178655f59e89a77692b8f5584c760fe581d4293a0c`  
		Last Modified: Sat, 11 Feb 2023 13:02:45 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df4cdab1d8e3d29243418ff069eb199ca158c94b3269a0128e557514cf80d20`  
		Last Modified: Sat, 11 Feb 2023 13:02:46 GMT  
		Size: 3.1 MB (3069011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e631300db7045a607806b4c9fafac51b4ac72e3485cb5524d6b47fadaf9663`  
		Last Modified: Sat, 11 Feb 2023 13:02:50 GMT  
		Size: 52.9 MB (52871361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36c5ece9ac6ae38f858da33821f39662ad069d8dc28ff582032458126911a0a4`  
		Last Modified: Sat, 11 Feb 2023 13:02:45 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
