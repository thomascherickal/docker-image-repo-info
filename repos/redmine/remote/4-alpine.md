## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:f6acfe95b1e168862ec4a30c40daf724261db9e658d6c6900aee89340e3a9ec9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:565553b54661d93b1a8fc68c4c693b3300e0d20b60ed587b3df7200dd9a3783e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155056434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c694f4a650c98037c231fb541bba077c4ac025ce4e958ec10d6cef8a92e273e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 22:04:24 GMT
RUN apk add --no-cache 		gmp-dev
# Mon, 21 Oct 2019 22:04:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Mon, 21 Oct 2019 22:07:38 GMT
ENV RUBY_MAJOR=2.6
# Mon, 21 Oct 2019 22:07:38 GMT
ENV RUBY_VERSION=2.6.5
# Mon, 21 Oct 2019 22:07:38 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Mon, 21 Oct 2019 22:10:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 21 Oct 2019 22:10:21 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 21 Oct 2019 22:10:21 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 21 Oct 2019 22:10:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 21 Oct 2019 22:10:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 21 Oct 2019 22:10:22 GMT
CMD ["irb"]
# Tue, 22 Oct 2019 00:15:38 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Tue, 22 Oct 2019 00:15:52 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Tue, 22 Oct 2019 00:15:53 GMT
ENV RAILS_ENV=production
# Tue, 22 Oct 2019 00:15:53 GMT
WORKDIR /usr/src/redmine
# Tue, 22 Oct 2019 00:15:53 GMT
ENV HOME=/home/redmine
# Tue, 22 Oct 2019 00:15:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 30 Dec 2019 23:34:38 GMT
ENV REDMINE_VERSION=4.1.0
# Mon, 30 Dec 2019 23:34:38 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Mon, 30 Dec 2019 23:34:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 30 Dec 2019 23:36:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		imagemagick6-dev 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 30 Dec 2019 23:36:13 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 30 Dec 2019 23:36:13 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Mon, 30 Dec 2019 23:36:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 30 Dec 2019 23:36:13 GMT
EXPOSE 3000
# Mon, 30 Dec 2019 23:36:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81839f6c7e4a62b6b4b89424e9f5e4dbb32ecf955ac07f9a348d57b9d6b0347e`  
		Last Modified: Mon, 21 Oct 2019 22:18:41 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74d1ce2ee2b7e47bae7fb763eb17d6c0a654bcecc699eac708bc23628c8ef10a`  
		Last Modified: Mon, 21 Oct 2019 22:18:41 GMT  
		Size: 194.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5a157b0fb9c39dae3e1adaa90cd7197fb90c3827eac6e84468f6fa584422992`  
		Last Modified: Mon, 21 Oct 2019 22:18:56 GMT  
		Size: 22.1 MB (22078313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd1c732d3e5fb94758eb2b795ba475ac8328d70f510c3b46f10e1636970e3283`  
		Last Modified: Mon, 21 Oct 2019 22:18:52 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2429943e49fda8d0b38c92fb22def8816e414ff531070ffe85fb3356171cd8a`  
		Last Modified: Tue, 22 Oct 2019 00:22:44 GMT  
		Size: 1.2 KB (1214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16fea0ab94a4aaa762fd2c276d3e1e0a7b478a8d7e454b4831a72bd2c9d626`  
		Last Modified: Tue, 22 Oct 2019 00:22:57 GMT  
		Size: 65.7 MB (65706757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a2209a1bc5fbbe15328db89bf1e4c8b455b5ec7ce14f3cfcd1ba300b88decd`  
		Last Modified: Tue, 22 Oct 2019 00:22:42 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100f192d75b912d6572c5640429c3cb1825cbae17c830be3b3c22ae6b68c479a`  
		Last Modified: Tue, 22 Oct 2019 00:22:42 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acbe0cce3dfba0b2f8a715e31a139c068ed88514d1a68523e2a1f81ec4e4e84e`  
		Last Modified: Mon, 30 Dec 2019 23:37:22 GMT  
		Size: 2.7 MB (2736260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acd455e7f060747138b6b4a3aa79b49e04ff6c350585eacf091f4fb3506a1df`  
		Last Modified: Mon, 30 Dec 2019 23:37:28 GMT  
		Size: 60.7 MB (60713816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1f16fc85324145749168a0fe5b45bb4a989be3049f9ed291f00067485011aa`  
		Last Modified: Mon, 30 Dec 2019 23:37:21 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
