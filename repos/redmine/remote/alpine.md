## `redmine:alpine`

```console
$ docker pull redmine@sha256:cf4ec4d559c84d289809ddc6554057e6522d3720200a340c70ba098c12202c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:518ba4effd92c427ef19922743eea649ed001436d8a66fe0de469abb2de00949
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.0 MB (149044368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48a04de41bf1795abeee36effc817551b3de5069209d3ec827816281c81211a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:58 GMT
ADD file:5a707b9d6cb5fff532e4c2141bc35707593f21da5528c9e71ae2ddb6ba4a4eb6 in / 
# Fri, 12 Nov 2021 17:19:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:28:17 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 13 Nov 2021 06:28:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 13 Nov 2021 06:28:18 GMT
ENV LANG=C.UTF-8
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_MAJOR=2.7
# Sat, 13 Nov 2021 06:44:36 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 13 Nov 2021 06:44:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 13 Nov 2021 06:47:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		s390x | armhf | armv7) 			apk add --no-cache libucontext-dev; 			export LIBS='-lucontext'; 			;; 	esac; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 13 Nov 2021 06:47:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 13 Nov 2021 06:47:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:47:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 13 Nov 2021 06:47:56 GMT
CMD ["irb"]
# Sat, 13 Nov 2021 14:28:59 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 13 Nov 2021 14:29:07 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 13 Nov 2021 14:29:07 GMT
ENV RAILS_ENV=production
# Sat, 13 Nov 2021 14:29:08 GMT
WORKDIR /usr/src/redmine
# Sat, 13 Nov 2021 14:29:08 GMT
ENV HOME=/home/redmine
# Sat, 13 Nov 2021 14:29:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_VERSION=4.2.3
# Sat, 13 Nov 2021 14:29:09 GMT
ENV REDMINE_DOWNLOAD_SHA256=72f633dc954217948558889ca85325fe6410cd18a2d8b39358e5d75932a47a0c
# Sat, 13 Nov 2021 14:29:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 13 Nov 2021 14:29:13 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 13 Nov 2021 14:31:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 13 Nov 2021 14:31:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 13 Nov 2021 14:31:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Sat, 13 Nov 2021 14:31:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 13 Nov 2021 14:31:22 GMT
EXPOSE 3000
# Sat, 13 Nov 2021 14:31:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5758d4e389a3f662e94a85fb76143dbe338b64f8d2a65f45536a9663b05305ad`  
		Last Modified: Fri, 12 Nov 2021 17:21:00 GMT  
		Size: 2.8 MB (2822425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e849bc66e37f2d898daa44d76330256a48635f1100e364c0f46206fca7b71`  
		Last Modified: Sat, 13 Nov 2021 06:56:48 GMT  
		Size: 3.6 MB (3582307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a2fc84ba5b32bce31936a6fdf8121f29d2eb485f8525795df7d32046e9f856`  
		Last Modified: Sat, 13 Nov 2021 06:56:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e81c0605571c3961987ae1ce872ebef2b5bcb439010c194e90b47282556c32d`  
		Last Modified: Sat, 13 Nov 2021 06:58:25 GMT  
		Size: 14.0 MB (13994126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2814005984530d27bc89e1c810fb8cb01371038a28bc3d85a1e95b710d9e043e`  
		Last Modified: Sat, 13 Nov 2021 06:58:23 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e171914095295d927972128e1f66156ce389cb697d40fc6d7ea68c919861015e`  
		Last Modified: Sat, 13 Nov 2021 14:36:45 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9802858485f172f49a49aa23ebc2ef97aa9a7dff598d4d6b18f27e107ae24436`  
		Last Modified: Sat, 13 Nov 2021 14:36:55 GMT  
		Size: 69.5 MB (69548252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5b29e3b352df46dbdcf96478507ab2ace06abee4b91e86cea6852a73067d98`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd79647c11e0ebdbaa7b41c71d969403768f7950e69f1b9eda5545fe42e86b3`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20504c29a1f01e91c83c2e1e82a90fb05c118bbf74d44fa621ec588a179bce4b`  
		Last Modified: Sat, 13 Nov 2021 14:36:43 GMT  
		Size: 3.1 MB (3064272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7d43b9df6162fdd2b107724ff288c851a49738e7e04fa16cd34fddde661b04`  
		Last Modified: Sat, 13 Nov 2021 14:36:48 GMT  
		Size: 56.0 MB (56029256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:561c4b4d66001dcdc5ff09131812075d6a6d4f6430e175565724033921e826f1`  
		Last Modified: Sat, 13 Nov 2021 14:36:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
