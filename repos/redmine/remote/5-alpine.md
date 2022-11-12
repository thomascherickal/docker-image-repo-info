## `redmine:5-alpine`

```console
$ docker pull redmine@sha256:1000c9a0c8f914c10e264db94f7bb5e9c167b8155f0944b024370c7170da2afb
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
$ docker pull redmine@sha256:26277e193906e55be2f2cc2de9590d010a5655ee4eaab380608765ee3d83eee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.9 MB (190927539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:777f990b27bdfee6f7703f2fde708179d3fc5794ec1a4dd9396ca72170363007`
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
# Sat, 08 Oct 2022 00:00:18 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 08 Oct 2022 00:00:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 08 Oct 2022 00:00:18 GMT
EXPOSE 3000
# Sat, 08 Oct 2022 00:00:18 GMT
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
	-	`sha256:a82792754087a13f92fa9216103ed65c79bde5cfb9dac79e75ab409616b523ca`  
		Last Modified: Sat, 08 Oct 2022 00:01:49 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:20fd2837f05a04a7b113324162a948c7a01b66b252e2f13a76051bc05e5e3abb
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.7 MB (182738594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ee6069487f90a86eaed70fe30b140156eb310a1be08b53462bea99d49f6167a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:49:36 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Thu, 10 Nov 2022 20:49:36 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 07:13:56 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 11 Nov 2022 07:13:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Nov 2022 07:13:57 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 07:19:35 GMT
ENV RUBY_MAJOR=3.1
# Fri, 11 Nov 2022 07:19:35 GMT
ENV RUBY_VERSION=3.1.2
# Fri, 11 Nov 2022 07:19:35 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Fri, 11 Nov 2022 07:22:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Nov 2022 07:22:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Nov 2022 07:22:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Nov 2022 07:22:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Nov 2022 07:22:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Nov 2022 07:22:08 GMT
CMD ["irb"]
# Fri, 11 Nov 2022 14:19:33 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 11 Nov 2022 14:19:49 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 11 Nov 2022 14:19:49 GMT
ENV RAILS_ENV=production
# Fri, 11 Nov 2022 14:19:49 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Nov 2022 14:19:49 GMT
ENV HOME=/home/redmine
# Fri, 11 Nov 2022 14:19:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Nov 2022 14:19:50 GMT
ENV REDMINE_VERSION=5.0.3
# Fri, 11 Nov 2022 14:19:50 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Fri, 11 Nov 2022 14:19:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Sat, 12 Nov 2022 13:57:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 12 Nov 2022 13:57:09 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 12 Nov 2022 13:59:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 12 Nov 2022 13:59:15 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 12 Nov 2022 13:59:15 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 12 Nov 2022 13:59:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Nov 2022 13:59:15 GMT
EXPOSE 3000
# Sat, 12 Nov 2022 13:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ac08bea1cd73617035de26493564e5c6eb6da521f8a11e4e594b7edf4ea9f4`  
		Last Modified: Fri, 11 Nov 2022 07:34:30 GMT  
		Size: 3.4 MB (3445404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d8a81935b84cc00f34e62fa00ffdd506287e97ddc8ca3d7ec475e4b0beabe4`  
		Last Modified: Fri, 11 Nov 2022 07:34:30 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53cd7ff7a7493ceb448cc2e5377b858c15022d5506dec07fe1b76a2666f8cac`  
		Last Modified: Fri, 11 Nov 2022 07:35:24 GMT  
		Size: 29.4 MB (29369560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a03c4f456c43293a73969e869bfc1649ea74141730866fcecf8a639b5eed4e`  
		Last Modified: Fri, 11 Nov 2022 07:35:20 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b098a6a75b5809b2b54cfa9065ee40c7b41b1b7246a9aed4ce72084f74f2d2`  
		Last Modified: Sat, 12 Nov 2022 14:02:57 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3794fc5a60368d5b5a96b5e054ae031aefa54beeb90d50cd3c24d5c487b962`  
		Last Modified: Sat, 12 Nov 2022 14:03:12 GMT  
		Size: 78.5 MB (78459551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f4ff552d87501709f96a486b82b837daa665f07c2c426da1e176a7df0a3eb1`  
		Last Modified: Sat, 12 Nov 2022 14:02:55 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77e00293c6b72c2a68893f996ab4786e1e85c6571d3aca0ba97b053a2a41539`  
		Last Modified: Sat, 12 Nov 2022 14:02:55 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665df8c1b50335dca2c268b943da44b5ffb629b822d4ea129165de0ec043c86c`  
		Last Modified: Sat, 12 Nov 2022 14:02:56 GMT  
		Size: 3.1 MB (3142302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a65716ab7b672c4a6bb98beb6b30dccf33dfb1490aba99ff6a0cb8c13f615f0`  
		Last Modified: Sat, 12 Nov 2022 14:03:04 GMT  
		Size: 65.7 MB (65686819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aa89712471b0bd7d2036284ed7ff93a59dadc30678c9936d727aa132fd4f45`  
		Last Modified: Sat, 12 Nov 2022 14:02:55 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:aee58d95e1647258b94f304781a2da5ed0e1a5c9a28bfe5118e50e0c5c3124ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **177.3 MB (177310899 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c01a4b46aff308dd3a542f6b10623489a9e3c1bff86a6862521fbd2dab23cb5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Wed, 26 Oct 2022 08:31:42 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 26 Oct 2022 08:31:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 26 Oct 2022 08:31:43 GMT
ENV LANG=C.UTF-8
# Wed, 26 Oct 2022 08:46:09 GMT
ENV RUBY_MAJOR=3.1
# Wed, 26 Oct 2022 08:46:09 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 26 Oct 2022 08:46:09 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 26 Oct 2022 08:48:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 26 Oct 2022 08:48:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 26 Oct 2022 08:48:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 26 Oct 2022 08:48:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Oct 2022 08:48:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 26 Oct 2022 08:48:26 GMT
CMD ["irb"]
# Thu, 27 Oct 2022 05:56:41 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 27 Oct 2022 05:56:54 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 27 Oct 2022 05:56:54 GMT
ENV RAILS_ENV=production
# Thu, 27 Oct 2022 05:56:54 GMT
WORKDIR /usr/src/redmine
# Thu, 27 Oct 2022 05:56:54 GMT
ENV HOME=/home/redmine
# Thu, 27 Oct 2022 05:56:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 27 Oct 2022 05:56:55 GMT
ENV REDMINE_VERSION=5.0.3
# Thu, 27 Oct 2022 05:56:55 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Thu, 27 Oct 2022 05:56:55 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Thu, 27 Oct 2022 05:56:59 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 27 Oct 2022 05:56:59 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 27 Oct 2022 05:58:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 27 Oct 2022 05:58:57 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 27 Oct 2022 05:58:57 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 27 Oct 2022 05:58:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 27 Oct 2022 05:58:58 GMT
EXPOSE 3000
# Thu, 27 Oct 2022 05:58:58 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462f62b2a71d21d0e17ff6ec19ae37ef51268d87770f8c2e72df3be5a8469842`  
		Last Modified: Wed, 26 Oct 2022 09:19:19 GMT  
		Size: 3.3 MB (3313571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00da6451aa7023231c19f82ebbd28716035814ccc058e01730afae7870bf007`  
		Last Modified: Wed, 26 Oct 2022 09:19:18 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02523d138b446e454400512f14de7073184d64b7697c438a5d9e48e000e302f3`  
		Last Modified: Wed, 26 Oct 2022 09:22:13 GMT  
		Size: 28.0 MB (28035060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378d1a7b3a5618c6e0b70d8a5981942af7289250708d55e903d6a3c09c59fbc4`  
		Last Modified: Wed, 26 Oct 2022 09:22:10 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b500e618894968429e41bcaec62a21fbb05495bb8b93122e823b4e7ac0da2c4`  
		Last Modified: Thu, 27 Oct 2022 06:07:08 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5530386881158454c557bb5eabfc6efd0733e6f1cd66e0a141a38afdaf51ed6`  
		Last Modified: Thu, 27 Oct 2022 06:07:21 GMT  
		Size: 75.0 MB (75003278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7781150ec1d515f1e48c13bd5c1120cec2b1a2f797f801f42e1e73aa9c78843`  
		Last Modified: Thu, 27 Oct 2022 06:07:05 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fff7b545d7e05c47d38e9de847af0563744724634349dd3baa3b08ce30fb9d7`  
		Last Modified: Thu, 27 Oct 2022 06:07:06 GMT  
		Size: 129.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22f81e43cac94c67633678a582a17dc7f60c59fa5f0f4ce866d7d9f8f00c9bf7`  
		Last Modified: Thu, 27 Oct 2022 06:07:06 GMT  
		Size: 3.1 MB (3142348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63d265865b6e6a3af8caa171867c0b3ae887490294e89fa671119e76998663e7`  
		Last Modified: Thu, 27 Oct 2022 06:07:14 GMT  
		Size: 65.4 MB (65377717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8022a783a24842e6741fbaf67a35c3707f75bd9a1e5b48e9b2edab3b52805a1`  
		Last Modified: Thu, 27 Oct 2022 06:07:05 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:dd52fc3c1bdce3fc1b2eace275bf39f0f53152b6c3bddb258d22e4493460662f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.1 MB (187062479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75d12aecb3f6e337546d0713282257555371e43a3f6633b39e7ca986bab9537f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 10 Nov 2022 20:39:46 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Thu, 10 Nov 2022 20:39:46 GMT
CMD ["/bin/sh"]
# Fri, 11 Nov 2022 05:05:02 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Fri, 11 Nov 2022 05:05:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Nov 2022 05:05:02 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 05:08:56 GMT
ENV RUBY_MAJOR=3.1
# Fri, 11 Nov 2022 05:08:56 GMT
ENV RUBY_VERSION=3.1.2
# Fri, 11 Nov 2022 05:08:56 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Fri, 11 Nov 2022 05:10:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Nov 2022 05:10:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Nov 2022 05:10:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Nov 2022 05:10:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Nov 2022 05:10:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Nov 2022 05:10:35 GMT
CMD ["irb"]
# Fri, 11 Nov 2022 12:23:50 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 11 Nov 2022 12:23:59 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 11 Nov 2022 12:24:00 GMT
ENV RAILS_ENV=production
# Fri, 11 Nov 2022 12:24:00 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Nov 2022 12:24:00 GMT
ENV HOME=/home/redmine
# Fri, 11 Nov 2022 12:24:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Nov 2022 12:24:01 GMT
ENV REDMINE_VERSION=5.0.3
# Fri, 11 Nov 2022 12:24:01 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Fri, 11 Nov 2022 12:24:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Sat, 12 Nov 2022 11:47:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 12 Nov 2022 11:47:28 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 12 Nov 2022 11:48:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 12 Nov 2022 11:48:59 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 12 Nov 2022 11:48:59 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 12 Nov 2022 11:48:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Nov 2022 11:48:59 GMT
EXPOSE 3000
# Sat, 12 Nov 2022 11:48:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4060ed78b9b77bc4928b3dd92b2d1f30c9bc40efec34f001751cbcff3c06a24`  
		Last Modified: Fri, 11 Nov 2022 05:19:14 GMT  
		Size: 3.7 MB (3659135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e18e33ab217eb01f18a43bcd22110c623c9332d4fbddc8694d9c6a14abd7621`  
		Last Modified: Fri, 11 Nov 2022 05:19:13 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac20065ca8ba32d86f5676eb9b268c93389a3793246ffee37d5fb4374b093421`  
		Last Modified: Fri, 11 Nov 2022 05:20:00 GMT  
		Size: 30.2 MB (30247404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8df68a92c1143de3a828d54997e2cccc153dfe11f22080cc8bacc5e0b0182b3`  
		Last Modified: Fri, 11 Nov 2022 05:19:58 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b37176abc7ef2e900dc71711a4de13314cf3a67a79400c8d87479e26d061b8d6`  
		Last Modified: Sat, 12 Nov 2022 11:51:46 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878a3e82db63f96259ed1828838eb423153c2cf02c1eab8e4475fe4f13ee656c`  
		Last Modified: Sat, 12 Nov 2022 11:51:56 GMT  
		Size: 80.2 MB (80246371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a399a1336e11c5dd85d1ad30408b991c881f545faba4e6e28b83aba405b53f5`  
		Last Modified: Sat, 12 Nov 2022 11:51:43 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b0e3fdce5fbe5bc9572f1fb672e4ae9fc5ee50cdca9285189a23e05dfa5f00`  
		Last Modified: Sat, 12 Nov 2022 11:51:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af2332fddf31bc837222eb973dd768db6849bdc8147064f969c822d94250d5d`  
		Last Modified: Sat, 12 Nov 2022 11:51:44 GMT  
		Size: 3.1 MB (3142547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593c09f5c06b869248011587129e9abc38e721eeefc9c3fb9f8f699227c60514`  
		Last Modified: Sat, 12 Nov 2022 11:51:50 GMT  
		Size: 67.0 MB (67044632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20c090f6977679c7450d2b06cd8114272a3fa54132f796ef01ac33a3ed433ff`  
		Last Modified: Sat, 12 Nov 2022 11:51:43 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; 386

```console
$ docker pull redmine@sha256:39c3d9d9d0bed28864f985f5d5949e28cc288a34c473b3d37ee2e830b6bee4d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.6 MB (189625586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c6e56b9da855a85169a2fac51ee0e6a650c412e3484b80f4d4e49c7022df6f`
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
# Sat, 08 Oct 2022 00:39:59 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 08 Oct 2022 00:40:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 08 Oct 2022 00:40:00 GMT
EXPOSE 3000
# Sat, 08 Oct 2022 00:40:01 GMT
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
	-	`sha256:d1a3be5cabf8966f9e3a6d072c7c323ccbd02e585a48dedb7983304ce19173b5`  
		Last Modified: Sat, 08 Oct 2022 00:42:01 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; ppc64le

```console
$ docker pull redmine@sha256:73a387fc0e89498cd99798b6e0941ced028e5da6e0123ea203cbdfb50d15dbcc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.7 MB (191661930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e541c1a239181222d3d70c1d0971f8ccd2fe406c3e2fba1ed076e1e4029b644`
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
# Fri, 07 Oct 2022 07:14:47 GMT
ENV RUBY_MAJOR=3.1
# Fri, 07 Oct 2022 07:14:47 GMT
ENV RUBY_VERSION=3.1.2
# Fri, 07 Oct 2022 07:14:47 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Fri, 07 Oct 2022 07:17:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 07:18:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 07:18:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 07:18:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 07:18:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 07:18:03 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 11:44:37 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 11:45:09 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 11:45:13 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 11:45:13 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 11:45:14 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 11:45:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 11:45:15 GMT
ENV REDMINE_VERSION=5.0.3
# Fri, 07 Oct 2022 11:45:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Fri, 07 Oct 2022 11:45:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Fri, 07 Oct 2022 11:45:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 11:45:21 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 11:49:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 11:49:16 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 07 Oct 2022 23:53:02 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Fri, 07 Oct 2022 23:53:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 07 Oct 2022 23:53:03 GMT
EXPOSE 3000
# Fri, 07 Oct 2022 23:53:03 GMT
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
	-	`sha256:a195f2d9f186ad8c041e55f4c07f2b5343f8473b4fce1cac8d591f324c3ae16b`  
		Last Modified: Fri, 07 Oct 2022 07:34:41 GMT  
		Size: 29.6 MB (29578746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbe3fc3b4fbf36bbe7411c3dcb24374bd3ffde82f5d86916c448934189a7ef0`  
		Last Modified: Fri, 07 Oct 2022 07:34:36 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5eafe2d14c207c8533e3b0ce8f30a9fb12b9cd43499fe55389589a6e0b47d40`  
		Last Modified: Fri, 07 Oct 2022 11:56:08 GMT  
		Size: 1.2 KB (1220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7817f306fe61700f25ccd8ace84ae154bfaeb0c4703212c58bfd56d63094eb8`  
		Last Modified: Fri, 07 Oct 2022 11:56:30 GMT  
		Size: 83.3 MB (83259708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff13c8f28d427662d4dab2b3eeb913994df76727bb8425ad7ec8c9c5ebd51e25`  
		Last Modified: Fri, 07 Oct 2022 11:56:06 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460131a7b5299ca4737324862729f1fe8a613f6a37821e978204ff921a2c3fa7`  
		Last Modified: Fri, 07 Oct 2022 11:56:06 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86454b49cf587ed53d735a373c4ab45aabc3ac4256bc0862da83e81cab2a6b16`  
		Last Modified: Fri, 07 Oct 2022 11:56:07 GMT  
		Size: 3.1 MB (3142565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3171cde0495f9336a8cb2ac79f2e4c0d29aa875534ae484a1ea4ac24b792ca0d`  
		Last Modified: Fri, 07 Oct 2022 11:56:18 GMT  
		Size: 69.1 MB (69052107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d2f6359b134a7930d7b83f48405608c8c118f26d264cfb5373ac1a7b4c11eb`  
		Last Modified: Fri, 07 Oct 2022 23:55:06 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-alpine` - linux; s390x

```console
$ docker pull redmine@sha256:1d6d10dc8a0d1d893ccf66ccfb9cf8274b93e41497ffc39f393243fb4b209b7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.0 MB (182993328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfa88a9f9b98bad0c5f2d6ef2af62c1628bc2aa82e277fef8a91f165224d61e4`
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
# Fri, 07 Oct 2022 09:34:45 GMT
ENV RUBY_MAJOR=3.1
# Fri, 07 Oct 2022 09:34:45 GMT
ENV RUBY_VERSION=3.1.2
# Fri, 07 Oct 2022 09:34:45 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Fri, 07 Oct 2022 09:37:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 07 Oct 2022 09:37:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 07 Oct 2022 09:37:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 07 Oct 2022 09:37:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Oct 2022 09:37:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 07 Oct 2022 09:37:57 GMT
CMD ["irb"]
# Fri, 07 Oct 2022 13:02:51 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 07 Oct 2022 13:03:19 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 07 Oct 2022 13:03:33 GMT
ENV RAILS_ENV=production
# Fri, 07 Oct 2022 13:03:33 GMT
WORKDIR /usr/src/redmine
# Fri, 07 Oct 2022 13:03:33 GMT
ENV HOME=/home/redmine
# Fri, 07 Oct 2022 13:03:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 07 Oct 2022 13:03:35 GMT
ENV REDMINE_VERSION=5.0.3
# Fri, 07 Oct 2022 13:03:36 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.3.tar.gz
# Fri, 07 Oct 2022 13:03:36 GMT
ENV REDMINE_DOWNLOAD_SHA256=594068014b2c5eceb3510bfd8786b8d7bc837896912a95cbb24dd76941d36ca0
# Fri, 07 Oct 2022 13:03:42 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 07 Oct 2022 13:03:44 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 07 Oct 2022 13:05:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 13:05:46 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 08 Oct 2022 00:29:43 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Sat, 08 Oct 2022 00:29:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 08 Oct 2022 00:29:43 GMT
EXPOSE 3000
# Sat, 08 Oct 2022 00:29:44 GMT
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
	-	`sha256:0baf485a97a84f73f2a4ea8ef50804e048341138cdd402da7ad65466132e908e`  
		Last Modified: Fri, 07 Oct 2022 09:54:03 GMT  
		Size: 29.4 MB (29366426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d3665d09514c5b9d04ecb4735b9a8fcd05e373007003aa6e71a7e4760dbe9f8`  
		Last Modified: Fri, 07 Oct 2022 09:54:00 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359d021ce9b9541f0e092658daa28642b8da264d433ef0a9f3ee24dc5f063535`  
		Last Modified: Fri, 07 Oct 2022 13:09:57 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0893e1a922757eb53c59fdac8bc5a144be7e26bb49c45b22fb695cd52eb991ad`  
		Last Modified: Fri, 07 Oct 2022 13:10:06 GMT  
		Size: 75.1 MB (75115408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f33db6325ed72c12f7e5581b95b20f1b95b2bec93990fdb6e759e763d36ce5c`  
		Last Modified: Fri, 07 Oct 2022 13:09:56 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684e949a041f20ee5d26ce342a5be4ebb05db691f27fdf43f3b02e52732c182`  
		Last Modified: Fri, 07 Oct 2022 13:09:56 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70fd0b6948d10874fded1cdf8e8a4de70b97bcbf425ca64b52d89829e641f053`  
		Last Modified: Fri, 07 Oct 2022 13:09:56 GMT  
		Size: 3.1 MB (3142557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a75aeacf1dfafab9b460bb9fd00cd29be48c9d56d14d524250030645dc52de6`  
		Last Modified: Fri, 07 Oct 2022 13:10:02 GMT  
		Size: 69.0 MB (69000314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df335e5dd6b1d32627e8d4857066e1d9b921f47f888c3ea1945369fcb3d1a49`  
		Last Modified: Sat, 08 Oct 2022 00:31:27 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
