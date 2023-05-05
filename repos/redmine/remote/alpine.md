## `redmine:alpine`

```console
$ docker pull redmine@sha256:5a45fb86a0cc449ebc1bb0be515caa2a28f35d7ce794a112239388bcf322159a
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

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:8b83627b5e29857a1dad8b21065f1c0ad0544df22f1d64d2b706361f13e016a2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.8 MB (199813433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c9393fc776d76d233cd6822eba976c29a2d3b031b91cea3150faec3f6229952`
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
# Thu, 30 Mar 2023 19:48:33 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:48:33 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:50:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:50:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:50:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:50:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:50:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:50:59 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 20:33:39 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 20:33:46 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 20:33:46 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 20:33:47 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 20:33:47 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 20:33:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 20:33:47 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 20:33:47 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 20:33:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 20:33:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 20:33:51 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 20:35:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 20:35:41 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 20:35:42 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 20:35:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 20:35:42 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 20:35:42 GMT
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
	-	`sha256:1c2a3a5b627564d481f805a55a23e7f1663dd0d7eb7525e247797db9e6369f57`  
		Last Modified: Thu, 30 Mar 2023 20:14:24 GMT  
		Size: 29.3 MB (29326139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89627a8763b3c1b4363004a3ba47b1747ca21550f584f23b7f704f7582ee2473`  
		Last Modified: Thu, 30 Mar 2023 20:14:22 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c13327e88176015ea7bd92b93a7e12975bf5d48a6fa3e9e8dfb38a73db9961`  
		Last Modified: Thu, 30 Mar 2023 20:40:47 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2af3b2ef26593c915dea85cb4452de78ad6dd5cec94b13264981afa37a5f5c`  
		Last Modified: Thu, 30 Mar 2023 20:40:58 GMT  
		Size: 90.4 MB (90427930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e05ac321911eea3893d118374b8778fdc1b5ceed04858dbee7bf6463d1e49f5`  
		Last Modified: Thu, 30 Mar 2023 20:40:44 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe9e179d2750292d5f2c2f6f51ce2ec02bdee36e9891f259a44ead9ec647dd4`  
		Last Modified: Thu, 30 Mar 2023 20:40:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59fcaa1627ad5a2fe13406b0777a754eaf06a639ac51513d35e5b5a53837c1a`  
		Last Modified: Thu, 30 Mar 2023 20:40:45 GMT  
		Size: 3.1 MB (3146039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfebcc2d28284fd149e30d066841c96cab132d3fd89473c20e05488a3c03b493`  
		Last Modified: Thu, 30 Mar 2023 20:40:51 GMT  
		Size: 70.3 MB (70250090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a8519a305d23167a02e20b3d8ad03bf7e7e85ce0798ac490874af0a85d2bc61`  
		Last Modified: Thu, 30 Mar 2023 20:40:44 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:682d2906fa55846959ec4de950a0352cea7a5bfcd440739932c2d8ebfe32de43
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190093024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40910d79fedcff86fe1c4cbb092475f6fd8a62883c67727d1723850f71922aa`
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
# Thu, 30 Mar 2023 19:53:51 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:53:51 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:55:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:55:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:55:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:55:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:55:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:55:56 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 21:10:18 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 21:10:28 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 21:10:30 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 21:10:30 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 21:10:30 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 21:10:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 21:10:30 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 21:10:30 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 21:10:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 21:10:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 21:10:34 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 21:12:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 21:12:36 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 21:12:36 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 21:12:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 21:12:36 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 21:12:36 GMT
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
	-	`sha256:a6d260f62bf114523f1bcc5159778836e87f5d5ba17b8aa37806569fc8336aee`  
		Last Modified: Thu, 30 Mar 2023 20:54:29 GMT  
		Size: 28.3 MB (28271401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1072b09e619daaa81c280c5403881192cde2652df10768d424330edb267334f0`  
		Last Modified: Thu, 30 Mar 2023 20:54:26 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384954b06fdb24cb3dc71b2d0847b77526170f7598176d5ee6a465e123d522d2`  
		Last Modified: Thu, 30 Mar 2023 21:19:13 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85531e5848f8569063914487fd88a126149d1948295aac0fdb166307d584f28`  
		Last Modified: Thu, 30 Mar 2023 21:19:26 GMT  
		Size: 83.9 MB (83936567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e452ad15b6fb2bdc20ff0673eec64af26c9ef13f5d1d93affbef3f353e2a55f`  
		Last Modified: Thu, 30 Mar 2023 21:19:11 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b067573b3d37c32a1d4a1f56804194c7210d30b1e182095da704dbefde1ed1`  
		Last Modified: Thu, 30 Mar 2023 21:19:11 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a46ebf671e188d3107090e44dd2ee6c85a0ecd6a7bf2bd14fe683cdeed95a0`  
		Last Modified: Thu, 30 Mar 2023 21:19:12 GMT  
		Size: 3.1 MB (3146012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbecffbf41b89bf4e064a7e5b903fbb7eb99162df683f13da501023ce16348d`  
		Last Modified: Thu, 30 Mar 2023 21:19:19 GMT  
		Size: 68.5 MB (68524320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6284a43a498181bbe6f5ca155ceb7b113975e56c04058814705aee0410eedff6`  
		Last Modified: Thu, 30 Mar 2023 21:19:11 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:edff5f6c596b8746cdc48b3cc5b466eba51b245117aad292f0babc07cea5395b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.4 MB (187366155 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd89c2cc9439cab962694ba1d2540bab7afc88cbacd70fa07de6abe3c47eb94`
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
# Thu, 30 Mar 2023 19:34:43 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:34:43 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:36:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:36:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:36:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:36:44 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:36:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:36:44 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 20:19:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 20:19:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 20:19:49 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 20:19:49 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 20:19:49 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 20:19:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 20:19:50 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 20:19:50 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 20:19:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 20:19:53 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 20:19:53 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 20:21:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 20:21:46 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 20:21:46 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 20:21:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 20:21:47 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 20:21:47 GMT
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
	-	`sha256:4aeb58706fec0dc5b2bbf9db3c0dad74375ee8a5c471b4fd2dff5c1a1ec3fdad`  
		Last Modified: Thu, 30 Mar 2023 19:59:50 GMT  
		Size: 28.1 MB (28147589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40325f5ddf228c85844f7c755ac50da852e2738744d74fffc9c29f8c3b464859`  
		Last Modified: Thu, 30 Mar 2023 19:59:47 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8f8ef5d4fea782a73808033ffdac3339ceecfc906a662e9733dfd81eeacf11`  
		Last Modified: Thu, 30 Mar 2023 20:25:19 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf76f0c62447fa5e5d935f5e4557c64256a98c7ca99e2d26759020797b4117c`  
		Last Modified: Thu, 30 Mar 2023 20:25:31 GMT  
		Size: 82.1 MB (82059325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a9d55a3df0bd33069bfbf9fb5c8ef54a58bc155287853ef9f55826bd36c188`  
		Last Modified: Thu, 30 Mar 2023 20:25:17 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f81e5cf17c1170e495ac14bccf829e5c74e76394d289572966e8aa036ab4b1d`  
		Last Modified: Thu, 30 Mar 2023 20:25:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b708292c5fb423cef7cf9efaee42b2235cf72642ca4f103339392c9c6173fb7a`  
		Last Modified: Thu, 30 Mar 2023 20:25:19 GMT  
		Size: 3.1 MB (3145770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b412f6feb35bd8ef9ff6203ed00cb0401853d22a271f17b3139352631a17c73`  
		Last Modified: Thu, 30 Mar 2023 20:25:25 GMT  
		Size: 68.1 MB (68127375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd7c4bc337c954734a25674a363a6093ef504a9efa7b87a995bee3a70b5b77b`  
		Last Modified: Thu, 30 Mar 2023 20:25:18 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:d46029bf9bc6e2c1d924b6649f48fc88d7e994b2dc0a9997e595fc140ec1bfb1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.6 MB (195567395 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed442eca2587bb1ca6383d6e705d7e725a549f6e6e7837df8e4d3cb2c66fe03c`
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
# Thu, 30 Mar 2023 19:08:01 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:08:01 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:09:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:09:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:09:47 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:09:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:09:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:09:47 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 19:49:22 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 19:49:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 19:49:29 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 19:49:29 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 19:49:29 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 19:49:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 19:49:29 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 19:49:30 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 19:49:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 19:49:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 19:49:33 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 19:51:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 19:51:09 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 19:51:09 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 19:51:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 19:51:09 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 19:51:09 GMT
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
	-	`sha256:bffc069a521d8bd3fb4a4e76ebc87c221ca58cdc52f3b5ddfff5d8ed8a6fbfdb`  
		Last Modified: Thu, 30 Mar 2023 19:28:55 GMT  
		Size: 28.7 MB (28709573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63b551c9ce36eaccda41c7a86fcd250dde7d47e6ef4ed8d0a6715f726cd71f5`  
		Last Modified: Thu, 30 Mar 2023 19:28:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d82846b1db785ff69dee91de6048599af8742d8e21f14d39175786330a936d5`  
		Last Modified: Thu, 30 Mar 2023 19:55:35 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2469534a47975f46644bc5301e32488fb426eb38cbbc253210b2be4a199538`  
		Last Modified: Thu, 30 Mar 2023 19:55:44 GMT  
		Size: 87.3 MB (87292443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8eda5a8b566514cf8adbbc19014660946516793875dfdef805150a86cc5b34`  
		Last Modified: Thu, 30 Mar 2023 19:55:32 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3ff385bce9be082f8a05527066660818ab96f07629429efc1b43fd3605ce54`  
		Last Modified: Thu, 30 Mar 2023 19:55:32 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40d25b1a6e116e6751582134ddb4461de0a4b0cfae80416f975f59af1c8f4d9b`  
		Last Modified: Thu, 30 Mar 2023 19:55:33 GMT  
		Size: 3.1 MB (3146034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:838bb8f81f535b94cc33f1a1b2f1613b7dd9f964f2b64ca38a076a8d92326bed`  
		Last Modified: Thu, 30 Mar 2023 19:55:38 GMT  
		Size: 69.9 MB (69884646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:750d268b743eb5f511b98c275c79380087d171c9a73a59d30e50276655e0d25f`  
		Last Modified: Thu, 30 Mar 2023 19:55:33 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine` - linux; 386

```console
$ docker pull redmine@sha256:241c80d93349c289d9792b8d732037b44a35dbf060a8f754367db1168255313c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.1 MB (197106978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c4c598c08fc93b3b3325ce6c0c28644b143af84f4a6d04bffa0812a2710589f`
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
# Thu, 30 Mar 2023 19:18:23 GMT
ENV RUBY_VERSION=3.1.4
# Thu, 30 Mar 2023 19:18:23 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Thu, 30 Mar 2023 19:22:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 30 Mar 2023 19:22:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 30 Mar 2023 19:22:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 30 Mar 2023 19:22:51 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 19:22:51 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Thu, 30 Mar 2023 19:22:51 GMT
CMD ["irb"]
# Thu, 30 Mar 2023 20:19:18 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Thu, 30 Mar 2023 20:19:30 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Thu, 30 Mar 2023 20:19:32 GMT
ENV RAILS_ENV=production
# Thu, 30 Mar 2023 20:19:32 GMT
WORKDIR /usr/src/redmine
# Thu, 30 Mar 2023 20:19:32 GMT
ENV HOME=/home/redmine
# Thu, 30 Mar 2023 20:19:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 30 Mar 2023 20:19:32 GMT
ENV REDMINE_VERSION=5.0.5
# Thu, 30 Mar 2023 20:19:32 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Thu, 30 Mar 2023 20:19:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Thu, 30 Mar 2023 20:19:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 30 Mar 2023 20:19:36 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 30 Mar 2023 20:22:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 30 Mar 2023 20:22:11 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 30 Mar 2023 20:22:11 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Thu, 30 Mar 2023 20:22:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 30 Mar 2023 20:22:11 GMT
EXPOSE 3000
# Thu, 30 Mar 2023 20:22:11 GMT
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
	-	`sha256:72c8e3da93ac4548269613fd57fda0c4fc9b8434403d38ea08af68d0dee5d899`  
		Last Modified: Thu, 30 Mar 2023 19:57:50 GMT  
		Size: 28.1 MB (28130416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f53ea2e75968da4a3f7d53e5d1bcda3cee766c5e495fe3109819ab6bc0b21fd`  
		Last Modified: Thu, 30 Mar 2023 19:57:46 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7298cab2b3708749856155ee6e6a6e960c8976a635b7f8c172b31b4e6991d0`  
		Last Modified: Thu, 30 Mar 2023 20:28:12 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27230bc97f24983e3953a9c2e5f9c588fd7a2c387cd156f001dc54454598189`  
		Last Modified: Thu, 30 Mar 2023 20:28:31 GMT  
		Size: 90.3 MB (90301589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65312781fbcf164afbeb3327430458bf9f97bc661dab73568176c2f6995daa5`  
		Last Modified: Thu, 30 Mar 2023 20:28:10 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71c46e9bc6f0211ae265e8497db82f5f13d2013846bb402ad9153a283abd4b62`  
		Last Modified: Thu, 30 Mar 2023 20:28:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0d93a5a6f4bf026e0a626f4677b6504de536160a2b59e86ddbc68e1bd3bbd5`  
		Last Modified: Thu, 30 Mar 2023 20:28:11 GMT  
		Size: 3.1 MB (3146014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652bebe65ec0bd6f977fa8fe4a161ee1047e8e5bdba2a33eb9dfbd95a674936e`  
		Last Modified: Thu, 30 Mar 2023 20:28:20 GMT  
		Size: 68.8 MB (68827534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09d31b3d9d71599023d21b7bb998de5bbcc736165feb676d54942d183d1f9e3`  
		Last Modified: Thu, 30 Mar 2023 20:28:10 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine` - linux; ppc64le

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

### `redmine:alpine` - linux; s390x

```console
$ docker pull redmine@sha256:43665a5e35ce21bff2fee8d302157dbaecf0d7ad41c62f22f61cab980a82c081
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.0 MB (189975146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486a29e53579adafe0dffb6710c3dc7c4f0a3d8d071ad6f5ba46266a3ef01b93`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 03 May 2023 21:46:13 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 03 May 2023 21:46:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 03 May 2023 21:46:14 GMT
ENV LANG=C.UTF-8
# Wed, 03 May 2023 21:55:26 GMT
ENV RUBY_MAJOR=3.1
# Wed, 03 May 2023 21:55:26 GMT
ENV RUBY_VERSION=3.1.4
# Wed, 03 May 2023 21:55:26 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Wed, 03 May 2023 21:57:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 03 May 2023 21:57:43 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 03 May 2023 21:57:43 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 03 May 2023 21:57:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 May 2023 21:57:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Wed, 03 May 2023 21:57:44 GMT
CMD ["irb"]
# Fri, 05 May 2023 00:42:21 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 05 May 2023 00:42:35 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Fri, 05 May 2023 00:42:39 GMT
ENV RAILS_ENV=production
# Fri, 05 May 2023 00:42:39 GMT
WORKDIR /usr/src/redmine
# Fri, 05 May 2023 00:42:39 GMT
ENV HOME=/home/redmine
# Fri, 05 May 2023 00:42:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 05 May 2023 00:42:40 GMT
ENV REDMINE_VERSION=5.0.5
# Fri, 05 May 2023 00:42:40 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.5.tar.gz
# Fri, 05 May 2023 00:42:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=a89ad1c4bb9bf025e6527c77ab18c8faf7749c94a975caf2cfdbba00eb12a481
# Fri, 05 May 2023 00:42:42 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 05 May 2023 00:42:43 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Fri, 05 May 2023 00:44:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 05 May 2023 00:44:33 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 05 May 2023 00:44:33 GMT
COPY file:f2dac8fc10b4b9c85d18ffc54f3822ba7f98c858ad133cc1c0a63d9d52731204 in / 
# Fri, 05 May 2023 00:44:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 05 May 2023 00:44:34 GMT
EXPOSE 3000
# Fri, 05 May 2023 00:44:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab8b1ca33663c42ad310c6ae6a06986960378968a7f0e03f269a8bec7b16904`  
		Last Modified: Wed, 03 May 2023 22:10:11 GMT  
		Size: 3.9 MB (3941099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86f86a28f33679132831614379a4315c67bf8bb62db163302c454f3e0ff3f97`  
		Last Modified: Wed, 03 May 2023 22:10:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f83467cd4561ef1474874c0d8ed22480ecdd0fe96367ec28f63fee9c220dc4`  
		Last Modified: Wed, 03 May 2023 22:10:51 GMT  
		Size: 28.9 MB (28933448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59591a9a7b8c2ddd2a4352ecbd2ebd2c6e9e5acef9ced282e748fbe731b6af7`  
		Last Modified: Wed, 03 May 2023 22:10:49 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5e2df7a688c8669df6f56b4a538291d4b22a0a771d127deb9f8c48525bfa3d`  
		Last Modified: Fri, 05 May 2023 00:50:15 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5345318050d0b19e37901f20fea81412671c12366f6da9b3eb5feb63a11cbf82`  
		Last Modified: Fri, 05 May 2023 00:50:26 GMT  
		Size: 80.9 MB (80896416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e748ffb6415b47e5dbf4f5072fe79ce2dc80128d028ce38c57361d61cc8bd1`  
		Last Modified: Fri, 05 May 2023 00:50:14 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f6d03a3bf4ba582ead78dada46260bfa4a1dc7b2de0e43dea9677cbb7ac07db`  
		Last Modified: Fri, 05 May 2023 00:50:14 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb020ba16e7396923e3bd90a4f95250e35ea33b5fccbfe22f00c1e711035901`  
		Last Modified: Fri, 05 May 2023 00:50:15 GMT  
		Size: 3.1 MB (3146009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce774944a63830d25282a751c2b69f0b1b4386c488b544089a260fb29c4a787d`  
		Last Modified: Fri, 05 May 2023 00:50:21 GMT  
		Size: 70.5 MB (70460845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5666e7c805beb93d53ee582f9f818d9d4c461a6c51ddd8b5c38d8463311765`  
		Last Modified: Fri, 05 May 2023 00:50:14 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
