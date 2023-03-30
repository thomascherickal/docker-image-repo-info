## `redmine:alpine3.16`

```console
$ docker pull redmine@sha256:19c299be30e1e20bba04a308f7329f2aa64ab106224a01a1f3f050bf6ff2fcfd
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

### `redmine:alpine3.16` - linux; amd64

```console
$ docker pull redmine@sha256:51e5c0fd528c35fccb0040688b5a6c3cd3962a6316c2437c8d07ec240750c019
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.8 MB (199805812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9a40a6ff3322acf02088daf6b8f85ce1c5b2a1d874f51451956964b6f383979`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 02:21:43 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 30 Mar 2023 02:21:44 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 30 Mar 2023 02:21:44 GMT
ENV LANG=C.UTF-8
# Thu, 30 Mar 2023 02:27:19 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 02:27:19 GMT
ENV RUBY_VERSION=3.1.3
# Thu, 30 Mar 2023 02:27:19 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Thu, 30 Mar 2023 02:29:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 02:29:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 02:29:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 02:29:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 02:29:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 02:29:50 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 05:30:35 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 05:30:43 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 05:30:43 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 05:30:43 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 05:30:43 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 05:30:44 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 05:30:44 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 05:30:44 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 05:30:44 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 05:30:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 05:30:48 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 05:32:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 05:32:39 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 05:32:39 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 05:32:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 05:32:39 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 05:32:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52a5fbef9a7ca13abdb787ccddf6fb7d2ecad991b7d37fb776cd6d717b4e3d7`  
		Last Modified: Thu, 30 Mar 2023 02:35:25 GMT  
		Size: 3.9 MB (3851499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669ebe35e8508ac4a673ebf6ad67a95e27550896cb835fdd7a80cd80d9c0dc98`  
		Last Modified: Thu, 30 Mar 2023 02:35:24 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907c2de1783d2990dfd73ce2f8b55402a3d170543cfdee6eebba3adb1f9a9717`  
		Last Modified: Thu, 30 Mar 2023 02:35:57 GMT  
		Size: 29.3 MB (29318861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cc4135fcf909fc8f745a43448c7525879acfdeae8b2afa458d9d00ff760a8f`  
		Last Modified: Thu, 30 Mar 2023 02:35:55 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c2b07cda20f9dfb755d64ebd6f0f46c0e026031adcb672d7b9bde357036336`  
		Last Modified: Thu, 30 Mar 2023 05:35:41 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6710890fd6dd5563f60777bfbb7fc5c9fd1b6986bd4c36ed0f2738be68bf05`  
		Last Modified: Thu, 30 Mar 2023 05:35:53 GMT  
		Size: 90.4 MB (90427458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c70afda3cfdaad3f745f62233164d42022417cac57ba16f14843aa95ad931e2`  
		Last Modified: Thu, 30 Mar 2023 05:35:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07fc8d79473bf06a4cb4834eb31acc7bc2ac80704f4e6e4a61e39d7875b9919`  
		Last Modified: Thu, 30 Mar 2023 05:35:39 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902761c8dada1e0deb60f7926b59b6ba389b35b912c8518be23cdf0676be564c`  
		Last Modified: Thu, 30 Mar 2023 05:35:40 GMT  
		Size: 3.1 MB (3145994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de16203b6473756473886aa23a391f17f61cd1aac03e6dba80dbfdf5e7a2a8e`  
		Last Modified: Thu, 30 Mar 2023 05:35:45 GMT  
		Size: 70.3 MB (70250260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f597dffe1da40feafd9fdaf6e056d0b7d93af98d01a11c483f94854a311da45f`  
		Last Modified: Thu, 30 Mar 2023 05:35:39 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.16` - linux; arm variant v6

```console
$ docker pull redmine@sha256:a49702b0c3b15ba574ea612ed106890be06b97ac8bdb67222886a62d90190ec5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190089099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:288bb00f34a6206b3e5b023a892d988b55015009ef50a8abd31f89011c6000fe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:06:08 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 30 Mar 2023 00:06:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 30 Mar 2023 00:06:09 GMT
ENV LANG=C.UTF-8
# Thu, 30 Mar 2023 00:11:55 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 00:11:56 GMT
ENV RUBY_VERSION=3.1.3
# Thu, 30 Mar 2023 00:11:56 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Thu, 30 Mar 2023 00:13:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 00:13:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 00:13:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 00:13:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 00:14:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 00:14:00 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 01:16:07 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 01:16:18 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 01:16:19 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 01:16:19 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 01:16:20 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 01:16:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 01:16:20 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 01:16:20 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 01:16:20 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 01:16:24 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 01:16:24 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 01:18:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 01:18:19 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 01:18:19 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 01:18:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 01:18:19 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 01:18:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed94e4dc9ea9eca127e40e4b6b16da2ee175dde29c138fd7a8d5aedf32cf9e29`  
		Last Modified: Thu, 30 Mar 2023 00:20:59 GMT  
		Size: 3.6 MB (3593942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ac9bc6481f90a813d3da1de98c8b35d31e37a7f6e65d3d6bacc4996817175c`  
		Last Modified: Thu, 30 Mar 2023 00:20:58 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18664e7a42bb9465022f22c826da067ff6c86cc8fd81214b168886a9cd7f19ab`  
		Last Modified: Thu, 30 Mar 2023 00:21:32 GMT  
		Size: 28.3 MB (28266907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faea03c94ec3c9db6688e887648e5468bf29c265aca44a751e4233a2d7afe502`  
		Last Modified: Thu, 30 Mar 2023 00:21:29 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283799482d3a6ca7099a0f131f2a990c1dd0c3256b03aef52969e391ed24b1ba`  
		Last Modified: Thu, 30 Mar 2023 01:24:38 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de90a59315219ce281c568521cdedc5d4670bc356b7d5eeb3511517dceaccb0f`  
		Last Modified: Thu, 30 Mar 2023 01:24:51 GMT  
		Size: 83.9 MB (83937157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4589000873d3c5af8585677724d2c6bb3ea5aae9dac4c43106dafe41194797bf`  
		Last Modified: Thu, 30 Mar 2023 01:24:36 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb08418710362f7e92020b6faada9fdeef6d5a6d18c35e1ce4795fe42e0b2e0`  
		Last Modified: Thu, 30 Mar 2023 01:24:35 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:288a44e1c83b2bb974f3fe94c8819cdfd4a3c709339db96d94a085d8083a909d`  
		Last Modified: Thu, 30 Mar 2023 01:24:37 GMT  
		Size: 3.1 MB (3145759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe57441553d9c35cc29c5ce527e9a917f61e0b0d04af0ce574a0acbb065f4eb6`  
		Last Modified: Thu, 30 Mar 2023 01:24:43 GMT  
		Size: 68.5 MB (68524556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c619112d438605ae8dc8f8c400a07f35e47590b046af2960f912adb540353f`  
		Last Modified: Thu, 30 Mar 2023 01:24:36 GMT  
		Size: 2.0 KB (2011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.16` - linux; arm variant v7

```console
$ docker pull redmine@sha256:4d33c1f927231ac31eacbbfbb78d400750d3874c442a4d3aa0f098eeadccc710
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187363650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51b1fcbbe4305fef0deb17f67816944f0e66d1a21b8235d02a7e2242117f4a58`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:37:23 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 30 Mar 2023 05:37:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 30 Mar 2023 05:37:23 GMT
ENV LANG=C.UTF-8
# Thu, 30 Mar 2023 05:44:38 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 05:44:38 GMT
ENV RUBY_VERSION=3.1.3
# Thu, 30 Mar 2023 05:44:38 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Thu, 30 Mar 2023 05:46:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 05:46:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 05:46:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 05:46:38 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 05:46:39 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 05:46:39 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 06:47:12 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 06:47:22 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 06:47:23 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 06:47:23 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 06:47:23 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 06:47:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 06:47:24 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 06:47:24 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 06:47:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 06:47:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 06:47:28 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 06:49:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 06:49:23 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 06:49:23 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 06:49:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 06:49:23 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 06:49:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0e2bb5f86e6c76ffc574535478b37638416b94d7f6a24f27d26c3602b3c1b2d`  
		Last Modified: Thu, 30 Mar 2023 05:53:04 GMT  
		Size: 3.5 MB (3461614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a72eed43cd068815244c3f42447a9d10d3d14af8cfc72145b264b40c4eabf39`  
		Last Modified: Thu, 30 Mar 2023 05:53:03 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee2a2b3137bf39ff53abe11d77d39649e90dbec90d2b050fe821d213df46a40c`  
		Last Modified: Thu, 30 Mar 2023 05:53:38 GMT  
		Size: 28.1 MB (28145450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1966ffb908ce1ceccfa5fd6f080f3a8bea2099ca1468ec655bf54c2d2236bd7e`  
		Last Modified: Thu, 30 Mar 2023 05:53:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead48fd5ff444cc311e7a741ade7af93a86c2731588035ae18654bc57a5af418`  
		Last Modified: Thu, 30 Mar 2023 06:53:07 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bec813a9d08d362cb7eea8260f91dd0a6011966337512de6cddb2eb47740f7`  
		Last Modified: Thu, 30 Mar 2023 06:53:19 GMT  
		Size: 82.1 MB (82058842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c667e9849aaf33b8f0bff5e7e92d8d78eec5142f7f298b8dcd6ea5ed26ae010e`  
		Last Modified: Thu, 30 Mar 2023 06:53:05 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208f68e658464600811d90f6a9b0aff87f5637b0dca1fc4b629a928f9d833606`  
		Last Modified: Thu, 30 Mar 2023 06:53:05 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb09813b88bc462fcca413aed3fafeac7f9d761d40af84d8590ea6d393a074c8`  
		Last Modified: Thu, 30 Mar 2023 06:53:06 GMT  
		Size: 3.1 MB (3145984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c90eaa326d1a1238258dd639a3324ecbffd19a2047e93221f332375661b599`  
		Last Modified: Thu, 30 Mar 2023 06:53:13 GMT  
		Size: 68.1 MB (68127277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfc4025f0b6fc1379891a92ace742c174680d851accae432e8c4f34845b0b2a`  
		Last Modified: Thu, 30 Mar 2023 06:53:05 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.16` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:5bcb0738e733bd956ce2f9717eb5b789ae269243e8bbf4e338f191f7a5fabae4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.6 MB (195562070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b848c0b3c85bbb1ff9c2436f7f7fcd782ab246ea742aee049571eb2d060d13d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:31:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 30 Mar 2023 05:31:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 30 Mar 2023 05:31:58 GMT
ENV LANG=C.UTF-8
# Thu, 30 Mar 2023 05:36:00 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 05:36:00 GMT
ENV RUBY_VERSION=3.1.3
# Thu, 30 Mar 2023 05:36:00 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Thu, 30 Mar 2023 05:37:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 05:37:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 05:37:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 05:37:44 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 05:37:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 05:37:45 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 07:49:30 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 07:49:36 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 07:49:37 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 07:49:37 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 07:49:37 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 07:49:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 07:49:38 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 07:49:38 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 07:49:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 07:49:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 07:49:41 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 07:51:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 07:51:17 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 07:51:17 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 07:51:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 07:51:18 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 07:51:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1a9490257ae7ef0e0bc1c83706c2438d863108df9a74d33ad1f5104d50de88`  
		Last Modified: Thu, 30 Mar 2023 05:42:27 GMT  
		Size: 3.8 MB (3821415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12c93e378d0ceba3619afba2196ca86017a31284505e76b9d15780ac1c1d790`  
		Last Modified: Thu, 30 Mar 2023 05:42:26 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855e294d1ab93efbe4088adc899105d8b803a6f3c679d84699632de4b79ab00b`  
		Last Modified: Thu, 30 Mar 2023 05:42:57 GMT  
		Size: 28.7 MB (28704287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b29e49395e1bbc514c8a0c7553264daaba6d04fa23366240a9724e08b048d6`  
		Last Modified: Thu, 30 Mar 2023 05:42:55 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39c6da132a66a9edc83a85fe5a34495719e884a4c1aa2185da962143f84ddf9`  
		Last Modified: Thu, 30 Mar 2023 07:54:00 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc9e73e9006d938322b5569861625170bd55511d912ce39e0c5628d53ce6dc1`  
		Last Modified: Thu, 30 Mar 2023 07:54:09 GMT  
		Size: 87.3 MB (87292431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15645d28d375378bc290b4511b3f90216cb117091574935ca27f8ff0b893ef8e`  
		Last Modified: Thu, 30 Mar 2023 07:53:58 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af902591a9c38ae0dfecff68ea5189d2c1f6382619418f7c3060cf175913e58`  
		Last Modified: Thu, 30 Mar 2023 07:53:58 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfb6e9d986c3b40299d2939043d05766fc0e54671327b987d9c2e7751b7d6d8`  
		Last Modified: Thu, 30 Mar 2023 07:53:59 GMT  
		Size: 3.1 MB (3146030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b3d23648974e7df5b0ab23c92bc7da1669b1761db00d3538bbdb05f0ada1928`  
		Last Modified: Thu, 30 Mar 2023 07:54:04 GMT  
		Size: 69.9 MB (69884627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a231654c1cee66e6a63fb360bfed6ea42a4ddc0f8a5efd83be3b0ac635d05c5`  
		Last Modified: Thu, 30 Mar 2023 07:53:58 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.16` - linux; 386

```console
$ docker pull redmine@sha256:fb52fd2ec5bc21196292b5ed915a9aa0cc2170f5fa4cdb4f4acdfd2f21b79373
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.1 MB (197095220 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bda5e8e085d2e60efe238007883b0588bfe9eecb6b2149c69b1a6ddc0ce375c3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:33 GMT
ADD file:c9d37b1a7eee54b1a8c1ebde284829510ec289f7b7db2c16059b26f01b416fe0 in / 
# Wed, 29 Mar 2023 17:38:33 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:09:33 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 30 Mar 2023 01:09:34 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 30 Mar 2023 01:09:34 GMT
ENV LANG=C.UTF-8
# Thu, 30 Mar 2023 01:18:05 GMT
ENV RUBY_MAJOR=3.1
# Thu, 30 Mar 2023 01:18:06 GMT
ENV RUBY_VERSION=3.1.3
# Thu, 30 Mar 2023 01:18:06 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Thu, 30 Mar 2023 01:22:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 01:22:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 01:22:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 01:22:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 01:22:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 01:22:36 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 03:39:02 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 03:39:12 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 03:39:14 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 03:39:14 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 03:39:14 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 03:39:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 03:39:15 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 03:39:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 03:39:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 03:39:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 03:39:22 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 03:41:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 03:41:56 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 03:41:57 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 03:41:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:41:57 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 03:41:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dea45757091f21722aec41fb20845e57a04f4bb8c199531491f1dc070480a574`  
		Last Modified: Wed, 29 Mar 2023 17:39:11 GMT  
		Size: 2.8 MB (2810814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec757ac8272e11b5833accc88f85293f1b7b49ba1bdb61dde9025bc0f725cc25`  
		Last Modified: Thu, 30 Mar 2023 01:31:40 GMT  
		Size: 3.9 MB (3886676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3736da23bde1b795da95fc3c284ab996b92cf770d252551bedf5b63943f8483b`  
		Last Modified: Thu, 30 Mar 2023 01:31:39 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:659a304669c274bf38fb39f6f6786173cac9b27b7ee203585b87887d332f8e57`  
		Last Modified: Thu, 30 Mar 2023 01:32:17 GMT  
		Size: 28.1 MB (28119338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e75dea3c4e82af45bfb400bcc38dd5498638890058613923712268e93341d36`  
		Last Modified: Thu, 30 Mar 2023 01:32:13 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728fdfae8d7e60f69ee4ad43174ae35e983aa036327a2e5dec79234e5022c722`  
		Last Modified: Thu, 30 Mar 2023 03:45:34 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acab8ff082dfbbf91989f20121a8049284c629c12df45dbabc97fadb26057617`  
		Last Modified: Thu, 30 Mar 2023 03:45:53 GMT  
		Size: 90.3 MB (90301206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4e3f486ad787b516f13fea6ac0d44a05b4c826b7e9789aa3004132560d70e7`  
		Last Modified: Thu, 30 Mar 2023 03:45:32 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ced829d6eb1f109a759135cd9fd2f25e202ffb3a1b7e348374d52e8f94a734`  
		Last Modified: Thu, 30 Mar 2023 03:45:32 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90b1b186db01c479ed8b86b6bbb5ce50d8b3d743d793c1dc647e2fd7ccd6ba2c`  
		Last Modified: Thu, 30 Mar 2023 03:45:33 GMT  
		Size: 3.1 MB (3145814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882403fbdc755176d2c2b097ce687136259e1cfb9f31567b183cd07af8ddaa1f`  
		Last Modified: Thu, 30 Mar 2023 03:45:42 GMT  
		Size: 68.8 MB (68827434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01cdc9e3db620991df944f8577314b42ba9acbef489b601a030d0df70f84c546`  
		Last Modified: Thu, 30 Mar 2023 03:45:32 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.16` - linux; ppc64le

```console
$ docker pull redmine@sha256:c9b09f2f925bbe715b02145fba4771a2cc3912f640ed21f274f1e4b22a2da850
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.8 MB (206808343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f032a77a43e53a7f2e6a6c2bdb8713acd30b6a911b7f6394303128c8f5af3e07`
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
# Thu, 30 Mar 2023 04:18:15 GMT
ENV RUBY_VERSION=3.1.3
# Thu, 30 Mar 2023 04:18:15 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Thu, 30 Mar 2023 04:21:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 04:21:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 04:21:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 04:21:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 04:21:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 04:21:56 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 08:16:14 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 08:16:34 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 08:16:38 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 08:16:38 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 08:16:38 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 08:16:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 08:16:40 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 08:16:40 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 08:16:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 08:16:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 08:16:47 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 08:20:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 08:20:45 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 08:20:45 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 08:20:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 08:20:46 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 08:20:46 GMT
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
	-	`sha256:73e0931d5464bd5ee9bd6c8b585cb43f396bc57495f2cbd37fa17c69a0f2e72b`  
		Last Modified: Thu, 30 Mar 2023 04:31:25 GMT  
		Size: 29.5 MB (29517738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec950bd82fef0915e2f4c3ece39affb96c80bd10bc9f1a21951cd1f2b5118a3`  
		Last Modified: Thu, 30 Mar 2023 04:31:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b42164a2bf6620d8410486c39c5657a8c098844b33216b6c2917ca1be0dc6b3`  
		Last Modified: Thu, 30 Mar 2023 08:26:39 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88affceacdc77462125b09a9b6c70559e049bbd448410c228744683c3878c6c6`  
		Last Modified: Thu, 30 Mar 2023 08:27:03 GMT  
		Size: 96.3 MB (96318235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a064b7bbf7ffaff7acf137e2eb56a744522755ac7f41ebe25c864202eb9e2a`  
		Last Modified: Thu, 30 Mar 2023 08:26:37 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc9a8abfbc5dd8e0ef1e6007d3f16a7656aec57558d64a65269aa5deb1974b4`  
		Last Modified: Thu, 30 Mar 2023 08:26:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fff16926d096f5c6337ccad40b30adee16c08705f3e92e8051f7e21221f4bc4`  
		Last Modified: Thu, 30 Mar 2023 08:26:38 GMT  
		Size: 3.1 MB (3146087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86357f8ab5fe80f033fa0a4b66b80d0aba8214cde5c558f971b4730e03c63154`  
		Last Modified: Thu, 30 Mar 2023 08:26:49 GMT  
		Size: 71.0 MB (71044015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4061b6cf522e7c9ebf072222e2384bbf40f58a78845b7b04df69394bfdd99e23`  
		Last Modified: Thu, 30 Mar 2023 08:26:37 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine3.16` - linux; s390x

```console
$ docker pull redmine@sha256:fdcee821771c813fe6f4393445a1e577eca5d32d17a2069409fc6f241519f74a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.9 MB (189932088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e876a013fb36c7d4f4edccbb1c94ab5ecb1ea6e2ebc0335fe64a39b43a912c18`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:18:04 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 29 Mar 2023 22:18:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 29 Mar 2023 22:18:07 GMT
ENV LANG=C.UTF-8
# Wed, 29 Mar 2023 22:25:53 GMT
ENV RUBY_MAJOR=3.1
# Wed, 29 Mar 2023 22:25:53 GMT
ENV RUBY_VERSION=3.1.3
# Wed, 29 Mar 2023 22:25:54 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Wed, 29 Mar 2023 22:29:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 29 Mar 2023 22:29:13 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 29 Mar 2023 22:29:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 29 Mar 2023 22:29:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 22:29:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 29 Mar 2023 22:29:15 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 04:52:52 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 04:53:01 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 04:53:04 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 04:53:05 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 04:53:05 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 04:53:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 04:53:05 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 04:53:05 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 04:53:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 04:53:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 04:53:08 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 04:54:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 04:54:54 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 04:54:54 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 04:54:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 04:54:54 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 04:54:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65ad13b2023bc984343067f4fd6c0e60cb56fa44b7ea6d7d0aeedb5ef6085ae`  
		Last Modified: Wed, 29 Mar 2023 22:36:08 GMT  
		Size: 3.9 MB (3941156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20af8b6ad1ca8f1b69f8e3f0c32270dedb57e35279646158bffcec1b34cc7e59`  
		Last Modified: Wed, 29 Mar 2023 22:36:07 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09537cae90d022ef6c04cf31e5651a1883b55c47b16b3c69a1e4ce6638c1dc3`  
		Last Modified: Wed, 29 Mar 2023 22:36:33 GMT  
		Size: 28.9 MB (28926385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4056c7b458834bdae2bf198abf6c35528074301d3f51a2ffe81426e0d508c094`  
		Last Modified: Wed, 29 Mar 2023 22:36:31 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d86c53f56333f2aedd777f5fc89a43c3aaadfa8254ff189a6ddea455865f7698`  
		Last Modified: Thu, 30 Mar 2023 04:57:51 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc80396bf90de4c111a6182dc9a0da2f0c898abf364e3931519fe969d7f8fac`  
		Last Modified: Thu, 30 Mar 2023 04:58:02 GMT  
		Size: 80.9 MB (80871055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eabaef4e85ce956dffcae20d32765bbdac5800ed7d0fd376925d0bcc21905e0`  
		Last Modified: Thu, 30 Mar 2023 04:57:50 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e6cf7154fa78c30ef953221575af3a2c06edfe04520b34ea29a07d64125081`  
		Last Modified: Thu, 30 Mar 2023 04:57:50 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbfc64c72a6bf95cd5f9ae0c57c33f633c8863d07e0568c27cfac7029110360`  
		Last Modified: Thu, 30 Mar 2023 04:57:51 GMT  
		Size: 3.1 MB (3146004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2fec353b166e32bd5c1c55a37d0cae6255354311dd7808f539a81d224b673b`  
		Last Modified: Thu, 30 Mar 2023 04:57:57 GMT  
		Size: 70.5 MB (70450163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0fbc46f9473f2f607187ba5e14613175ef521d4edf8a097fde478759020e5f`  
		Last Modified: Thu, 30 Mar 2023 04:57:50 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
