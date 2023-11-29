## `redmine:alpine`

```console
$ docker pull redmine@sha256:20c2cd61fd5dd9eb576f213e450c2435465046ec7509c45d0a1af5d8009589d5
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 13
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:7aefad553c8ca1c7027e91a661e412286dede792402cf219b490cc69bceeaf15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.5 MB (220529077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e9b4257bccc173eda678ec2883484630db02caae151ad0f0999e7398360960`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:11:31 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 03:11:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 03:11:32 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 03:26:23 GMT
ENV RUBY_MAJOR=3.1
# Sat, 21 Oct 2023 03:26:24 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 21 Oct 2023 03:26:24 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 21 Oct 2023 03:28:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 03:28:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 03:28:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 03:28:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 03:28:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 03:28:35 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4aa1eac13c67269190a4c7f27a8ce412c32f75e636e984c567ba29d75a7b0546`  
		Last Modified: Sat, 21 Oct 2023 03:34:34 GMT  
		Size: 4.1 MB (4131443 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6b5a8305b1a57a6245aaf891d0482f1fc5455f7318480149d9b9792d11463a31`  
		Last Modified: Sat, 21 Oct 2023 03:34:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5361b85a0b7658251a123f00b4bb554943cd37b1225ed1fb9ef74bfd9270bb33`  
		Last Modified: Sat, 21 Oct 2023 03:35:55 GMT  
		Size: 29.9 MB (29884735 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f97f93069985e6d43276dc1f8bd5e543e7e5cfdf30cb1298ce059a40887e7677`  
		Last Modified: Sat, 21 Oct 2023 03:35:52 GMT  
		Size: 173.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c86e2557a7ab3397dd0cba92d6a75aae2fc7faf65ccdd0cebb4d370394585f14`  
		Last Modified: Wed, 29 Nov 2023 17:35:44 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4d60b7dee39144b5c0b821100ebd50de7c22e498a5cd75ac4d20ced25dfbd450`  
		Last Modified: Wed, 29 Nov 2023 17:35:47 GMT  
		Size: 87.3 MB (87314465 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0d4b5a9787cc4c1c663ea0b46e79890650e63b10ae7904926a35f53ed8e09971`  
		Last Modified: Wed, 29 Nov 2023 17:35:40 GMT  
		Size: 137.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f4327eb15da04c4a9311a886340aed257c6b2509d57342ff685c8960d97003f8`  
		Last Modified: Wed, 29 Nov 2023 17:35:40 GMT  
		Size: 125.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c89339a7c72112a539eccced1659356a4da67fe9fbb1ae7915c577a4d4285789`  
		Last Modified: Wed, 29 Nov 2023 17:35:45 GMT  
		Size: 3.2 MB (3236517 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4c8086e7644825e59d1f12143abd88b843e72134a25baf25052af00d467d6842`  
		Last Modified: Wed, 29 Nov 2023 17:35:47 GMT  
		Size: 92.6 MB (92556073 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4958b4547afda8ddd568f53959d5771de2a00f044dc4c0d219aaa589fbc8a026`  
		Last Modified: Wed, 29 Nov 2023 17:35:45 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:47a85ffab935aa4747bf9738fc7233308bbd414a74e459803ac42797ef224091
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4609958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8cb7207a12d6870e2395c725c797b2494f6280382e3ca66279c8fe634015407`

```dockerfile
```

-	Layers:
	-	`sha256:2e15ce07909ac9f99c0cd0d9e34fcf1d7b68491f42e7cf64f49aaa53aef8474a`  
		Last Modified: Wed, 29 Nov 2023 17:35:44 GMT  
		Size: 4.6 MB (4574974 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:59ab28ced8c520c80612197b3ce5c83aed9d47dcf500e6ddab408eb8432b985f`  
		Last Modified: Wed, 29 Nov 2023 17:35:44 GMT  
		Size: 35.0 KB (34984 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:alpine` - linux; arm variant v6

```console
$ docker pull redmine@sha256:a8bc930b760aaaafa37432ada986d4b00b7f483aab898bbb02a8bccc9545ab3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.2 MB (212196704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c2a23cba062ef0ebc58713a3c970486280ed4ebeb46aaf4845b62f596917ae8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:43:47 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 00:43:47 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 00:43:47 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 00:56:02 GMT
ENV RUBY_MAJOR=3.1
# Sat, 21 Oct 2023 00:56:02 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 21 Oct 2023 00:56:02 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 21 Oct 2023 00:58:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 00:58:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 00:58:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 00:58:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:58:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 00:58:28 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f673ff883163cbdf5d096ae4e56eabd4965586ea42893cf760d88961235874`  
		Last Modified: Sat, 21 Oct 2023 01:04:04 GMT  
		Size: 3.8 MB (3807424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00c0aed38036eea1aeb6ea20f77bc395966346924174fd9392268a8c47e66f3`  
		Last Modified: Sat, 21 Oct 2023 01:04:03 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d85c5ae5793bc9675353432ea3c9b699cc27694fc7ab05eae5cd53640356b27`  
		Last Modified: Sat, 21 Oct 2023 01:05:17 GMT  
		Size: 28.8 MB (28764767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d03788d79e4045344a5d2f660f448c49b4abb92606b7d79b2403940a6f083bd`  
		Last Modified: Sat, 21 Oct 2023 01:05:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee0e95a4466628a99a08a5c08a6274fa92929dfc34a634e95308d84d9346dec`  
		Last Modified: Sat, 18 Nov 2023 20:24:25 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2ec1ad2f607860a3c0d57ea72f31e7b024dc7e7981148353e4351b50403e4f2`  
		Last Modified: Sat, 18 Nov 2023 20:24:38 GMT  
		Size: 82.9 MB (82896227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94fc2824c776a25e86eb12cdec9725997ab78af6fb90a81d2b3ed16bf5614fd`  
		Last Modified: Sat, 18 Nov 2023 20:24:23 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d801a5f31557504958dcdcee40433ac398b6c39ca1947fffd859247c27098e44`  
		Last Modified: Sat, 18 Nov 2023 20:24:23 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1ba9a84d296546531a93967884ad03c16a9ec643c77843331c6090266c89ce`  
		Last Modified: Wed, 29 Nov 2023 06:15:58 GMT  
		Size: 3.2 MB (3236500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce39803dbeb732b8a4238245da8d5fc894b3ca59d230adaa03fcff7046b6ffe8`  
		Last Modified: Wed, 29 Nov 2023 06:16:06 GMT  
		Size: 90.3 MB (90342621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e073003b24742f0995d3469efe1bd5204a19864125cc15b70b64551c3a18b1c`  
		Last Modified: Wed, 29 Nov 2023 06:15:57 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:alpine` - linux; arm variant v7

```console
$ docker pull redmine@sha256:30e42be8ab026e22197b8fa2a7b197a748f32bd2e4cf9772678b00c81e1ecdea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.0 MB (206957669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:492be2e170185583351991ee97b4aef3fa0024391d62073402908855868ccd35`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:08:10 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 01:08:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 01:08:11 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 01:20:38 GMT
ENV RUBY_MAJOR=3.1
# Sat, 21 Oct 2023 01:20:38 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 21 Oct 2023 01:20:39 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 21 Oct 2023 01:22:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 01:22:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 01:22:54 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 01:22:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 01:22:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 01:22:55 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db414e90fabd568227d38efa5d95aac12ab5de1a7d426bee026b5f3f8118bd46`  
		Last Modified: Sat, 21 Oct 2023 01:29:40 GMT  
		Size: 3.7 MB (3717167 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b3da1322e16d65c0b8597c82348f9ac8cd2d0e26e59b842b785f3bb683593c97`  
		Last Modified: Sat, 21 Oct 2023 01:29:38 GMT  
		Size: 224.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dd580861c2883c3567a77345cf019d71773f0e4dbcfd8aea4f713c5bc5d8e69c`  
		Last Modified: Sat, 21 Oct 2023 01:31:06 GMT  
		Size: 28.6 MB (28597381 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:80d6096158a1db17db180211f577459be3d2515a88e0abcfc83f791857fa79bf`  
		Last Modified: Sat, 21 Oct 2023 01:31:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:304e0b4022eb9b8fa9297a15ce9db7bc92b5c90e71c5be69a812460730533dfb`  
		Last Modified: Sat, 21 Oct 2023 06:45:33 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4cdba2893374e600c2c8aefa524c40dd78c545f499f223aa0a67e61b80b41d44`  
		Last Modified: Sat, 21 Oct 2023 06:45:38 GMT  
		Size: 79.5 MB (79467526 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7d0d0b956d4119813fa5671454856d28faebcc2ec2ff8f8662c015fa8d8e99c4`  
		Last Modified: Sat, 21 Oct 2023 06:45:34 GMT  
		Size: 134.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:994fa3aed3c4a06061a0aa87c075d3335c39da59634ae12b4cb47ff5ac25d1f8`  
		Last Modified: Sat, 21 Oct 2023 06:45:34 GMT  
		Size: 124.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:93456276076eea58cd098f83c86675b4609b6ac51534ef2d8278e87a4ba14132`  
		Last Modified: Wed, 29 Nov 2023 10:44:00 GMT  
		Size: 3.2 MB (3236500 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b944ba3d4af89b274cb000522009725bf953bafb5deb3225146d1919028ba31`  
		Last Modified: Wed, 29 Nov 2023 10:44:02 GMT  
		Size: 89.0 MB (89035319 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99ab8f4118ec63de97a68e89eb613c7b6a84999d3f620586dfd389ff61d40246`  
		Last Modified: Wed, 29 Nov 2023 10:43:59 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:bec1171b552d2277147ff8938a026f309fe7651702d5e44abb39978a6590e12b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4597685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e47e29a44ce42397146fc935ced2e08f993cdc5bd74a2c467ba40a04215302f8`

```dockerfile
```

-	Layers:
	-	`sha256:4b0f71ba44040626e804d06d659d31408aa16f92a92045d6c7bcc742b413dbf8`  
		Last Modified: Wed, 29 Nov 2023 10:44:00 GMT  
		Size: 4.6 MB (4563363 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:98b06cb3c9316cecae273c2945b7536c20eed4fc13b093c7340a4002b9a40c43`  
		Last Modified: Wed, 29 Nov 2023 10:43:59 GMT  
		Size: 34.3 KB (34322 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:alpine` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:6cebcf443890e4315c743da82a5be3475435da3d65b6b1983b7dfa8596f5174d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.2 MB (219164118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6f42bd7f97fc7f44793c94b471dffae31623b576750d88d218093e9a4836040`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:41:45 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 02:41:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 02:41:46 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 02:52:56 GMT
ENV RUBY_MAJOR=3.1
# Sat, 21 Oct 2023 02:52:57 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 21 Oct 2023 02:52:57 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 21 Oct 2023 02:54:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 02:54:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 02:54:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 02:54:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 02:54:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 02:54:28 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fb291e44c5bae3b8936a1747b64a310dffe6de296c9e6bb5886e9d3e59921c79`  
		Last Modified: Sat, 21 Oct 2023 02:58:56 GMT  
		Size: 4.1 MB (4061501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:25747c219cc4eeb387babcb5293d1f1a80d98749186167441bc4c688d76f87fa`  
		Last Modified: Sat, 21 Oct 2023 02:58:56 GMT  
		Size: 223.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:400128dea6dc4b17af139c13b97dc912fc6f1d4765fa01711c2c2e588348599e`  
		Last Modified: Sat, 21 Oct 2023 03:00:17 GMT  
		Size: 29.3 MB (29339809 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b251245088fd55046650290ffda966cc0d009ac4b6626fa429bbbf5f91a7184b`  
		Last Modified: Sat, 21 Oct 2023 03:00:14 GMT  
		Size: 173.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7548fb4286009b65571d4ec326a39a03b1fe0d2209a6ee1f540692250e2bfc46`  
		Last Modified: Sat, 21 Oct 2023 09:02:02 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2f918c91d2082f01317bfe36256ef7843bb85a80c28f1b096663d0146f2697f1`  
		Last Modified: Sat, 21 Oct 2023 09:02:08 GMT  
		Size: 86.9 MB (86906734 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6533b67667276cc5c579eae5143e6e2d0e050590836ad60033d06f61fa2108f2`  
		Last Modified: Sat, 21 Oct 2023 09:02:03 GMT  
		Size: 134.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d1be79c8a6dfbc136f3e92a3dac1802face1d095447448f95ba97f6c2024a381`  
		Last Modified: Sat, 21 Oct 2023 09:02:03 GMT  
		Size: 124.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:850d0abfe898855e576217615dcbe236d456d88dbdfa642bd3499ddbf3bc72f0`  
		Last Modified: Wed, 29 Nov 2023 06:13:25 GMT  
		Size: 3.2 MB (3236533 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:075bed88e4bf2d2c9fce3fcee79a1d631edb0601fde7b7ce7090c8e47dfa536d`  
		Last Modified: Wed, 29 Nov 2023 06:13:28 GMT  
		Size: 92.3 MB (92283841 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:96969b6597bdde4a286f36497462f70b2549ca8c4b6bda57da836a1067d0a2ca`  
		Last Modified: Wed, 29 Nov 2023 06:13:25 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:b0861dabc109f614d96bde85d1df194c3c7e9560688e2148fa7b9e95fd1c6be7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4598280 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:648091a3349a2cc042d41192dcb883b827190406bb4b7457cfdc51c7fddc6718`

```dockerfile
```

-	Layers:
	-	`sha256:3c72d8746191bc3725434ccd022bc93bd43191e5f9609fa3dff51c7254de424b`  
		Last Modified: Wed, 29 Nov 2023 06:13:25 GMT  
		Size: 4.6 MB (4564093 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:a4aaa2defabc4a7b5f7dbebc851d1f35d269da17129883a3cce98ac273e2c2b8`  
		Last Modified: Wed, 29 Nov 2023 06:13:25 GMT  
		Size: 34.2 KB (34187 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:alpine` - linux; 386

```console
$ docker pull redmine@sha256:f1c05664b3c710ce6e10d13577ab40a5d80d6a0216d87a3fe848ac3b997053bf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.0 MB (193008914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9baa370a5d313f7843050c9dba94a260db4db7b056b774b3719fd3d18e2d6e64`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 30 Sep 2023 08:26:15 GMT
ENV LANG=C.UTF-8
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_MAJOR=3.1
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 30 Sep 2023 08:26:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 30 Sep 2023 08:26:15 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 30 Sep 2023 08:26:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 30 Sep 2023 08:26:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["irb"]
# Sat, 30 Sep 2023 08:26:15 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV RAILS_ENV=production
# Sat, 30 Sep 2023 08:26:15 GMT
WORKDIR /usr/src/redmine
# Sat, 30 Sep 2023 08:26:15 GMT
ENV HOME=/home/redmine
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_VERSION=5.0.6
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.6.tar.gz
# Sat, 30 Sep 2023 08:26:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=488fe08f37a8eb1011415922a8ea743b7f38d8a7a5f8822950a34a375dcf08ee
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Sat, 30 Sep 2023 08:26:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 30 Sep 2023 08:26:15 GMT
COPY docker-entrypoint.sh / # buildkit
# Sat, 30 Sep 2023 08:26:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 30 Sep 2023 08:26:15 GMT
EXPOSE map[3000/tcp:{}]
# Sat, 30 Sep 2023 08:26:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c8e4bf4a2ec6b69fe3700f1259c686d0c2d1fe3c070183216d20e6db2d17598`  
		Last Modified: Sat, 21 Oct 2023 02:01:38 GMT  
		Size: 4.1 MB (4135907 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:75c1944d06f4d0a2ca6ce71cc1c9d7398176a9b1959df9fa6c225f47845de712`  
		Last Modified: Sat, 21 Oct 2023 02:01:36 GMT  
		Size: 225.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cf047c528fbb05b5cccbce89254356fb23b77abc49091cce29502565a2c9e6fc`  
		Last Modified: Sat, 21 Oct 2023 02:03:02 GMT  
		Size: 28.6 MB (28624625 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6d26a2b4a307e1d27296237833d9f1a0b23f2dc865eb42629d89f4f0d4445c0c`  
		Last Modified: Sat, 21 Oct 2023 02:02:58 GMT  
		Size: 175.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:508db4d1122dcffbd8f0815005142a2830eb117e63db4b5ff6f288d4a43567ca`  
		Last Modified: Sat, 21 Oct 2023 03:33:40 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05e5cb86acb71708f51826d4c6706190ded1df5e1e60e8a95aaba7481ef8f302`  
		Last Modified: Sat, 21 Oct 2023 03:33:44 GMT  
		Size: 84.3 MB (84303255 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5bd8bcf2632f9e47ab4a85e0aafdf17be9922e10e7c948504af905692c3598f`  
		Last Modified: Sat, 21 Oct 2023 03:33:40 GMT  
		Size: 135.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:015088bcbbb47a4657a77bd37baea8556ad1d50acd50137e3014a295a83d5358`  
		Last Modified: Sat, 21 Oct 2023 03:33:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b4d417dfa4e0a213fa605e117950458dc0330a3d7892542e54632ca663af8fb`  
		Last Modified: Sat, 21 Oct 2023 03:33:41 GMT  
		Size: 3.1 MB (3147435 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ed5f57d55f70c61e55e4d0414d9c530f8242811756b0ef810499901e25082849`  
		Last Modified: Sat, 21 Oct 2023 03:33:45 GMT  
		Size: 69.6 MB (69558058 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3c2ed9980282f6f93f2eb54ff2182edccd4143c9852cd2ee3173a6cc83e4a8c5`  
		Last Modified: Sat, 21 Oct 2023 03:33:42 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:ac30d280440ea478268089f57f7fcb3349ac19c7bd5bd7a63f31a7490f874103
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.5 KB (34546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e6494e9f0bef6b38f2b44eda359e3301c951d422bf400b3ef20476b1f8c2400`

```dockerfile
```

-	Layers:
	-	`sha256:a663d8fa378de444be9c6fa0e8a0418c3a8f9cf805eb0e040ca88dd5b707a0eb`  
		Last Modified: Sat, 21 Oct 2023 03:33:39 GMT  
		Size: 34.5 KB (34546 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:alpine` - linux; ppc64le

```console
$ docker pull redmine@sha256:c27aaeeb5eab69255155b78ec99538087953fd19ae89a20e13beb13aa1d82443
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.9 MB (228895830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:834ea5edfae8cbc5b3d6ef6658fb55b8e1e97e4c84219ddc877f9d5a99881e14`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:50:53 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 00:50:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 00:50:54 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 01:03:44 GMT
ENV RUBY_MAJOR=3.1
# Sat, 21 Oct 2023 01:03:45 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 21 Oct 2023 01:03:45 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 21 Oct 2023 01:05:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 01:05:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 01:05:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 01:05:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 01:05:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 01:05:47 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3f7e0a6ba1cba9baf57fedfe9893787af1f8d03e2650bf9467dd0d2e61454945`  
		Last Modified: Sat, 21 Oct 2023 01:11:10 GMT  
		Size: 4.3 MB (4279337 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8c62f8560a744c5db39bd64c364f6cffdfaa088cd0a6d421610e6b51fc2b844f`  
		Last Modified: Sat, 21 Oct 2023 01:11:10 GMT  
		Size: 223.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2ea3970f0fd4f1cca730685f4653052c2b638560021d87f1d4a39e5790e6637e`  
		Last Modified: Sat, 21 Oct 2023 01:12:33 GMT  
		Size: 30.1 MB (30060363 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:344ce0314636eb977376f03b3109d1fefaf0c7edeb49828e5962dc4673df9cf3`  
		Last Modified: Sat, 21 Oct 2023 01:12:30 GMT  
		Size: 173.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6277e9c0159711ebad98cd4ba6e67712ba80b42bd21df4d17aa12b87d0e06ae0`  
		Last Modified: Sat, 21 Oct 2023 07:13:20 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f7710e23881be3c65a9f3d08f623b9ce1663e4a02bb39213e842dfc2af0b213e`  
		Last Modified: Sat, 21 Oct 2023 07:13:25 GMT  
		Size: 93.1 MB (93062446 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2eca9a0bc2e4ed19c5b3ba3a2dd14924f4040fbfc4873b1c844466d79e66d77e`  
		Last Modified: Sat, 21 Oct 2023 07:13:21 GMT  
		Size: 134.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15004d9e4ae61ffb0c294ceb03ac035b1e117046bcb7f7f4d7ebf628da7fbb39`  
		Last Modified: Sat, 21 Oct 2023 07:13:21 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:77dbfd12c7b144012ac54633062bd80bf13ba6da50f22738d9715d0d4c363296`  
		Last Modified: Wed, 29 Nov 2023 08:30:35 GMT  
		Size: 3.2 MB (3236512 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3b069a6d20c67612a754e73a0da98fe3df48a984d855279e96df328e19701478`  
		Last Modified: Wed, 29 Nov 2023 08:30:38 GMT  
		Size: 94.9 MB (94906791 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1fc82a26ab76ae65ea372dd0cf157567fc2253e6863d58c2ff93ce206aed2148`  
		Last Modified: Wed, 29 Nov 2023 08:30:34 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:56c2ce5f4ce59f0dd33cba29411f54ef5bf24a431d25d868b281d29f7e7a85c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4603757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dab2066e372dc41aa61f636b817faa13c49a9aa313edf9d770248f179b5074a4`

```dockerfile
```

-	Layers:
	-	`sha256:44e4b090a34d6e2ce6c9bcc3e023992e4090a5b3b034e9780bfc1b8a5d6bdb1e`  
		Last Modified: Wed, 29 Nov 2023 08:30:34 GMT  
		Size: 4.6 MB (4569518 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:91662ddfc44a28e92b9c4aa1a5f3f075a495fe3c5098e8c6bc2b266c395c9d38`  
		Last Modified: Wed, 29 Nov 2023 08:30:34 GMT  
		Size: 34.2 KB (34239 bytes)  
		MIME: application/vnd.in-toto+json

### `redmine:alpine` - linux; s390x

```console
$ docker pull redmine@sha256:29caa9bcbf57db7cbce83336ffd464f307029fb590d8b9cab4f2498f686824af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.5 MB (219486557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eeaf5f08920cd112c6cfef0bc041650187eefb6c8d32d53b50c7bfcb0e3890df`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 00:45:56 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Sat, 21 Oct 2023 00:45:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 21 Oct 2023 00:45:57 GMT
ENV LANG=C.UTF-8
# Sat, 21 Oct 2023 00:57:54 GMT
ENV RUBY_MAJOR=3.1
# Sat, 21 Oct 2023 00:57:54 GMT
ENV RUBY_VERSION=3.1.4
# Sat, 21 Oct 2023 00:57:54 GMT
ENV RUBY_DOWNLOAD_SHA256=1b6d6010e76036c937b9671f4752f065aeca800a6c664f71f6c9a699453af94f
# Sat, 21 Oct 2023 00:59:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 21 Oct 2023 00:59:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 21 Oct 2023 00:59:52 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 21 Oct 2023 00:59:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 21 Oct 2023 00:59:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 1777 "$GEM_HOME"
# Sat, 21 Oct 2023 00:59:53 GMT
CMD ["irb"]
# Mon, 27 Nov 2023 21:32:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		findutils 		su-exec 		tini 		tzdata 		wget 				breezy 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	; # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV RAILS_ENV=production
# Mon, 27 Nov 2023 21:32:27 GMT
WORKDIR /usr/src/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
ENV HOME=/home/redmine
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME" # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_VERSION=5.1.1
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.1.1.tar.gz
# Mon, 27 Nov 2023 21:32:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=edf3095746effd04ad5140681d618f5fa8d06be09c47b6f8b615dcad0b753e6e
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' + # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 27 Nov 2023 21:32:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 27 Nov 2023 21:32:27 GMT
COPY docker-entrypoint.sh / # buildkit
# Mon, 27 Nov 2023 21:32:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 27 Nov 2023 21:32:27 GMT
EXPOSE map[3000/tcp:{}]
# Mon, 27 Nov 2023 21:32:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:72989e5bd2b454111755120583d050e22d64d9535341d940125f64d206481a1b`  
		Last Modified: Sat, 21 Oct 2023 01:06:03 GMT  
		Size: 4.2 MB (4235386 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:46a7f81240913ffe48303f880aae4f2fbe342a31839f2e1879132f9ccc5dd49c`  
		Last Modified: Sat, 21 Oct 2023 01:06:03 GMT  
		Size: 223.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6a34d0a6821ff376a78e9ca1ffcb6a4734ed8ddd212b6d6a077d8c977166416c`  
		Last Modified: Sat, 21 Oct 2023 01:07:17 GMT  
		Size: 29.5 MB (29500471 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06f93aee446f1566155cbe92967d1158de3bb51b42b145554c523fda1ea7a5c1`  
		Last Modified: Sat, 21 Oct 2023 01:07:15 GMT  
		Size: 172.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d35150615162d1b6e3e8c1e9ec618fa328fce2dcc802001da54a0bde09878b25`  
		Last Modified: Sat, 21 Oct 2023 06:08:23 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c527cf43f3736e9470ad2cd21ccb4b9aef09a90eb026c629b26881a3a1c0c8f1`  
		Last Modified: Sat, 21 Oct 2023 06:08:28 GMT  
		Size: 86.8 MB (86828853 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:972beb165701e2eafa4bd30a2666474385d64b3a2ff702220b2dba419bf6af31`  
		Last Modified: Sat, 21 Oct 2023 06:08:23 GMT  
		Size: 136.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fc7409e8c1aff2f53c8dbd54c2cfa3b18cea422e5516eb283d6f1b05aee0af97`  
		Last Modified: Sat, 21 Oct 2023 06:08:24 GMT  
		Size: 126.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:caf1c25439628dd397616c2bb7ffec8eedbeb1888d35bbaedfc7ce19304067a7`  
		Last Modified: Wed, 29 Nov 2023 01:22:24 GMT  
		Size: 3.2 MB (3236489 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:47a7e6be609728e1c268945edf6e222cdafdb5bd4215a039faaddb6b55efa1c5`  
		Last Modified: Wed, 29 Nov 2023 01:22:26 GMT  
		Size: 92.5 MB (92466382 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a56ac2768f1e413dfbda7d659d30359eda5739dd515abf75fc6ad69525cb89f`  
		Last Modified: Wed, 29 Nov 2023 01:22:24 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `redmine:alpine` - unknown; unknown

```console
$ docker pull redmine@sha256:dcb154955701caacbb237c43b1c95cc25291b74937b829a4ea3f3cc040335337
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4603542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d17e414430e05f9f23ef74b9d4673652b6c1199f894e8d5ae42c0cc51a5a2c2`

```dockerfile
```

-	Layers:
	-	`sha256:6d047cbfaab60cccd3618bb112784747399e93e7dc07d85a0c9ff65e9649de13`  
		Last Modified: Wed, 29 Nov 2023 01:22:23 GMT  
		Size: 4.6 MB (4569373 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:49c407e8e7c500e83060bd4dba0a6d76e158c259644a544cc7514ac392f36406`  
		Last Modified: Wed, 29 Nov 2023 01:22:23 GMT  
		Size: 34.2 KB (34169 bytes)  
		MIME: application/vnd.in-toto+json
