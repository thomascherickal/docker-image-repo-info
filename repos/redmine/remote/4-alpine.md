## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:b1651c4e29b3219c5e6cb28c4df1a212a17486babd5ace3e3b89cd272d3b9b31
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
$ docker pull redmine@sha256:990a3f40114c8eb81919cf2a3f8d2744252398f9186ea03fbf9cdcc506f22f62
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156069855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65f3252d87125c28dc0f47a25a466e8977bc14b0e995d69869787e7e0dc9f1d4`
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
# Tue, 07 Dec 2021 23:30:57 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Tue, 07 Dec 2021 23:30:58 GMT
ENV RAILS_ENV=production
# Tue, 07 Dec 2021 23:30:58 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Dec 2021 23:30:58 GMT
ENV HOME=/home/redmine
# Tue, 07 Dec 2021 23:30:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Dec 2021 23:30:59 GMT
ENV REDMINE_VERSION=4.2.3
# Tue, 07 Dec 2021 23:30:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Tue, 07 Dec 2021 23:31:03 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 07 Dec 2021 23:31:04 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Tue, 07 Dec 2021 23:33:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 07 Dec 2021 23:33:11 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 07 Dec 2021 23:33:12 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Tue, 07 Dec 2021 23:33:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 07 Dec 2021 23:33:12 GMT
EXPOSE 3000
# Tue, 07 Dec 2021 23:33:12 GMT
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
	-	`sha256:209fca68b7f9657e0a3696b0039f10fcde5e9276d40953425bac9836cee54672`  
		Last Modified: Tue, 07 Dec 2021 23:45:24 GMT  
		Size: 76.8 MB (76773695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f25bfc32ad166dc726540194adfc457fbb709d5e8c85d1690d326fd208d3e9`  
		Last Modified: Tue, 07 Dec 2021 23:45:10 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d1e868ad8b0d15f584292647f9dba9699201c701652bd0e0c132d0eeba7acc`  
		Last Modified: Tue, 07 Dec 2021 23:45:10 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38978a8f5a3ce1b62f2e1fe245359cd185dbdc9ab1a6829b75b83e5eb038803`  
		Last Modified: Tue, 07 Dec 2021 23:45:11 GMT  
		Size: 3.1 MB (3064282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd351df3b3b56c582a91938831c628e2f2ca04c3b5ce12fc8695ba3cedfa490e`  
		Last Modified: Tue, 07 Dec 2021 23:45:16 GMT  
		Size: 55.7 MB (55741633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d518ebcfae3b722650d4cff80714880de0e13f77f658a9bf5195195b2bcf23`  
		Last Modified: Tue, 07 Dec 2021 23:45:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:9deb1ecfe754d08f7311a91bb4add0c7e1ea809c29e64f3b77d67c5180149042
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.7 MB (149703670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd705ac4a610f4119f1143ec6ad08a77bdbdfba79c87da3851fcff7de45230ab`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:31:21 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Tue, 30 Nov 2021 05:31:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 30 Nov 2021 05:31:23 GMT
ENV LANG=C.UTF-8
# Tue, 30 Nov 2021 05:41:29 GMT
ENV RUBY_MAJOR=2.7
# Tue, 30 Nov 2021 05:41:30 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 30 Nov 2021 05:41:30 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 30 Nov 2021 05:45:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 30 Nov 2021 05:45:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 30 Nov 2021 05:45:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 30 Nov 2021 05:45:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 05:45:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 30 Nov 2021 05:45:27 GMT
CMD ["irb"]
# Wed, 15 Dec 2021 19:59:11 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 15 Dec 2021 19:59:44 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 15 Dec 2021 19:59:45 GMT
ENV RAILS_ENV=production
# Wed, 15 Dec 2021 19:59:46 GMT
WORKDIR /usr/src/redmine
# Wed, 15 Dec 2021 19:59:47 GMT
ENV HOME=/home/redmine
# Wed, 15 Dec 2021 19:59:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 15 Dec 2021 19:59:49 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 15 Dec 2021 19:59:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 15 Dec 2021 20:00:07 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 15 Dec 2021 20:00:07 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 15 Dec 2021 20:06:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 15 Dec 2021 20:06:15 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 15 Dec 2021 20:06:16 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 15 Dec 2021 20:06:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 15 Dec 2021 20:06:17 GMT
EXPOSE 3000
# Wed, 15 Dec 2021 20:06:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842eb5d56c73e6f9e351db359308334ee810d1cb732270ae35bfdaa5208caf9c`  
		Last Modified: Tue, 30 Nov 2021 05:52:37 GMT  
		Size: 3.4 MB (3441437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c29b1da293c8320455d68a5d44ebe572144259afdb3aed7c4d69ac9d80a4d2`  
		Last Modified: Tue, 30 Nov 2021 05:52:34 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a83fcafa12294c811a8d455918c7b657fdf639f25ae44f6b4d12a4ef579f402`  
		Last Modified: Tue, 30 Nov 2021 05:54:08 GMT  
		Size: 13.4 MB (13411614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe3677ca64582d63aa23f90040bf190c5adb6c64280647662a63a0a6591e692`  
		Last Modified: Tue, 30 Nov 2021 05:54:00 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fc611248b9b7a30ce2efc14e5c3c60e44f4c9df47a3ab0c93796c65c457e53`  
		Last Modified: Wed, 15 Dec 2021 20:36:47 GMT  
		Size: 1.2 KB (1221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8b615d00225b1ae4f96dfd492db13c1835eda95ffac3978a2e39334a59f45b`  
		Last Modified: Wed, 15 Dec 2021 20:37:34 GMT  
		Size: 72.3 MB (72250838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf1032dafd28175d5caf29a236801fd2cd9f1a8d72ddc210cc05d61a5dc7573`  
		Last Modified: Wed, 15 Dec 2021 20:36:45 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24788a6d00131a74cc1cea35cb291503aba303a056769b2b46944aaf21a2f71`  
		Last Modified: Wed, 15 Dec 2021 20:36:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bd699752e64f05889c247721fc14b0482fb7f363051676ab85ef8938eef2cf`  
		Last Modified: Wed, 15 Dec 2021 20:36:51 GMT  
		Size: 3.1 MB (3064283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf5c73be7af6935ff0961029c8c5d4498e0a9fa24b10c3a9f88725ee05488ec`  
		Last Modified: Wed, 15 Dec 2021 20:37:10 GMT  
		Size: 54.9 MB (54900336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dcedf71fe9c88fc4760abbbeced1fcab3506df6516a8635f4593d318e906bb`  
		Last Modified: Wed, 15 Dec 2021 20:36:46 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:1851357d13b5cf69bc9bbc4bea480103e9911493ea649f377fd5e9a7f2b5ceb9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.6 MB (145578656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e1f8486a749157441f5def413b75f74535369444955b3fcde090c7e13e98d84`
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
# Wed, 08 Dec 2021 01:03:41 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 08 Dec 2021 01:03:43 GMT
ENV RAILS_ENV=production
# Wed, 08 Dec 2021 01:03:43 GMT
WORKDIR /usr/src/redmine
# Wed, 08 Dec 2021 01:03:44 GMT
ENV HOME=/home/redmine
# Wed, 08 Dec 2021 01:03:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 08 Dec 2021 01:03:46 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 08 Dec 2021 01:03:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 08 Dec 2021 01:03:52 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 08 Dec 2021 01:03:53 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 08 Dec 2021 01:09:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 08 Dec 2021 01:09:30 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 08 Dec 2021 01:09:31 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 08 Dec 2021 01:09:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 08 Dec 2021 01:09:32 GMT
EXPOSE 3000
# Wed, 08 Dec 2021 01:09:32 GMT
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
	-	`sha256:d2580a15ac1182b1a1b12c09d99bf33cb0795675de3b0d9be4be48f1bf8ce07d`  
		Last Modified: Wed, 08 Dec 2021 01:39:58 GMT  
		Size: 68.9 MB (68854327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e1a1b0570a99dd9d196c5c7e8835cfbdd9a0c31ec402a8542e686752289421`  
		Last Modified: Wed, 08 Dec 2021 01:39:14 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e46ba3449e05e287636088e0e37a3c77911c06f1da3755b0fde8fe3a6f82360`  
		Last Modified: Wed, 08 Dec 2021 01:39:15 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df77c9ad615154dcc5cb09138d2265cddb48ca91d90da9038715a5d1d99bc72`  
		Last Modified: Wed, 08 Dec 2021 01:39:18 GMT  
		Size: 3.1 MB (3064253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f1291f2ab23c6a608787f2e82b1e7e91b4e03579511eabcf1e4589ae062847`  
		Last Modified: Wed, 08 Dec 2021 01:39:38 GMT  
		Size: 54.6 MB (54613949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde3b7165f5f307731f8b8bdcb384a6dd57ba693ca9bd79dc995eb6e9607e108`  
		Last Modified: Wed, 08 Dec 2021 01:39:15 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:fb51441b43b7323257f5fcd3db7970bada0e8c70693261ef19fa276ef73b2406
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.7 MB (159711265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b33dd2b26f008b43f6f8b75fdb3f38c30ec9368e9b89c4d0bd097260600ea524`
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
# Thu, 06 Jan 2022 20:27:43 GMT
ENV REDMINE_VERSION=4.2.3
# Thu, 06 Jan 2022 20:27:44 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Thu, 06 Jan 2022 20:27:49 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 06 Jan 2022 20:27:49 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 06 Jan 2022 20:30:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 06 Jan 2022 20:30:15 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 06 Jan 2022 20:30:16 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Thu, 06 Jan 2022 20:30:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Jan 2022 20:30:17 GMT
EXPOSE 3000
# Thu, 06 Jan 2022 20:30:18 GMT
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
	-	`sha256:670c38ae06a193ddd6b897ef7a72a8796e0aa0f29d8c2f70cec42649806f5e1a`  
		Last Modified: Thu, 06 Jan 2022 20:36:52 GMT  
		Size: 3.1 MB (3064365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fb2a113c8cf464c0df979b336cb68dc46d12dd75a94b7d35884f1a1c2b5d52`  
		Last Modified: Thu, 06 Jan 2022 20:36:58 GMT  
		Size: 57.0 MB (56990479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286d92c729cfe083f01d9a85b245f457a191da9e1d81dfb880d4bf808d83eea0`  
		Last Modified: Thu, 06 Jan 2022 20:36:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; 386

```console
$ docker pull redmine@sha256:6b5917b41889be158e16132cd9baf004906d977b70ce0990ed944502197e4c8a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **163.2 MB (163198887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bcd71ebbc2bf8c563a185afa5cffa68a36481ed7f75e06e860b81e9476e50e1`
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
# Thu, 06 Jan 2022 20:14:53 GMT
ENV REDMINE_VERSION=4.2.3
# Thu, 06 Jan 2022 20:14:53 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Thu, 06 Jan 2022 20:14:58 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 06 Jan 2022 20:14:58 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 06 Jan 2022 20:17:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 06 Jan 2022 20:17:33 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 06 Jan 2022 20:17:33 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Thu, 06 Jan 2022 20:17:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Jan 2022 20:17:34 GMT
EXPOSE 3000
# Thu, 06 Jan 2022 20:17:34 GMT
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
	-	`sha256:a71ca73d88a3ff571fd65d5d03727f5a6c7aefaa81e8d17f90039a9b02024e6e`  
		Last Modified: Thu, 06 Jan 2022 20:25:06 GMT  
		Size: 3.1 MB (3064282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174c2f2d870a0c595aa6dc0cc48de1958a590efeddfef961c5d207d905340d3e`  
		Last Modified: Thu, 06 Jan 2022 20:25:14 GMT  
		Size: 56.5 MB (56466995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef72d57c982e071a9c03b9c23990e8a9e5ded56f663470f37b3c104e2e8f848e`  
		Last Modified: Thu, 06 Jan 2022 20:25:05 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; ppc64le

```console
$ docker pull redmine@sha256:166db002ecfe5d18a61bb65bfc78dc67a214d306430422b4899831a9274351fe
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.6 MB (157640113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:102f5197b20ef9a9aba0cfb934fd2c50863a94978db87600a4e1831e18ee01cc`
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
# Wed, 08 Dec 2021 00:42:39 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 08 Dec 2021 00:42:46 GMT
ENV RAILS_ENV=production
# Wed, 08 Dec 2021 00:42:48 GMT
WORKDIR /usr/src/redmine
# Wed, 08 Dec 2021 00:42:50 GMT
ENV HOME=/home/redmine
# Wed, 08 Dec 2021 00:42:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 08 Dec 2021 00:42:58 GMT
ENV REDMINE_VERSION=4.2.3
# Wed, 08 Dec 2021 00:42:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Wed, 08 Dec 2021 00:43:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 08 Dec 2021 00:43:11 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 08 Dec 2021 00:46:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 08 Dec 2021 00:47:03 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 08 Dec 2021 00:47:09 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 08 Dec 2021 00:47:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 08 Dec 2021 00:47:17 GMT
EXPOSE 3000
# Wed, 08 Dec 2021 00:47:18 GMT
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
	-	`sha256:fd6d65193bbf6fd7974dcdbd10a270fd167119185f378a12238451fd8665e3a9`  
		Last Modified: Wed, 08 Dec 2021 01:26:04 GMT  
		Size: 77.0 MB (76993034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fb46827ce29ecda6adca20e0389f69bd1d2bb440f88a49c6eb5207eadc97dc4`  
		Last Modified: Wed, 08 Dec 2021 01:25:05 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed08a587b539fda11e1ee11a5e22f385353b34a7c8b99ab66d43f76fd5ac3be`  
		Last Modified: Wed, 08 Dec 2021 01:25:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30cd29e12ba1c863b2424c2b3b7a4b1947964913be63648ccef2a5814a90d75a`  
		Last Modified: Wed, 08 Dec 2021 01:25:13 GMT  
		Size: 3.1 MB (3064268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08176a18c41dda5ee5f4940f56f0dc8222937a612e7fdc67671fe9020dcb5476`  
		Last Modified: Wed, 08 Dec 2021 01:25:34 GMT  
		Size: 56.5 MB (56536769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbab0da4d1faa84a11c043479413b9572d7b0713f8971476c474f70a9ae366a`  
		Last Modified: Wed, 08 Dec 2021 01:25:05 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4-alpine` - linux; s390x

```console
$ docker pull redmine@sha256:e4412133e53124d2ede2e1b713ae29a7881628303da903493caf394a6791185d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.1 MB (155111244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f40445ca4e9ecef1f01dd2ddcaf206abbee3a0dcbaf56c966e7646cc58f41a1`
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
# Thu, 06 Jan 2022 20:13:14 GMT
ENV REDMINE_VERSION=4.2.3
# Thu, 06 Jan 2022 20:13:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Thu, 06 Jan 2022 20:13:17 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 06 Jan 2022 20:13:17 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Thu, 06 Jan 2022 20:15:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 06 Jan 2022 20:15:10 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 06 Jan 2022 20:15:10 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Thu, 06 Jan 2022 20:15:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 06 Jan 2022 20:15:11 GMT
EXPOSE 3000
# Thu, 06 Jan 2022 20:15:11 GMT
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
	-	`sha256:ef43a5202d3974b6bd3c521104e888eb7cb149dbd5acfccc1831f93551b71e45`  
		Last Modified: Thu, 06 Jan 2022 20:20:50 GMT  
		Size: 3.1 MB (3064298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d452b8a04a15ed3717414b5d0c9f1ee42a206cbae3ab4271912666e2d6e8e1e2`  
		Last Modified: Thu, 06 Jan 2022 20:20:55 GMT  
		Size: 57.2 MB (57236737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8658e14b4a17b61109d47e3d4cbb6bba7d48aae02b992162a4233a820019586f`  
		Last Modified: Thu, 06 Jan 2022 20:20:50 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
