## `redmine:4-alpine3.15`

```console
$ docker pull redmine@sha256:468a1c49fc19b94b5a674142d358db68e416559fdfd63096de2e4d94f74cea05
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
$ docker pull redmine@sha256:851ccb02ee1eadd1f2f282810d4f0246baab45b0e1f335e21c511a65afde36a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.0 MB (160980955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d362221f4a9a5fa727eea3a5b16f547edff36c79e8944523328b786a8dd620c`
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
# Tue, 05 Apr 2022 03:32:43 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 18:55:43 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 18:55:43 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 18:57:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 18:57:26 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 18:57:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 18:57:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 18:57:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 18:57:27 GMT
CMD ["irb"]
# Tue, 12 Apr 2022 19:58:06 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 12 Apr 2022 19:58:14 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 12 Apr 2022 19:58:15 GMT
ENV RAILS_ENV=production
# Tue, 12 Apr 2022 19:58:15 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Apr 2022 19:58:15 GMT
ENV HOME=/home/redmine
# Tue, 12 Apr 2022 19:58:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:02:40 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 02:02:40 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 02:02:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 02:02:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:02:43 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 02:04:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 02:04:53 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:04:53 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 02:04:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:04:53 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:04:53 GMT
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
	-	`sha256:2f1b0fc20e43ff265f2bc9c57f278423445f4f2905785deda94f5a0b0da399d9`  
		Last Modified: Tue, 12 Apr 2022 19:19:16 GMT  
		Size: 14.0 MB (13980571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56d8c6ef3c8315c36873b0dde952db2d2f60c01b2d48753766227bbcf480a73`  
		Last Modified: Tue, 12 Apr 2022 19:19:14 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c166a9d8aad28f33274ae35592d7c12cfadd4371321a5d3bfab42650c180e8fb`  
		Last Modified: Tue, 12 Apr 2022 20:08:18 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ac2bb42142982c9239c56304eba684d9767765238a800ec00f73f477df21c0`  
		Last Modified: Tue, 12 Apr 2022 20:08:30 GMT  
		Size: 82.2 MB (82231750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3459af0cf3af7906e851778897088ed7a77cc97cc207852141fa88f9bbd2d63f`  
		Last Modified: Tue, 12 Apr 2022 20:08:16 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8681feda746b6af278739436a0fc6f67e10314aea591b254c540484134eb0a`  
		Last Modified: Tue, 12 Apr 2022 20:08:16 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47820179d62b6654d70bc3d6fd33f0606a8a4192e9d476d4695378f3b2bca946`  
		Last Modified: Wed, 22 Jun 2022 02:07:26 GMT  
		Size: 3.1 MB (3067028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb044aeeee1dcc9bf48a516005867ebfc9173b9a880b85173116e4aad1f8f28c`  
		Last Modified: Wed, 22 Jun 2022 02:07:31 GMT  
		Size: 55.2 MB (55199795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640cb426a63fa37b60ec3420c7177c93bb6e1da4d3fe68abd158cff05b307531`  
		Last Modified: Wed, 22 Jun 2022 02:07:25 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; arm variant v6

```console
$ docker pull redmine@sha256:fb35b1c65258b0f977573184403658951a3b333264dff6dea545608cd3d75329
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.3 MB (154300331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6113c9758606b2477f1e41c747b89fc6f5e888efa82e82d6d180a58bbad81ef0`
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
# Tue, 05 Apr 2022 02:12:27 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 19:09:21 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 19:09:22 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 19:13:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:13:10 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:13:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:13:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:13:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:13:13 GMT
CMD ["irb"]
# Tue, 12 Apr 2022 19:54:46 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 12 Apr 2022 19:55:16 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 12 Apr 2022 19:55:18 GMT
ENV RAILS_ENV=production
# Tue, 12 Apr 2022 19:55:18 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Apr 2022 19:55:19 GMT
ENV HOME=/home/redmine
# Tue, 12 Apr 2022 19:55:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 01:57:20 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 01:57:20 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 01:57:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 01:57:28 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 01:57:29 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 02:03:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 02:03:49 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:03:50 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 02:03:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:03:51 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:03:51 GMT
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
	-	`sha256:d14d063246c143639357fe6e93cfdb6be9be70df5ef4ef1f89e8d762d7764604`  
		Last Modified: Tue, 12 Apr 2022 19:31:21 GMT  
		Size: 13.4 MB (13412168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803cc631b17a95f18e33a337cd3392dde8ec43e730f8fe53405019a219ab4583`  
		Last Modified: Tue, 12 Apr 2022 19:31:15 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afca80ecfbf6203148cc277d73e614268c53d7c53e592e11526736324ebfe96`  
		Last Modified: Tue, 12 Apr 2022 20:12:00 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3427d99e3724c6f8d5d11122dedb99a13f249da5b1734f1fcef48d3a2c9fbd2`  
		Last Modified: Tue, 12 Apr 2022 20:12:52 GMT  
		Size: 77.7 MB (77699502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a333f4f0b96bf5f7f9deb35eec3ecfe62fb9b3a6dc34ab792f46ee0fa6771bd7`  
		Last Modified: Tue, 12 Apr 2022 20:11:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e3eda0a85742840d0a03e4bbddf7f0417898c7ec57a0eba559ec847addfd738`  
		Last Modified: Tue, 12 Apr 2022 20:11:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9484446267af9a5e07eb56dd4a6d7148552cc52f4e798458a1e657022f71dbf`  
		Last Modified: Wed, 22 Jun 2022 02:06:29 GMT  
		Size: 3.1 MB (3067070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff73207e5de6132e0d44546a63db129b66283317084a71bd1eb410f360dc87f1`  
		Last Modified: Wed, 22 Jun 2022 02:06:51 GMT  
		Size: 54.1 MB (54064305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de8c45f1f9699454de9a4ed8ce7459d01703d598511f851d55232a06130e3c`  
		Last Modified: Wed, 22 Jun 2022 02:06:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; arm variant v7

```console
$ docker pull redmine@sha256:761a720f571dcae2b77d22d66c416a431824a1ffd779a147435cfe2477f50073
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.0 MB (150025949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df1577025ac62c833066d3697f3d60daca0edd1c6a1c170deccaf4ff4412c77d`
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
# Tue, 05 Apr 2022 03:43:27 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 20:12:11 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 20:12:11 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 20:15:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 20:15:31 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 20:15:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 20:15:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 20:15:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 20:15:33 GMT
CMD ["irb"]
# Wed, 13 Apr 2022 02:53:20 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 13 Apr 2022 02:53:51 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 13 Apr 2022 02:53:52 GMT
ENV RAILS_ENV=production
# Wed, 13 Apr 2022 02:53:53 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Apr 2022 02:53:53 GMT
ENV HOME=/home/redmine
# Wed, 13 Apr 2022 02:53:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 03:48:38 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 03:48:39 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 03:48:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 03:48:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 03:48:46 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 03:54:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 03:54:34 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 03:54:34 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 03:54:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 03:54:35 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 03:54:35 GMT
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
	-	`sha256:db348fdd8eec59ffbf61656974ad18acb6ce5b85f041d971169c15aa99dd304a`  
		Last Modified: Tue, 12 Apr 2022 21:03:58 GMT  
		Size: 13.3 MB (13301907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229623706c6989ddd690cfaf7c87a113158ac019297bd5284d2a8ace7f43ebe6`  
		Last Modified: Tue, 12 Apr 2022 21:03:54 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e92f223765a01ea367ffe2ff4d1c69a90a65ac2f75189fd1022e02952b3394f`  
		Last Modified: Wed, 13 Apr 2022 03:18:56 GMT  
		Size: 1.2 KB (1223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f62b75aed2849dcd31da8b67f8587eb33fc08e373ddf4a3eb48788c2731b1a7d`  
		Last Modified: Wed, 13 Apr 2022 03:19:44 GMT  
		Size: 74.3 MB (74255265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6007f93565ebb04ab52a192be194aee3a5577316baffe170876e2f760eae4dde`  
		Last Modified: Wed, 13 Apr 2022 03:18:54 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c5cb4b524c88e92799f8a9c7d43d483cc0120079706bc0a04adbceeb65083ce`  
		Last Modified: Wed, 13 Apr 2022 03:18:54 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e3de11d019abdeb460bdb9cb6fcdcf5afea2610b78ddda56228ffeab08c954`  
		Last Modified: Wed, 22 Jun 2022 04:00:04 GMT  
		Size: 3.1 MB (3067029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3894098ecbba35400c9817df62f1a640e9560522a1f20b448be2af3195f3a8d`  
		Last Modified: Wed, 22 Jun 2022 04:00:24 GMT  
		Size: 53.7 MB (53671736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15275d4dd2c14557cad92765280d25d819147f023f4081d936ae5ba068cc593a`  
		Last Modified: Wed, 22 Jun 2022 04:00:00 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:78881f458d56e65349092c8ff405cb4412560fb9db0754691df68ae106aadfbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.6 MB (157612082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2cce00599d05b9e4413e4bd82d210428f96ad7110968890068dee00abfc3af8`
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
# Tue, 05 Apr 2022 02:28:18 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 19:16:48 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 19:16:49 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 19:18:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:18:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:18:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:18:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:18:45 GMT
CMD ["irb"]
# Tue, 12 Apr 2022 21:51:23 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 12 Apr 2022 21:51:32 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 12 Apr 2022 21:51:33 GMT
ENV RAILS_ENV=production
# Tue, 12 Apr 2022 21:51:33 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Apr 2022 21:51:34 GMT
ENV HOME=/home/redmine
# Tue, 12 Apr 2022 21:51:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:58:47 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 02:58:48 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 02:58:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 02:58:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:58:54 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 03:01:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 03:01:32 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 03:01:33 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 03:01:33 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 03:01:34 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 03:01:35 GMT
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
	-	`sha256:630fc641f979699b23e5879d68651796fe78cc68713b31e606a38e76fa48ed7c`  
		Last Modified: Tue, 12 Apr 2022 19:43:41 GMT  
		Size: 13.8 MB (13813960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14dc7c87c4ac327aa4fbe3b80d1e2eb6533313c22573edc00db55c5041c693f2`  
		Last Modified: Tue, 12 Apr 2022 19:43:39 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d739413346f6e7f9f8d9bb62962ed7370b06e1e2e1acf2e7d98c72dd461f61a`  
		Last Modified: Tue, 12 Apr 2022 22:03:48 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78fe6b6855a7bd6331b2ebc2b152acdb69d502303eccfe9e64175251a42e639`  
		Last Modified: Tue, 12 Apr 2022 22:04:00 GMT  
		Size: 79.5 MB (79477811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a6fbca1f2fc92b59c1b7ebe0cf75a0c229867e8a1b6a2daf46f66d4938c584`  
		Last Modified: Tue, 12 Apr 2022 22:03:46 GMT  
		Size: 133.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a178d0e197dea1e3f1701a2b745aa0f486188804eab71a8ba98402f164b3ee`  
		Last Modified: Tue, 12 Apr 2022 22:03:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71fb359d8344df71d20438858432af0a46119e967a5fc5efecee29e4782e3afb`  
		Last Modified: Wed, 22 Jun 2022 03:04:26 GMT  
		Size: 3.1 MB (3067420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13894446cd1be743c606ee56364170e8badd8b664559a6768833818dceda254c`  
		Last Modified: Wed, 22 Jun 2022 03:04:31 GMT  
		Size: 54.9 MB (54886745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6ccd6c8236fa08600784fc34311eafc30037cc00d46382e79656222ae0fa99`  
		Last Modified: Wed, 22 Jun 2022 03:04:25 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; 386

```console
$ docker pull redmine@sha256:ea1745f22537e2a8a7d3ea336f39f1ca0589b5487630a60c91e44b0e6e20c3cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.2 MB (161188172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dcb7c93bf8c1b48c34deff645c288fb590bc9042deae218d66b1065c79f0feb`
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
# Tue, 05 Apr 2022 02:00:50 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 19:15:14 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 19:15:15 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 19:16:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:16:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:16:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:16:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:17:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:17:01 GMT
CMD ["irb"]
# Tue, 12 Apr 2022 21:44:56 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 12 Apr 2022 21:45:06 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 12 Apr 2022 21:45:07 GMT
ENV RAILS_ENV=production
# Tue, 12 Apr 2022 21:45:07 GMT
WORKDIR /usr/src/redmine
# Tue, 12 Apr 2022 21:45:08 GMT
ENV HOME=/home/redmine
# Tue, 12 Apr 2022 21:45:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:11:58 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 02:11:59 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 02:12:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 02:12:04 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:12:05 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 02:14:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 02:14:22 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:14:24 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 02:14:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:14:25 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:14:26 GMT
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
	-	`sha256:406e996b0a6c5bb9e7ddbee220a24bbf7c02b0d6eca49a00c35b9449c9f4a7e9`  
		Last Modified: Tue, 12 Apr 2022 19:42:14 GMT  
		Size: 13.3 MB (13291781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad32bb3550bafe1f4cd5d646830db3edff4b1e39b4e6d8fb87f8831c9fa2e875`  
		Last Modified: Tue, 12 Apr 2022 19:42:10 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452089c454562072f20ce37de3a6806346d01554c75c0e53a6171bf009d7be46`  
		Last Modified: Tue, 12 Apr 2022 21:55:41 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad6e5b3d5249ed026f4f44d4d0cddbab0fb50fc97749986c4fb34e5265f8e76f`  
		Last Modified: Tue, 12 Apr 2022 21:56:02 GMT  
		Size: 83.8 MB (83842817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5378b9425a47b88d9e8db4ee4702649d7027c7d39ed65cd114106806a209122d`  
		Last Modified: Tue, 12 Apr 2022 21:55:39 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe233225c484c9e665d33ade86e16bbfeadfd7d64eed1256c3e3b3d549e16bb3`  
		Last Modified: Tue, 12 Apr 2022 21:55:39 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba3c91fab4204939b82fa9a200193446662e384fe1e481f19b13660d227a9c9`  
		Last Modified: Wed, 22 Jun 2022 02:17:44 GMT  
		Size: 3.1 MB (3067367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52edc8d5b766a064d3c8cf504290156d81da673388f857f802e924d3657fee25`  
		Last Modified: Wed, 22 Jun 2022 02:17:49 GMT  
		Size: 54.5 MB (54454366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe27f5f3aa218ad3c5db9387ed88a322a7be45d81c0fcdb8ba15db751eff23`  
		Last Modified: Wed, 22 Jun 2022 02:17:43 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; ppc64le

```console
$ docker pull redmine@sha256:8456be25f6649bd4b065721f238a2cdb39ee6db8297f3ddf6df3740f35e31421
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.5 MB (162488442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:740682f45d82adf76e760685b4f484a52b839f0758ae99f2834b07f0e5b7f0ec`
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
# Tue, 05 Apr 2022 06:08:03 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 20:31:48 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 20:31:50 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 20:34:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 20:34:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 20:34:30 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 20:34:32 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 20:34:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 20:34:40 GMT
CMD ["irb"]
# Wed, 13 Apr 2022 01:33:10 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 13 Apr 2022 01:34:43 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 13 Apr 2022 01:34:50 GMT
ENV RAILS_ENV=production
# Wed, 13 Apr 2022 01:34:52 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Apr 2022 01:34:53 GMT
ENV HOME=/home/redmine
# Wed, 13 Apr 2022 01:34:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 04:33:23 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 04:33:26 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 04:33:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 04:33:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 04:33:48 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 04:37:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 04:38:02 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 04:38:04 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 04:38:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 04:38:08 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 04:38:11 GMT
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
	-	`sha256:635b9cb0e564dc9616ad879e2f36fd919791fb1cf6a9a774891f676f23c60c14`  
		Last Modified: Tue, 12 Apr 2022 21:21:40 GMT  
		Size: 14.4 MB (14418346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2487b6c5fa19ce3779f6e3bfbe796d4f07d6091e86c095ca3fc9ceb55735c5e3`  
		Last Modified: Tue, 12 Apr 2022 21:21:37 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd86fd843216c729218c96eac4efec0302a93ca15c7c82398c1a961d59f23de`  
		Last Modified: Wed, 13 Apr 2022 01:57:49 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a3cd5458f83d83b91ebbdc3f5c0440cf9f84a1ef63b58f25851f3f13d7fd41`  
		Last Modified: Wed, 13 Apr 2022 01:58:05 GMT  
		Size: 82.5 MB (82471882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34802a92813f45622d5604d720c6641558aa719e8fce4e4ed4f9dd7a08c2382`  
		Last Modified: Wed, 13 Apr 2022 01:57:47 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99f38296c787bbd8f10c767ae658a0a7d9b1c4ddc7ec155d62ed69defcf24ccd`  
		Last Modified: Wed, 13 Apr 2022 01:57:47 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184b279ba02201b663696dfb857ea6905224bb519b84074ae28864a72a98bcaf`  
		Last Modified: Wed, 22 Jun 2022 04:41:57 GMT  
		Size: 3.1 MB (3067057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:063884ba2f902b4a7d43f9fe9d64ff4039d9d17515f16dfad1c06eaa5d60a28c`  
		Last Modified: Wed, 22 Jun 2022 04:42:04 GMT  
		Size: 55.9 MB (55915966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9073226d1d784655239f50d6e2150df0544567cfbae1f1744e1e2e8fe969ebf3`  
		Last Modified: Wed, 22 Jun 2022 04:41:56 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine3.15` - linux; s390x

```console
$ docker pull redmine@sha256:6bdb33429a6fa9623e033919368dd076bd7208ee20f6fc98c20e0e9d8fa0f0b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.1 MB (153111566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d26dd62a323d85ede623f718117acb9e0f17ad7787517f98215cf35f1cd8cf`
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
# Tue, 05 Apr 2022 03:21:58 GMT
ENV RUBY_MAJOR=2.7
# Tue, 12 Apr 2022 19:21:03 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 12 Apr 2022 19:21:03 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 12 Apr 2022 19:23:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 12 Apr 2022 19:23:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 12 Apr 2022 19:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 12 Apr 2022 19:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Apr 2022 19:23:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 12 Apr 2022 19:23:47 GMT
CMD ["irb"]
# Wed, 13 Apr 2022 00:44:28 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 13 Apr 2022 00:44:36 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 13 Apr 2022 00:44:40 GMT
ENV RAILS_ENV=production
# Wed, 13 Apr 2022 00:44:40 GMT
WORKDIR /usr/src/redmine
# Wed, 13 Apr 2022 00:44:40 GMT
ENV HOME=/home/redmine
# Wed, 13 Apr 2022 00:44:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 22 Jun 2022 02:19:36 GMT
ENV REDMINE_VERSION=4.2.7
# Wed, 22 Jun 2022 02:19:36 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Wed, 22 Jun 2022 02:19:36 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Wed, 22 Jun 2022 02:19:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 22 Jun 2022 02:19:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 22 Jun 2022 02:21:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 22 Jun 2022 02:21:29 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 22 Jun 2022 02:21:29 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 22 Jun 2022 02:21:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:21:30 GMT
EXPOSE 3000
# Wed, 22 Jun 2022 02:21:30 GMT
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
	-	`sha256:1f9aed4b18e5e5166aa9b402bc4d388bcba04e819df6d16f19c71b755851c305`  
		Last Modified: Tue, 12 Apr 2022 20:04:30 GMT  
		Size: 14.1 MB (14127965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6a4a25dbf31c4557eb3807db4a426dfb42ae16ee0e5bc82fe8edaaef261dd0`  
		Last Modified: Tue, 12 Apr 2022 20:04:28 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b0ff00f01849d710610976014fb18501b3db52513146d25636f7924de199bc`  
		Last Modified: Wed, 13 Apr 2022 00:53:44 GMT  
		Size: 1.2 KB (1222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ac64d852d2b34b9a5e103dc3e9eaba2d50dbce6332b26d9c9b4f9d1cb43c0`  
		Last Modified: Wed, 13 Apr 2022 00:53:53 GMT  
		Size: 74.3 MB (74324099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0353ad3296245f2b7fb1173324723dc414abf520a3cf461ef69d3bd8e280e7b3`  
		Last Modified: Wed, 13 Apr 2022 00:53:42 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938af277c269c3f498a4b7f2e44e951d07a9d2c4b9af27ccc73dc568a2e71ab4`  
		Last Modified: Wed, 13 Apr 2022 00:53:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fbedab992feaa20b62465f86820d1dc125c9c0861a9c0868b61733299a6bf9`  
		Last Modified: Wed, 22 Jun 2022 02:23:46 GMT  
		Size: 3.1 MB (3067051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37604a24bb6547a98867652b8acd18efe1077aa2273d657f1bb7300f73c6abb9`  
		Last Modified: Wed, 22 Jun 2022 02:23:50 GMT  
		Size: 55.2 MB (55242140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7c89a228181999425ae9c5d125843e254a36d81fc4e21a9c5ca46fe02b307f`  
		Last Modified: Wed, 22 Jun 2022 02:23:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
