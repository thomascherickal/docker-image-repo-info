<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `redmine`

-	[`redmine:4`](#redmine4)
-	[`redmine:4-alpine`](#redmine4-alpine)
-	[`redmine:4-passenger`](#redmine4-passenger)
-	[`redmine:4.0`](#redmine40)
-	[`redmine:4.0-alpine`](#redmine40-alpine)
-	[`redmine:4.0-passenger`](#redmine40-passenger)
-	[`redmine:4.0.9`](#redmine409)
-	[`redmine:4.0.9-alpine`](#redmine409-alpine)
-	[`redmine:4.0.9-passenger`](#redmine409-passenger)
-	[`redmine:4.1`](#redmine41)
-	[`redmine:4.1-alpine`](#redmine41-alpine)
-	[`redmine:4.1-passenger`](#redmine41-passenger)
-	[`redmine:4.1.3`](#redmine413)
-	[`redmine:4.1.3-alpine`](#redmine413-alpine)
-	[`redmine:4.1.3-passenger`](#redmine413-passenger)
-	[`redmine:4.2`](#redmine42)
-	[`redmine:4.2-alpine`](#redmine42-alpine)
-	[`redmine:4.2-passenger`](#redmine42-passenger)
-	[`redmine:4.2.1`](#redmine421)
-	[`redmine:4.2.1-alpine`](#redmine421-alpine)
-	[`redmine:4.2.1-passenger`](#redmine421-passenger)
-	[`redmine:alpine`](#redminealpine)
-	[`redmine:latest`](#redminelatest)
-	[`redmine:passenger`](#redminepassenger)

## `redmine:4`

```console
$ docker pull redmine@sha256:cae6a4d4227606764c6a75b180a5b675e4d7415888b5a1261069761a7cd84eac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4` - linux; amd64

```console
$ docker pull redmine@sha256:c303bc0f5596613dabea4516d47172296178fa21f6db17497624805f778cb357
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195475758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:338c47d4bca896733efe021ec38c0d595cf043de470eba5e45d6e3dde1a485c3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:504785f157b11fc0cf462141bdae1564241f3417ea1c8371d3c2e4c7dd41c552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196972163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217c8956d29925ec9e63ffbf48e3d04a71ec25911566cd968e65a03abbcef198`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:06:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:06:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:17:20 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:05:54 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:05:55 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:19:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:19:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:20:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:20:00 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:20:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:20:03 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:32:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:33:44 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:33:45 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:33:45 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:33:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:33:48 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 22:33:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 22:33:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:39:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:39:30 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:39:30 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:39:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:39:32 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:39:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b3ba0f03212caacd2191837bdac2f1a9abf399938b4020b315e4c6ea7ba0c7`  
		Last Modified: Wed, 23 Jun 2021 14:05:28 GMT  
		Size: 10.3 MB (10345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfab7796870f80c9db896239384ac194808f4ce5fab9f16ba155559772cc1e`  
		Last Modified: Wed, 23 Jun 2021 14:05:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4340642939f48d099081c75a2712db898b9985ae54a619b2452aac1d6d5811`  
		Last Modified: Thu, 08 Jul 2021 20:43:39 GMT  
		Size: 13.9 MB (13871335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695fcd3bc334ffbc54deec488d9db9eda8fec160e0a45fb2eaf1cb3c40fe5d17`  
		Last Modified: Thu, 08 Jul 2021 20:43:31 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e84c1768026dd91ab7c8b588e6bca6eb786ae29dbdbcb5cfe9942272bcfc56b`  
		Last Modified: Thu, 08 Jul 2021 22:55:15 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7075123429263b675529579bcba18589d90fc77e59eb5919484dedb6d1c64c1f`  
		Last Modified: Thu, 08 Jul 2021 22:56:17 GMT  
		Size: 89.6 MB (89576320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e64c6c915303586fcbdb5e1921c304efd17cae07d4aabc1d6ebae70a889fd8`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b203953be51a5b5e20215561ddbcf8db375b9ca69dd0f7ba4d114fa962f6d7d`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ac40a10c440649c65c501f24a90d153143ce98bcf9b9bf731f6e22a347570`  
		Last Modified: Thu, 08 Jul 2021 22:55:17 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14230d92bd82d511c4f7398fd0d256fb2c88bc9039691884c1a0a90a6b9b7d56`  
		Last Modified: Thu, 08 Jul 2021 22:55:35 GMT  
		Size: 55.2 MB (55236836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eea4df7ac799e61a3b26a4195f6641617e2e656b4b38cd6c47240821584be3`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:918c928c44808884e8f314ba4798c35f6c33f66f3af9808185b7cb6632829c4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4523ba6f474f4b705844d9e15d89345a8277bfdbf939337c277171f2733bc896`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 23:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 23:18:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 23:18:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 23:36:25 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 23:43:24 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 23:43:24 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:35:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:35:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:35:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:35:12 GMT
CMD ["irb"]
# Fri, 09 Jul 2021 04:06:25 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 09 Jul 2021 04:07:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 04:07:27 GMT
ENV RAILS_ENV=production
# Fri, 09 Jul 2021 04:07:27 GMT
WORKDIR /usr/src/redmine
# Fri, 09 Jul 2021 04:07:28 GMT
ENV HOME=/home/redmine
# Fri, 09 Jul 2021 04:07:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 09 Jul 2021 04:07:30 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 09 Jul 2021 04:07:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 09 Jul 2021 04:07:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 09 Jul 2021 04:12:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 09 Jul 2021 04:12:52 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 09 Jul 2021 04:12:53 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 09 Jul 2021 04:12:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 09 Jul 2021 04:12:54 GMT
EXPOSE 3000
# Fri, 09 Jul 2021 04:12:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b763290fb30bc16e505b4aa06ba1c3041182ac9bd8be48df5e94cbbe8545d`  
		Last Modified: Thu, 24 Jun 2021 00:49:52 GMT  
		Size: 9.9 MB (9872206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f611d0cebec7d01271526d00ff39f508174641d4e952ac4954fb89f368bf331`  
		Last Modified: Thu, 24 Jun 2021 00:49:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c081e6813d08a36724de201912dcf2049b4b63e901379b09265fff1f204332`  
		Last Modified: Thu, 08 Jul 2021 23:20:14 GMT  
		Size: 13.8 MB (13766804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47e03b2ecd26a74249ee57a56b50a959f58fbcaca622b530a671eca71a7384d`  
		Last Modified: Thu, 08 Jul 2021 23:20:07 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5ad0520989f495616ff11a4e507a10e68c9135a8387cf52dfca8fefd1fa348`  
		Last Modified: Fri, 09 Jul 2021 04:27:36 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23a4b1761119307dc0dd899befff1a28684d45a780a3b964aef62e5ea8c5147`  
		Last Modified: Fri, 09 Jul 2021 04:28:33 GMT  
		Size: 85.6 MB (85590504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089aa8086891a0e5b87d68a89f8621e084085b5786ee8e0c05539a337161a184`  
		Last Modified: Fri, 09 Jul 2021 04:27:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57d7596e26caaeafa01d35cfbd470f7a013b174e7c5c25852729c10b10448c`  
		Last Modified: Fri, 09 Jul 2021 04:27:33 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2efb117cd99001cc83a98b5a1277459f26c1b985c59ae03866ca74c7d1380`  
		Last Modified: Fri, 09 Jul 2021 04:27:38 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ab3b3250933a12c6c93d662c3198824bef82b64f0d7f119675b68e1cec76a6`  
		Last Modified: Fri, 09 Jul 2021 04:27:59 GMT  
		Size: 55.1 MB (55076972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3916fdc65621036c0f5ddd98394f1e47796b2f19531e4ab24c86648449214c16`  
		Last Modified: Fri, 09 Jul 2021 04:27:33 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:0741f6999c4d2a4e13afe1af9a34785c48f61a2feb89930198909593b569e246
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203231922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3d2c5023b434e055c0449d22553bc2ecc42a9e53a462c79fada428177c6180`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:53:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 03:53:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 03:53:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 03:58:54 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 23:45:12 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 23:45:13 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:45:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:45:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:45:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:45:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:45:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:45:29 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 23:21:02 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 23:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 23:21:24 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 23:21:25 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 23:21:25 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 23:21:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 23:21:26 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 23:21:26 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 23:21:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 23:23:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 23:23:52 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 23:23:53 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 23:23:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 23:23:53 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 23:23:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f276f053f0cad4dbf0c339099f5dd135531eb3ffb0bccc09369e7b7391b18d72`  
		Last Modified: Wed, 23 Jun 2021 04:22:18 GMT  
		Size: 11.3 MB (11263062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863be1d4664c690cf3e71cf9494c9b590ce4781e8008aef05d7cf572b8feddcc`  
		Last Modified: Wed, 23 Jun 2021 04:22:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f5d2c58688ac84743d00ab7bbdc6b4093e20d9a833d6af3496cc62e935a25`  
		Last Modified: Thu, 08 Jul 2021 21:09:46 GMT  
		Size: 14.4 MB (14356604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4dfdc14b449c213e94db8cd01bdfa232be4fa72040ffeebb4ea881ffa8634`  
		Last Modified: Thu, 08 Jul 2021 21:09:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df641efdceaa2aee736b0b2ed3580d9cc12941e9d5b47754238e2832b4290d`  
		Last Modified: Thu, 08 Jul 2021 23:29:47 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e08f5ce73ad17307002bfba119f4a63a0edae9959555829f15c37ec8f76c2`  
		Last Modified: Thu, 08 Jul 2021 23:30:04 GMT  
		Size: 92.6 MB (92610656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4765b269f180b2c2704772dd7d776ea01a9075ed5d1d8cd8f0882ca083129c2c`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6329e48a16d3a91d290cfbae3c0a552cfe96c6b792fcb231df35ff3c039a1`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feadd8be638a909710f31206aa67f01ca6d2a8ebec560b39b0dc3523c0211f6`  
		Last Modified: Thu, 08 Jul 2021 23:29:46 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5a01cee6465420071dfb449649aebee78fb947eecd0b3b279df2405c1c4d9d`  
		Last Modified: Thu, 08 Jul 2021 23:29:51 GMT  
		Size: 56.0 MB (56023674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbbcb4d6ad95bc21ed907d86fa7e683a21628ed441ad64f891f7322fc156b12`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; 386

```console
$ docker pull redmine@sha256:38c75a4b236bb825b9ee8fa35034d33dab94661ce6f8ce26c59869e809aa60ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202116586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cab517b8b53a6715a276de085b7d54ac6b3054ed3ee985c2ec4022d275a36e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:33:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:33:25 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:42:41 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:08:54 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:08:54 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:01:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:01:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:01:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:01:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:01:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:01:08 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:46:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:47:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:47:20 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:47:20 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:47:20 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:47:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:47:21 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 22:47:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 22:47:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:48:13 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:48:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:48:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:48:14 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:48:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb2041b26a9335dbdc8e6cc9bd945661b43317eb0de6d4e1e8ce82275cbea6`  
		Last Modified: Wed, 23 Jun 2021 14:14:04 GMT  
		Size: 17.2 MB (17227420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c89206098d37979fca1f31ba315796953128b80660adc5194c5541f0ac3f34`  
		Last Modified: Wed, 23 Jun 2021 14:13:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce027bc021a8f988e98283d7e7edb0812da70bec1469306b760a90237fb460ac`  
		Last Modified: Thu, 08 Jul 2021 20:34:09 GMT  
		Size: 14.0 MB (13991996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f914d412069980e7e91c9e3b27cd62e1d17cffdd9dd8b8d86e009a47a54d257`  
		Last Modified: Thu, 08 Jul 2021 20:34:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ddcca7d90497767f04b499a232298ba4b6b367a55fc644281d45884b4904c4`  
		Last Modified: Thu, 08 Jul 2021 22:53:29 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a07456067d7c014c80d85bba6d608010bf9baaa1cbf62bfefc070f9e197d5`  
		Last Modified: Thu, 08 Jul 2021 22:53:53 GMT  
		Size: 95.7 MB (95703052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b637a32b9c8c0c921586600afc7d5867c46a31465bbb953d9f07412725c8f280`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe31a7355aa80ea3975b5e2ea081a34279b494c8636489851f5bb2adabbb9ba9`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc4f8125c232b162083e88887968149ff3e94b419b661c0c98ab1c249ae8e82`  
		Last Modified: Thu, 08 Jul 2021 22:53:28 GMT  
		Size: 3.1 MB (3058670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c938aebe09af0b44a41d919513d737720f30afcb71bcdfe7ff6ed289be406cdb`  
		Last Modified: Thu, 08 Jul 2021 22:53:34 GMT  
		Size: 44.3 MB (44333801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2250ccc831a8ba36b5f9238e570ea872df977ed50651174c22510dcdc699d`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; ppc64le

```console
$ docker pull redmine@sha256:8fb1ccf561c68fe89d8bcbae5ff084cf0abd84fd2363b4ec1789794b2dbc7a31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219629876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5d606a69ac811e24028853731ce3876c2081c9926124809b5369c40d3e38d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 17:21:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 17:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Jul 2021 17:22:32 GMT
ENV LANG=C.UTF-8
# Sat, 10 Jul 2021 17:45:35 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Jul 2021 17:45:38 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 10 Jul 2021 17:45:45 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 10 Jul 2021 17:57:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Jul 2021 17:57:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Jul 2021 17:57:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Jul 2021 17:57:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Jul 2021 17:57:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Jul 2021 17:57:59 GMT
CMD ["irb"]
# Sun, 11 Jul 2021 07:19:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Jul 2021 07:27:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 07:27:27 GMT
ENV RAILS_ENV=production
# Sun, 11 Jul 2021 07:27:31 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Jul 2021 07:27:38 GMT
ENV HOME=/home/redmine
# Sun, 11 Jul 2021 07:27:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Jul 2021 07:27:56 GMT
ENV REDMINE_VERSION=4.2.1
# Sun, 11 Jul 2021 07:27:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Sun, 11 Jul 2021 07:28:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Jul 2021 07:35:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Jul 2021 07:35:26 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Jul 2021 07:35:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Jul 2021 07:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Jul 2021 07:35:45 GMT
EXPOSE 3000
# Sun, 11 Jul 2021 07:35:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba063dbcdd8aa55ec2183194edae6ea424d440c8c3c4ab57e29bdc8d30739f`  
		Last Modified: Sat, 10 Jul 2021 18:24:25 GMT  
		Size: 12.7 MB (12704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302bed40ec71d6898df63835eb0d9463b4672fcb74c6d77594621b1a9d96089b`  
		Last Modified: Sat, 10 Jul 2021 18:24:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d142b79f0a553ffa66e8c2525798e544895249d98562aa21710905ebcdc6ed`  
		Last Modified: Sat, 10 Jul 2021 18:25:40 GMT  
		Size: 15.0 MB (14997790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3641aa4022fa299e9c8ba11982ead0ef3ba6b4e176be30a9d1f232615c99c`  
		Last Modified: Sat, 10 Jul 2021 18:25:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4804b39acc72bb6d81a7bfc7c05f56e803d5b3e9d2ed1c298bbd2eb44c7e5356`  
		Last Modified: Sun, 11 Jul 2021 08:15:25 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9073dd583be35eadb9e9e25a07f78b0a111fca6d47e69f14431eeb4b81f0682a`  
		Last Modified: Sun, 11 Jul 2021 08:15:45 GMT  
		Size: 101.3 MB (101327909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae14e6cdfd8bc5a68ed3c6f67843101b5677d40266ab29f2da8d3c24724ad20`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346cf33cfa1c3ae728b01723b2eacfc89d22db906bbb468ad356ffe6f80188b8`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4551ad703a6bab86fb1132fc6ecfd00620f4079d4d10d5c9d3f6b78a66d698a0`  
		Last Modified: Sun, 11 Jul 2021 08:15:22 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f790f7d0d86286c2d1129fa246d6eb23d09db45923ec78d8d0e2402cfd8660`  
		Last Modified: Sun, 11 Jul 2021 08:15:30 GMT  
		Size: 57.0 MB (56983237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dff610884a2816b07cde2af44a25989e11404807fe565fed2cee5ba172a03bc`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; s390x

```console
$ docker pull redmine@sha256:73d6f4443ca8fb63dbad4f2d16c45bd208f75b21472cd8dd96cc1307bd1e2773
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202549125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f90d1267f56ffe9dd1410a3837ccbf93c9da343fe9ff0a822248352eaeb441`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:56:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:56:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 09 Jul 2021 03:56:46 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jul 2021 04:10:42 GMT
ENV RUBY_MAJOR=2.7
# Fri, 09 Jul 2021 04:10:43 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 09 Jul 2021 04:10:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 09 Jul 2021 04:13:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 09 Jul 2021 04:13:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 09 Jul 2021 04:13:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 09 Jul 2021 04:13:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Jul 2021 04:13:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 09 Jul 2021 04:13:29 GMT
CMD ["irb"]
# Sat, 10 Jul 2021 03:58:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Jul 2021 03:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 03:59:51 GMT
ENV RAILS_ENV=production
# Sat, 10 Jul 2021 03:59:51 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Jul 2021 03:59:52 GMT
ENV HOME=/home/redmine
# Sat, 10 Jul 2021 03:59:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Jul 2021 03:59:54 GMT
ENV REDMINE_VERSION=4.2.1
# Sat, 10 Jul 2021 03:59:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Sat, 10 Jul 2021 04:00:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Jul 2021 04:03:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Jul 2021 04:03:24 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Jul 2021 04:03:25 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Jul 2021 04:03:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Jul 2021 04:03:26 GMT
EXPOSE 3000
# Sat, 10 Jul 2021 04:03:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb0861b7843d74cdcb468db372740a5fbb65d1a7a489cd207e57603e23b308`  
		Last Modified: Fri, 09 Jul 2021 04:33:35 GMT  
		Size: 10.8 MB (10814494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b9cde22299f5aa53f8d9540f770e1b6ab0e6223d1d106df86a5a071f8f3ec`  
		Last Modified: Fri, 09 Jul 2021 04:33:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf70f667dcd7c81ea6676bf03ad1d287575af1b2eceb425583be290e010897d`  
		Last Modified: Fri, 09 Jul 2021 04:34:14 GMT  
		Size: 14.7 MB (14697234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db437741211099211d57153dd52a63267f0affc47f39380dcd6da3552b8d5d5`  
		Last Modified: Fri, 09 Jul 2021 04:34:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a890c47c8baf9911890e19680c177f40232d060ba3cb040b2769a783f1ef98`  
		Last Modified: Sat, 10 Jul 2021 04:14:43 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95693198ef1207b35d9efaf8262d24914419aa240f3df8e04fc6369e5dcb55d8`  
		Last Modified: Sat, 10 Jul 2021 04:14:57 GMT  
		Size: 91.8 MB (91789992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5150ba28aa600261d40392db78998b0639dce33fa135a4749a3e03046b57ab38`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6faf8f4361902faa3aab0a419eeb7f8819ad29e5e3daf830099ed96210ec9fe`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472586cc07848d25dd2f1f9438ec666dc78b643ede7d89344b5da229b412a5c3`  
		Last Modified: Sat, 10 Jul 2021 04:14:42 GMT  
		Size: 3.1 MB (3058671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384911646e488885a18a1fc8217f5f547cde94a5281986d7b69f117e363381ea`  
		Last Modified: Sat, 10 Jul 2021 04:14:46 GMT  
		Size: 56.4 MB (56423763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051ac5465ae61ddb401a283b21e69175949f1424f30cea6aa203408b2ea9c214`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:7de4015773da4d105b5f43705556003eb3071d781612fa6e7f6010981e4e56e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:7fb14bb9edbf56cf78406c149b3015cfd560d8ab4b036edebde5aa5e4b83f5af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150068908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74c717ce35a7872383b67fe6276f951c39395fcba0eda36625d7e2eaa9a32932`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 08 Jul 2021 21:57:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 08 Jul 2021 21:57:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 08 Jul 2021 21:57:30 GMT
ENV LANG=C.UTF-8
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_MAJOR=2.7
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:18:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:18:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:18:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:18:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:18:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:18:51 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:22:24 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jul 2021 20:22:32 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 14 Jul 2021 20:22:33 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:22:33 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:22:33 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:22:34 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:22:35 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:22:35 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:22:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:22:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jul 2021 20:24:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jul 2021 20:24:42 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:24:42 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 14 Jul 2021 20:24:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:24:42 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:24:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b0ea69e9ed42c49b5af449b703a12a4d2f2e28d87905af6fcd903fdae5689`  
		Last Modified: Thu, 08 Jul 2021 22:38:46 GMT  
		Size: 3.6 MB (3581658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad656ed833315b61ea674706f32c2d18d7412c7120926442af57b9131ee72ee`  
		Last Modified: Thu, 08 Jul 2021 22:38:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626f6830afc6fb7a05a8f18f2b98e4ea4db3d2dd50803e5cd2c627fe25150dc8`  
		Last Modified: Thu, 08 Jul 2021 22:40:13 GMT  
		Size: 14.4 MB (14373123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5375389679c9573d241b22905aee17b20981e2628989561698087f107fcfed4a`  
		Last Modified: Thu, 08 Jul 2021 22:40:11 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76a82132aeb154f32b80803eecedc3e27e062a35ae1e05284dc2d7e6c7f4f59`  
		Last Modified: Wed, 14 Jul 2021 20:35:42 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb4af997128346f54fa569d3a04180c718e02a90e90eff7161241d54deef92`  
		Last Modified: Wed, 14 Jul 2021 20:35:52 GMT  
		Size: 69.5 MB (69526214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14da2816c58ef08b826f823d7b6a4126bb63594ed1109880b795c28cc4d3f032`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f34be07349b94807cc58a0e31cecec279d0591b9a6f1f65f1dbe94a4713462`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b05ead31106734fcef5216d256a8536461fa7935f729e67262c90f55e683b`  
		Last Modified: Wed, 14 Jul 2021 20:35:40 GMT  
		Size: 3.1 MB (3060004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c586852175065725ae48c5682f1ecea003599fbc0028c3387f5de00cc28f34`  
		Last Modified: Wed, 14 Jul 2021 20:36:03 GMT  
		Size: 56.7 MB (56712212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d1559a239e3bf1260f693961d40d28b32673907100b077a797e55d543f072c`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:9b780f98151823e0e84e1e41974c548143cae7090cd367eb711d44d3bc8a966b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:a320947c8461cd8bafad0bcfda90b4f5ac840389345003324df81de7b46ad296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3049f679e04c98a7643e800733c59f85c960a686a186192d9b12a222bed1592`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:22:01 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:22:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:22:20 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:22:20 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:22:20 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41f4f9e9b7629be3e6e9666279b940b489648484da4e41725e7b22c1c94b1b`  
		Last Modified: Wed, 14 Jul 2021 20:35:22 GMT  
		Size: 21.1 MB (21131700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436698f0e4aec6d6e7c991fd623ae0d4eab48e62193c564b2fa25de8f4a52e`  
		Last Modified: Wed, 14 Jul 2021 20:35:20 GMT  
		Size: 4.9 MB (4919284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0`

```console
$ docker pull redmine@sha256:5fe2bfa25e09380eb390b7cca4ad0af896d83a3224478b8ff0855871a724fe9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.0` - linux; amd64

```console
$ docker pull redmine@sha256:120d31ad80c1785e72a46398a061a612987797e4607a61e60010181de0caac33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205071171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf0b146af85cd11c523db51af33d174d5049495a32f1df271250cf823400a93e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:20:10 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:55:24 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:55:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:24:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:24:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:24:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:24:36 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:24:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:29:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:29:28 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:29:28 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:29:31 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:29:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:29:40 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 14 Jul 2021 20:29:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 14 Jul 2021 20:29:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:31:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:31:47 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:31:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:31:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:31:47 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:31:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b95c16c5624058c7516ccc9aff7fcb6ab05fd66e5e47c1228f4d1e8fec58b`  
		Last Modified: Thu, 08 Jul 2021 22:40:47 GMT  
		Size: 21.5 MB (21468025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596bd4a64fddd48add80e9f5ee6459a223843aacedfe89c777ed62847e9b45e`  
		Last Modified: Thu, 08 Jul 2021 22:40:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7eae1b0e301a4bb2e1dc9e8faf695f6a25c25fa76af391234a420401b27365`  
		Last Modified: Wed, 14 Jul 2021 20:36:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78eac6959ab00aa4aa16a8572577047e837cde31b8059a7c473709c1c5fd95a`  
		Last Modified: Wed, 14 Jul 2021 20:37:43 GMT  
		Size: 81.2 MB (81199589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770efe9534a041a263a97329ebea752bf15837faebf99a49e25457e40096ab17`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b58267e8ed59b94a5001480fd1362e24ec0054ae01393052c4782b412399d79`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedb8a1056b6d5f7546123709ccb9fbd52ff2e4f560bff5926c130bb0237afe`  
		Last Modified: Wed, 14 Jul 2021 20:37:29 GMT  
		Size: 2.5 MB (2542552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e80e9679392005f7d3a99eba067dbd5717479b70d7e761d843367213982dd2d`  
		Last Modified: Wed, 14 Jul 2021 20:37:36 GMT  
		Size: 60.1 MB (60148220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44914decf48cf9c7f0dce9ec00797c7f2f371ce9caf3d32730543bde7a11d036`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:17a8885564295f128c7732f2555b316d46a0843508087a8ce3c6be84ca49e3e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194719064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84172a34f45f4e36fa6b29923eeb581145a6663c127b0aa0e40b565893379040`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:06:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:06:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:26:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:16:44 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:16:45 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:28:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:29:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:29:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:29:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:29:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:29:03 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:39:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:48:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:48:03 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:48:03 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:48:04 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:48:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:48:06 GMT
ENV REDMINE_VERSION=4.0.9
# Thu, 08 Jul 2021 22:48:07 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Thu, 08 Jul 2021 22:48:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:54:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:54:19 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:54:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:54:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:54:21 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:54:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b3ba0f03212caacd2191837bdac2f1a9abf399938b4020b315e4c6ea7ba0c7`  
		Last Modified: Wed, 23 Jun 2021 14:05:28 GMT  
		Size: 10.3 MB (10345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfab7796870f80c9db896239384ac194808f4ce5fab9f16ba155559772cc1e`  
		Last Modified: Wed, 23 Jun 2021 14:05:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7534381e53bd89c246e0ccb2c35dac17bf88c731c8d0526c63e59be51e884c`  
		Last Modified: Thu, 08 Jul 2021 20:44:48 GMT  
		Size: 20.7 MB (20733354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f2a9ffe5b789dd841f07056ea0122491118e78120d0f014d80085c602ab19c`  
		Last Modified: Thu, 08 Jul 2021 20:44:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f907c18a99e2058cc185b62d06d2138efee18b95ce1a7a7cdb625a9f526d704`  
		Last Modified: Thu, 08 Jul 2021 22:56:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427196abb69a09f982b2b40fc3aaee3149f18cc32fa0eb59adf1b3e0f59efc47`  
		Last Modified: Thu, 08 Jul 2021 22:58:49 GMT  
		Size: 77.0 MB (76964657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ba7f018f81bc6c5e5a731b53765bcf148ab61d69e2884d0f9db1916bc8c74f`  
		Last Modified: Thu, 08 Jul 2021 22:57:58 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a62c8bc56da5384f26702c4e2b1afd20300d71a66a1c4613269d37bea1ed57`  
		Last Modified: Thu, 08 Jul 2021 22:57:58 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73596d5468e7e314bb8a661c8b46d7ae0285ff4faafdafb34c52419586231d2`  
		Last Modified: Thu, 08 Jul 2021 22:58:01 GMT  
		Size: 2.5 MB (2542548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27219bf2f048f277b05340b2c3968fb9c540542538281e1212a66176c3be0f25`  
		Last Modified: Thu, 08 Jul 2021 22:58:24 GMT  
		Size: 59.2 MB (59249510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4a58a4863a312e6d1b986cd4fd92c4de0d610ba97f6d5cd9b7abd15a8ad506`  
		Last Modified: Thu, 08 Jul 2021 22:57:58 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:1c0cce8f64fd6b3b96ab6e68a14a180e928cf7e9f2b33f324fbf0d2a395db63d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.1 MB (188054222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb6a3f75a9c20d8ef76079aeafeefab6a6b42cdaa2c435cc08a1d41689ba68e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 23:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 23:18:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 23:18:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 23:58:55 GMT
ENV RUBY_MAJOR=2.6
# Thu, 08 Jul 2021 00:04:37 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 08 Jul 2021 00:04:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:55:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:56:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:56:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:56:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:56:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:56:03 GMT
CMD ["irb"]
# Fri, 09 Jul 2021 04:13:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 09 Jul 2021 04:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 04:20:59 GMT
ENV RAILS_ENV=production
# Fri, 09 Jul 2021 04:21:00 GMT
WORKDIR /usr/src/redmine
# Fri, 09 Jul 2021 04:21:00 GMT
ENV HOME=/home/redmine
# Fri, 09 Jul 2021 04:21:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 09 Jul 2021 04:21:02 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 09 Jul 2021 04:21:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 09 Jul 2021 04:21:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 09 Jul 2021 04:26:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 09 Jul 2021 04:26:42 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 09 Jul 2021 04:26:42 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 09 Jul 2021 04:26:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 09 Jul 2021 04:26:43 GMT
EXPOSE 3000
# Fri, 09 Jul 2021 04:26:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b763290fb30bc16e505b4aa06ba1c3041182ac9bd8be48df5e94cbbe8545d`  
		Last Modified: Thu, 24 Jun 2021 00:49:52 GMT  
		Size: 9.9 MB (9872206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f611d0cebec7d01271526d00ff39f508174641d4e952ac4954fb89f368bf331`  
		Last Modified: Thu, 24 Jun 2021 00:49:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae3ab28fbce4cee595eb301139ed362bf539fc80d87e1203e0c2d53b9f30bd5`  
		Last Modified: Thu, 08 Jul 2021 23:21:22 GMT  
		Size: 20.6 MB (20643638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7253813058a0314e3fee8530b64e5f281a4697fd64c8d4f59d4d3c1e02f8b2`  
		Last Modified: Thu, 08 Jul 2021 23:21:13 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859eb1b9e2938ba6951e9b38fb78acaaa4383e0570cc02e2b62523694adf9dd`  
		Last Modified: Fri, 09 Jul 2021 04:28:57 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794ae46d21df62604127bd189cd0a68e3a88763dadf737e0353b247abedd16`  
		Last Modified: Fri, 09 Jul 2021 04:30:57 GMT  
		Size: 73.3 MB (73263930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfdd2c943ba8f6d6b1e1182cff35304fde92f76b3d398e9855ae2d9a885be1c`  
		Last Modified: Fri, 09 Jul 2021 04:30:08 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c48da2fb539ae9e73bfe86bfb185700093eb6d9793684b3ccb056e4a010e92f`  
		Last Modified: Fri, 09 Jul 2021 04:30:07 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d677deceea98b9187e223d9dfc234d8feec7032981da6731f644c03d58dc3518`  
		Last Modified: Fri, 09 Jul 2021 04:30:11 GMT  
		Size: 2.5 MB (2542534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b6c5c3bf2a5ab9c579a9d38b983fe6c9517016607fbd20230a9f6b1584aa72`  
		Last Modified: Fri, 09 Jul 2021 04:30:36 GMT  
		Size: 59.0 MB (58981614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4193fc56acb7aa51eeb30bee783268a00c2619bf1c6d9f1bdb5d739af105aea5`  
		Last Modified: Fri, 09 Jul 2021 04:30:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:0c0e8b2d97e492e291132c465b661ae141feb280bc050ba4c0173ad03bddd75d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200854434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c7e8511810a20ae664d07c2359a8ade45c9ff69408190776fe87267be6cfc8f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:53:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 03:53:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 03:53:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 04:03:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 23:54:15 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 23:54:15 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:55:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:55:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:55:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:55:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:55:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:55:12 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 23:24:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 23:27:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 23:27:01 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 23:27:01 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 23:27:02 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 23:27:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 23:27:03 GMT
ENV REDMINE_VERSION=4.0.9
# Thu, 08 Jul 2021 23:27:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Thu, 08 Jul 2021 23:27:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 23:29:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 23:29:15 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 23:29:16 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 23:29:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 23:29:16 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 23:29:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f276f053f0cad4dbf0c339099f5dd135531eb3ffb0bccc09369e7b7391b18d72`  
		Last Modified: Wed, 23 Jun 2021 04:22:18 GMT  
		Size: 11.3 MB (11263062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863be1d4664c690cf3e71cf9494c9b590ce4781e8008aef05d7cf572b8feddcc`  
		Last Modified: Wed, 23 Jun 2021 04:22:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66415307302b8ab292b3121af7b08354a3b8cdd3da935a6974c5a72434402d`  
		Last Modified: Thu, 08 Jul 2021 21:11:22 GMT  
		Size: 21.3 MB (21308810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a6b4a9d9bdbee57547a94063ad97358687fa8c834f32ae69bdbda7e30ae7f2`  
		Last Modified: Thu, 08 Jul 2021 21:11:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b848da2b7d2dc611df6b3a0f97805a3f84f9a37d2ed4c64297b3c6a599ff29`  
		Last Modified: Thu, 08 Jul 2021 23:30:27 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283276534280ca7488eedab69691a578f9a4ab1e4bce92240e245fbf2b9fe7ca`  
		Last Modified: Thu, 08 Jul 2021 23:31:12 GMT  
		Size: 79.7 MB (79748058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0a20be3baf759cd4cc371136a92a761149dd3c795690e2e6bdcf67f00888e7`  
		Last Modified: Thu, 08 Jul 2021 23:30:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972a54e8e5be6a20e8afe2b2e213c717c70d145fa74301e47e525f97563e1ce6`  
		Last Modified: Thu, 08 Jul 2021 23:30:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da864d531e7092cb89dbf5aabad1503412d5ac4c443fa1b5c4392744b50a70`  
		Last Modified: Thu, 08 Jul 2021 23:30:56 GMT  
		Size: 2.5 MB (2542540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca5c55431781c4f9dc46e8e8c53d75bf6efdc54619f5e95787fa8f1338e932`  
		Last Modified: Thu, 08 Jul 2021 23:31:04 GMT  
		Size: 60.1 MB (60072722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7248a81acf81289f5e57cfc3658039b397fc876cf5b00e3c9339ea40a81997`  
		Last Modified: Thu, 08 Jul 2021 23:30:56 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; 386

```console
$ docker pull redmine@sha256:6a735b9b38729e67ecb9451ec658599d54738dd5acbeab2717922b864ba2122d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210332609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85f6591bcbd03cdbb849f6b3019e8afa5b648253bf3ae262dd6236f22c109f26`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:33:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:33:25 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:49:20 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:19:42 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:19:42 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:13:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:13:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:13:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:13:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:13:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:13:41 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:48:29 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:50:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:50:37 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:50:37 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:50:38 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:50:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:50:39 GMT
ENV REDMINE_VERSION=4.0.9
# Thu, 08 Jul 2021 22:50:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Thu, 08 Jul 2021 22:50:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:52:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:52:59 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:53:00 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:53:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:53:00 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:53:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb2041b26a9335dbdc8e6cc9bd945661b43317eb0de6d4e1e8ce82275cbea6`  
		Last Modified: Wed, 23 Jun 2021 14:14:04 GMT  
		Size: 17.2 MB (17227420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c89206098d37979fca1f31ba315796953128b80660adc5194c5541f0ac3f34`  
		Last Modified: Wed, 23 Jun 2021 14:13:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207bc054547d2959d625941a3d713cbac274d3fde559874ce3f103742021fcd0`  
		Last Modified: Thu, 08 Jul 2021 20:36:03 GMT  
		Size: 20.9 MB (20910220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bf234722053e694517615663f536b0761cb76a5ba09b68a3c42f05280985c5`  
		Last Modified: Thu, 08 Jul 2021 20:35:59 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddd76acb28134714ff2ba2109219219a0b06c2f49c2942ba8183f19f18dc444`  
		Last Modified: Thu, 08 Jul 2021 22:54:17 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40a50be1fee54ea805936c3a1d6352f729af0b25d2c7062bb99d7cc5d019042`  
		Last Modified: Thu, 08 Jul 2021 22:55:15 GMT  
		Size: 82.6 MB (82599861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743ddacf24e24c15e5268f42cbb34701c06204e7c1e751120d0fd4a318bd3a9d`  
		Last Modified: Thu, 08 Jul 2021 22:54:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cec94defdad3fd63509e9888c5360499bac2b283e36def24fa2967e373cd29`  
		Last Modified: Thu, 08 Jul 2021 22:54:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e966d65046d5b8200d729f5d93484f53da5f35e93bd20038714bdc468cf2dcc`  
		Last Modified: Thu, 08 Jul 2021 22:54:53 GMT  
		Size: 2.5 MB (2542537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d34ccf25be014b39564aef59f262065cc1325a281c8b987153b7ba7bb27156`  
		Last Modified: Thu, 08 Jul 2021 22:55:04 GMT  
		Size: 59.3 MB (59250920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf4328016e1ecb0421a0ba26f22ee328541399840b78876b099d78535697075`  
		Last Modified: Thu, 08 Jul 2021 22:54:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:674b121945db632160b5b7507ca7edd0706929f903905f942baf05fd11757ae5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216454367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26b9902d6a319c00e6a6de6ad1c7aa140b73c3422f982eff6d185cfac90053f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 17:21:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 17:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Jul 2021 17:22:32 GMT
ENV LANG=C.UTF-8
# Sat, 10 Jul 2021 18:06:39 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Jul 2021 18:06:44 GMT
ENV RUBY_VERSION=2.6.8
# Sat, 10 Jul 2021 18:06:50 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Sat, 10 Jul 2021 18:17:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Jul 2021 18:17:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Jul 2021 18:17:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Jul 2021 18:17:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Jul 2021 18:17:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Jul 2021 18:17:54 GMT
CMD ["irb"]
# Sun, 11 Jul 2021 07:36:19 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Jul 2021 07:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 07:55:03 GMT
ENV RAILS_ENV=production
# Sun, 11 Jul 2021 07:55:08 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Jul 2021 07:55:12 GMT
ENV HOME=/home/redmine
# Sun, 11 Jul 2021 07:55:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Jul 2021 07:55:25 GMT
ENV REDMINE_VERSION=4.0.9
# Sun, 11 Jul 2021 07:55:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sun, 11 Jul 2021 07:55:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Jul 2021 08:14:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Jul 2021 08:14:21 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Jul 2021 08:14:24 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Jul 2021 08:14:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Jul 2021 08:14:33 GMT
EXPOSE 3000
# Sun, 11 Jul 2021 08:14:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba063dbcdd8aa55ec2183194edae6ea424d440c8c3c4ab57e29bdc8d30739f`  
		Last Modified: Sat, 10 Jul 2021 18:24:25 GMT  
		Size: 12.7 MB (12704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302bed40ec71d6898df63835eb0d9463b4672fcb74c6d77594621b1a9d96089b`  
		Last Modified: Sat, 10 Jul 2021 18:24:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae8fcb5d02ee6d84244d4abd42aa33daa130c38c85615ab4a4d0874e18a3233`  
		Last Modified: Sat, 10 Jul 2021 18:26:36 GMT  
		Size: 22.0 MB (21985630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0cda1836341e17f7519b587492ca37a7b447a8d6bfd60379f598076d411808`  
		Last Modified: Sat, 10 Jul 2021 18:26:32 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb446246ffeeee02507224564d47d57ef17f685a687ec77a197148e4ca919d6d`  
		Last Modified: Sun, 11 Jul 2021 08:16:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190d43858fa5077d6c1d4f2e08639d119b5b6762f46b9a28a85ac5a3c193f798`  
		Last Modified: Sun, 11 Jul 2021 08:17:11 GMT  
		Size: 87.9 MB (87901982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad24fee1d43ec0d26d78e1c1b9c89a1582bcecb2f2c68cd8c2b22238b4723bb0`  
		Last Modified: Sun, 11 Jul 2021 08:16:50 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbc3e255d84cdd34cf5081e18d660ac61e5cd8a0ede00fa78b5711ee41281db`  
		Last Modified: Sun, 11 Jul 2021 08:16:50 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52167f4f4ba241995b7f282ab11fd63ee3bec8fa9670bd75338b1f3478ff8d2f`  
		Last Modified: Sun, 11 Jul 2021 08:16:52 GMT  
		Size: 2.5 MB (2542551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c9e285cdc794c4508f8093c5782c93687587f21b4b4be1932583e051637728`  
		Last Modified: Sun, 11 Jul 2021 08:17:00 GMT  
		Size: 60.8 MB (60761940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c70e4ebd9b02a21a15866e9013b82d3ab23b7a2960bca79ca5a3296b96ca18e`  
		Last Modified: Sun, 11 Jul 2021 08:16:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; s390x

```console
$ docker pull redmine@sha256:2da3159861d5dc4e6220082df82d9407248c27884ee109123fb0281d48b43b69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200266732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1dbcbe1f46c48b583d905273acfa379157dd8e53c00e53cc24eadf2bd1094f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:56:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:56:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 09 Jul 2021 03:56:46 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jul 2021 04:25:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 09 Jul 2021 04:25:02 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 09 Jul 2021 04:25:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 09 Jul 2021 04:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 09 Jul 2021 04:28:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 09 Jul 2021 04:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 09 Jul 2021 04:28:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Jul 2021 04:28:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 09 Jul 2021 04:28:27 GMT
CMD ["irb"]
# Sat, 10 Jul 2021 04:03:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Jul 2021 04:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 04:10:10 GMT
ENV RAILS_ENV=production
# Sat, 10 Jul 2021 04:10:10 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Jul 2021 04:10:11 GMT
ENV HOME=/home/redmine
# Sat, 10 Jul 2021 04:10:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Jul 2021 04:10:13 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 10 Jul 2021 04:10:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 10 Jul 2021 04:10:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Jul 2021 04:14:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Jul 2021 04:14:09 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Jul 2021 04:14:09 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Jul 2021 04:14:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Jul 2021 04:14:11 GMT
EXPOSE 3000
# Sat, 10 Jul 2021 04:14:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb0861b7843d74cdcb468db372740a5fbb65d1a7a489cd207e57603e23b308`  
		Last Modified: Fri, 09 Jul 2021 04:33:35 GMT  
		Size: 10.8 MB (10814494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b9cde22299f5aa53f8d9540f770e1b6ab0e6223d1d106df86a5a071f8f3ec`  
		Last Modified: Fri, 09 Jul 2021 04:33:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c567400e82e0da61d3cd0628acf038b1f660df828736d747c5f078bf89f66f`  
		Last Modified: Fri, 09 Jul 2021 04:34:45 GMT  
		Size: 21.6 MB (21620064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267c98f7b0020a56c2dea2572a1386e898081dfbd1aa8e5c5c7b637234b6106c`  
		Last Modified: Fri, 09 Jul 2021 04:34:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d2c26dc1f4a79e7f57138c4d60e18a1efefb76d1a68fea231523dd4f61280b`  
		Last Modified: Sat, 10 Jul 2021 04:15:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873e7f0414124e21d31eb25fc989422885c98f321b6fa64904bd404c913e19ef`  
		Last Modified: Sat, 10 Jul 2021 04:15:48 GMT  
		Size: 78.9 MB (78942701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ebc5067686816d80d6f1b7f967e463030821fc3c2f520195d87bde2ca455b3`  
		Last Modified: Sat, 10 Jul 2021 04:15:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e4415b0bed5eecb3aa07263296d0cd600978da5d47a5d36f70747344436aa`  
		Last Modified: Sat, 10 Jul 2021 04:15:34 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3275e25393cb571c4316ae2296a654e68d54a9f207b5033a78953de83b9365a1`  
		Last Modified: Sat, 10 Jul 2021 04:15:35 GMT  
		Size: 2.5 MB (2542545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e47c7f2c77bb3df4747513dff31d76aef484800e246df653244270ac94bf0e2`  
		Last Modified: Sat, 10 Jul 2021 04:15:42 GMT  
		Size: 60.6 MB (60581953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e405efb3e00e11c634adbe5e545a971d1b9438220d448ce05dd17403405e99e`  
		Last Modified: Sat, 10 Jul 2021 04:15:35 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-alpine`

```console
$ docker pull redmine@sha256:9b8ec4df56622e6060cfc701a5059050c3b734da828cc8f154367d016ac22227
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:baed7be679b02ee2f252035dbc06e0fed257f026688a9fe3da3832b0bf54ae51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.9 MB (153900570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69f8d92df2e7210bf95dfe2b409c178cacd6767792bbca288c47ff774f5e817`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 08 Jul 2021 21:57:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 08 Jul 2021 21:57:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 08 Jul 2021 21:57:30 GMT
ENV LANG=C.UTF-8
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_MAJOR=2.6
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:35:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:35:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:35:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:35:59 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:26:37 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jul 2021 20:32:28 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Wed, 14 Jul 2021 20:32:28 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:32:28 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:32:29 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:32:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:32:30 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 14 Jul 2021 20:32:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 14 Jul 2021 20:32:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:32:34 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jul 2021 20:34:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jul 2021 20:34:03 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:34:04 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 14 Jul 2021 20:34:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:34:04 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:34:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b0ea69e9ed42c49b5af449b703a12a4d2f2e28d87905af6fcd903fdae5689`  
		Last Modified: Thu, 08 Jul 2021 22:38:46 GMT  
		Size: 3.6 MB (3581658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad656ed833315b61ea674706f32c2d18d7412c7120926442af57b9131ee72ee`  
		Last Modified: Thu, 08 Jul 2021 22:38:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a9d07bc1851494b8935d8593efecfea98e2c4a4ff1c3eaf2e5319eb31cb3a2`  
		Last Modified: Thu, 08 Jul 2021 22:41:47 GMT  
		Size: 19.9 MB (19889336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d50c8fd3318db7f0dbb1d50a8aa4e571ae4926440e66c07be861dd4685211d`  
		Last Modified: Thu, 08 Jul 2021 22:41:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e030b8560a875bcd9c87e7dd1c8faf94a9d48cf039ee0bf125017750cc802b`  
		Last Modified: Wed, 14 Jul 2021 20:37:07 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9541899ba9d0a6bde1aaa23a83e1e1cd6a17fc0adecb390591f66b0ccb93b`  
		Last Modified: Wed, 14 Jul 2021 20:38:23 GMT  
		Size: 66.2 MB (66172712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bc115e3ba6c2cb414f0bb5c4df5c0dad6b57442cf9044bbe1fc33e266821b4`  
		Last Modified: Wed, 14 Jul 2021 20:38:08 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0bf51497625cb7774642f214c3424e7a0e97dff3e9c1c7e96c279d965e3981`  
		Last Modified: Wed, 14 Jul 2021 20:38:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d58772bc79f2753b31d538e035d07bd09bb2731fc4843259e09b0c4be77e2f9`  
		Last Modified: Wed, 14 Jul 2021 20:38:10 GMT  
		Size: 2.5 MB (2543757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f9be46406ca851c437e457fa10b35fea3c15bda96b4f315f9514efea879beb`  
		Last Modified: Wed, 14 Jul 2021 20:38:15 GMT  
		Size: 58.9 MB (58897408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad779a0b33ba3ea1e31e4a1ee1c8bab4546aadacd48d0fb32d05adc26c02906`  
		Last Modified: Wed, 14 Jul 2021 20:38:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-passenger`

```console
$ docker pull redmine@sha256:5c4cd06fe1b29aa7167a46cc260fc067c63cf4d674b5e23dffb8d6d5f994da00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:da0b13e09beb165bb6b56a75ebbe1539903673281754de99f5c64d8c9938dd4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231317751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4a599ab4d7664421a016eba87a6a6596a9a32e5e583ae00aec3d5ab86eb6e12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:20:10 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:55:24 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:55:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:24:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:24:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:24:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:24:36 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:24:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:29:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:29:28 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:29:28 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:29:31 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:29:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:29:40 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 14 Jul 2021 20:29:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 14 Jul 2021 20:29:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:31:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:31:47 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:31:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:31:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:31:47 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:31:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:31:58 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:32:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:32:17 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:32:17 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:32:17 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b95c16c5624058c7516ccc9aff7fcb6ab05fd66e5e47c1228f4d1e8fec58b`  
		Last Modified: Thu, 08 Jul 2021 22:40:47 GMT  
		Size: 21.5 MB (21468025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596bd4a64fddd48add80e9f5ee6459a223843aacedfe89c777ed62847e9b45e`  
		Last Modified: Thu, 08 Jul 2021 22:40:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7eae1b0e301a4bb2e1dc9e8faf695f6a25c25fa76af391234a420401b27365`  
		Last Modified: Wed, 14 Jul 2021 20:36:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78eac6959ab00aa4aa16a8572577047e837cde31b8059a7c473709c1c5fd95a`  
		Last Modified: Wed, 14 Jul 2021 20:37:43 GMT  
		Size: 81.2 MB (81199589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770efe9534a041a263a97329ebea752bf15837faebf99a49e25457e40096ab17`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b58267e8ed59b94a5001480fd1362e24ec0054ae01393052c4782b412399d79`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedb8a1056b6d5f7546123709ccb9fbd52ff2e4f560bff5926c130bb0237afe`  
		Last Modified: Wed, 14 Jul 2021 20:37:29 GMT  
		Size: 2.5 MB (2542552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e80e9679392005f7d3a99eba067dbd5717479b70d7e761d843367213982dd2d`  
		Last Modified: Wed, 14 Jul 2021 20:37:36 GMT  
		Size: 60.1 MB (60148220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44914decf48cf9c7f0dce9ec00797c7f2f371ce9caf3d32730543bde7a11d036`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500a6ed36b2fa5886fdddf1c3900306c8cac410d018296ccc1e2de3220e92249`  
		Last Modified: Wed, 14 Jul 2021 20:37:58 GMT  
		Size: 21.3 MB (21327295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9ed997038310a9ec1bb536c1ba7fd7ce6674584b693e3d48b3badf23ee62ed`  
		Last Modified: Wed, 14 Jul 2021 20:37:56 GMT  
		Size: 4.9 MB (4919285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9`

```console
$ docker pull redmine@sha256:5fe2bfa25e09380eb390b7cca4ad0af896d83a3224478b8ff0855871a724fe9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.0.9` - linux; amd64

```console
$ docker pull redmine@sha256:120d31ad80c1785e72a46398a061a612987797e4607a61e60010181de0caac33
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205071171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf0b146af85cd11c523db51af33d174d5049495a32f1df271250cf823400a93e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:20:10 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:55:24 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:55:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:24:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:24:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:24:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:24:36 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:24:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:29:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:29:28 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:29:28 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:29:31 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:29:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:29:40 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 14 Jul 2021 20:29:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 14 Jul 2021 20:29:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:31:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:31:47 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:31:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:31:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:31:47 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:31:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b95c16c5624058c7516ccc9aff7fcb6ab05fd66e5e47c1228f4d1e8fec58b`  
		Last Modified: Thu, 08 Jul 2021 22:40:47 GMT  
		Size: 21.5 MB (21468025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596bd4a64fddd48add80e9f5ee6459a223843aacedfe89c777ed62847e9b45e`  
		Last Modified: Thu, 08 Jul 2021 22:40:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7eae1b0e301a4bb2e1dc9e8faf695f6a25c25fa76af391234a420401b27365`  
		Last Modified: Wed, 14 Jul 2021 20:36:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78eac6959ab00aa4aa16a8572577047e837cde31b8059a7c473709c1c5fd95a`  
		Last Modified: Wed, 14 Jul 2021 20:37:43 GMT  
		Size: 81.2 MB (81199589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770efe9534a041a263a97329ebea752bf15837faebf99a49e25457e40096ab17`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b58267e8ed59b94a5001480fd1362e24ec0054ae01393052c4782b412399d79`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedb8a1056b6d5f7546123709ccb9fbd52ff2e4f560bff5926c130bb0237afe`  
		Last Modified: Wed, 14 Jul 2021 20:37:29 GMT  
		Size: 2.5 MB (2542552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e80e9679392005f7d3a99eba067dbd5717479b70d7e761d843367213982dd2d`  
		Last Modified: Wed, 14 Jul 2021 20:37:36 GMT  
		Size: 60.1 MB (60148220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44914decf48cf9c7f0dce9ec00797c7f2f371ce9caf3d32730543bde7a11d036`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm variant v5

```console
$ docker pull redmine@sha256:17a8885564295f128c7732f2555b316d46a0843508087a8ce3c6be84ca49e3e1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194719064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84172a34f45f4e36fa6b29923eeb581145a6663c127b0aa0e40b565893379040`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:06:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:06:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:26:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:16:44 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:16:45 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:28:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:29:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:29:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:29:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:29:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:29:03 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:39:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:48:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:48:03 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:48:03 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:48:04 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:48:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:48:06 GMT
ENV REDMINE_VERSION=4.0.9
# Thu, 08 Jul 2021 22:48:07 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Thu, 08 Jul 2021 22:48:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:54:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:54:19 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:54:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:54:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:54:21 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:54:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b3ba0f03212caacd2191837bdac2f1a9abf399938b4020b315e4c6ea7ba0c7`  
		Last Modified: Wed, 23 Jun 2021 14:05:28 GMT  
		Size: 10.3 MB (10345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfab7796870f80c9db896239384ac194808f4ce5fab9f16ba155559772cc1e`  
		Last Modified: Wed, 23 Jun 2021 14:05:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7534381e53bd89c246e0ccb2c35dac17bf88c731c8d0526c63e59be51e884c`  
		Last Modified: Thu, 08 Jul 2021 20:44:48 GMT  
		Size: 20.7 MB (20733354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f2a9ffe5b789dd841f07056ea0122491118e78120d0f014d80085c602ab19c`  
		Last Modified: Thu, 08 Jul 2021 20:44:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f907c18a99e2058cc185b62d06d2138efee18b95ce1a7a7cdb625a9f526d704`  
		Last Modified: Thu, 08 Jul 2021 22:56:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427196abb69a09f982b2b40fc3aaee3149f18cc32fa0eb59adf1b3e0f59efc47`  
		Last Modified: Thu, 08 Jul 2021 22:58:49 GMT  
		Size: 77.0 MB (76964657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ba7f018f81bc6c5e5a731b53765bcf148ab61d69e2884d0f9db1916bc8c74f`  
		Last Modified: Thu, 08 Jul 2021 22:57:58 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a62c8bc56da5384f26702c4e2b1afd20300d71a66a1c4613269d37bea1ed57`  
		Last Modified: Thu, 08 Jul 2021 22:57:58 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d73596d5468e7e314bb8a661c8b46d7ae0285ff4faafdafb34c52419586231d2`  
		Last Modified: Thu, 08 Jul 2021 22:58:01 GMT  
		Size: 2.5 MB (2542548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27219bf2f048f277b05340b2c3968fb9c540542538281e1212a66176c3be0f25`  
		Last Modified: Thu, 08 Jul 2021 22:58:24 GMT  
		Size: 59.2 MB (59249510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee4a58a4863a312e6d1b986cd4fd92c4de0d610ba97f6d5cd9b7abd15a8ad506`  
		Last Modified: Thu, 08 Jul 2021 22:57:58 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm variant v7

```console
$ docker pull redmine@sha256:1c0cce8f64fd6b3b96ab6e68a14a180e928cf7e9f2b33f324fbf0d2a395db63d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.1 MB (188054222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbb6a3f75a9c20d8ef76079aeafeefab6a6b42cdaa2c435cc08a1d41689ba68e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 23:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 23:18:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 23:18:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 23:58:55 GMT
ENV RUBY_MAJOR=2.6
# Thu, 08 Jul 2021 00:04:37 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 08 Jul 2021 00:04:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:55:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:56:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:56:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:56:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:56:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:56:03 GMT
CMD ["irb"]
# Fri, 09 Jul 2021 04:13:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 09 Jul 2021 04:20:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 04:20:59 GMT
ENV RAILS_ENV=production
# Fri, 09 Jul 2021 04:21:00 GMT
WORKDIR /usr/src/redmine
# Fri, 09 Jul 2021 04:21:00 GMT
ENV HOME=/home/redmine
# Fri, 09 Jul 2021 04:21:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 09 Jul 2021 04:21:02 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 09 Jul 2021 04:21:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 09 Jul 2021 04:21:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 09 Jul 2021 04:26:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 09 Jul 2021 04:26:42 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 09 Jul 2021 04:26:42 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 09 Jul 2021 04:26:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 09 Jul 2021 04:26:43 GMT
EXPOSE 3000
# Fri, 09 Jul 2021 04:26:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b763290fb30bc16e505b4aa06ba1c3041182ac9bd8be48df5e94cbbe8545d`  
		Last Modified: Thu, 24 Jun 2021 00:49:52 GMT  
		Size: 9.9 MB (9872206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f611d0cebec7d01271526d00ff39f508174641d4e952ac4954fb89f368bf331`  
		Last Modified: Thu, 24 Jun 2021 00:49:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae3ab28fbce4cee595eb301139ed362bf539fc80d87e1203e0c2d53b9f30bd5`  
		Last Modified: Thu, 08 Jul 2021 23:21:22 GMT  
		Size: 20.6 MB (20643638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7253813058a0314e3fee8530b64e5f281a4697fd64c8d4f59d4d3c1e02f8b2`  
		Last Modified: Thu, 08 Jul 2021 23:21:13 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859eb1b9e2938ba6951e9b38fb78acaaa4383e0570cc02e2b62523694adf9dd`  
		Last Modified: Fri, 09 Jul 2021 04:28:57 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21794ae46d21df62604127bd189cd0a68e3a88763dadf737e0353b247abedd16`  
		Last Modified: Fri, 09 Jul 2021 04:30:57 GMT  
		Size: 73.3 MB (73263930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dfdd2c943ba8f6d6b1e1182cff35304fde92f76b3d398e9855ae2d9a885be1c`  
		Last Modified: Fri, 09 Jul 2021 04:30:08 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c48da2fb539ae9e73bfe86bfb185700093eb6d9793684b3ccb056e4a010e92f`  
		Last Modified: Fri, 09 Jul 2021 04:30:07 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d677deceea98b9187e223d9dfc234d8feec7032981da6731f644c03d58dc3518`  
		Last Modified: Fri, 09 Jul 2021 04:30:11 GMT  
		Size: 2.5 MB (2542534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b6c5c3bf2a5ab9c579a9d38b983fe6c9517016607fbd20230a9f6b1584aa72`  
		Last Modified: Fri, 09 Jul 2021 04:30:36 GMT  
		Size: 59.0 MB (58981614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4193fc56acb7aa51eeb30bee783268a00c2619bf1c6d9f1bdb5d739af105aea5`  
		Last Modified: Fri, 09 Jul 2021 04:30:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:0c0e8b2d97e492e291132c465b661ae141feb280bc050ba4c0173ad03bddd75d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200854434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c7e8511810a20ae664d07c2359a8ade45c9ff69408190776fe87267be6cfc8f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:53:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 03:53:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 03:53:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 04:03:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 23:54:15 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 23:54:15 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:55:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:55:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:55:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:55:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:55:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:55:12 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 23:24:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 23:27:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 23:27:01 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 23:27:01 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 23:27:02 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 23:27:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 23:27:03 GMT
ENV REDMINE_VERSION=4.0.9
# Thu, 08 Jul 2021 23:27:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Thu, 08 Jul 2021 23:27:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 23:29:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 23:29:15 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 23:29:16 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 23:29:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 23:29:16 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 23:29:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f276f053f0cad4dbf0c339099f5dd135531eb3ffb0bccc09369e7b7391b18d72`  
		Last Modified: Wed, 23 Jun 2021 04:22:18 GMT  
		Size: 11.3 MB (11263062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863be1d4664c690cf3e71cf9494c9b590ce4781e8008aef05d7cf572b8feddcc`  
		Last Modified: Wed, 23 Jun 2021 04:22:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66415307302b8ab292b3121af7b08354a3b8cdd3da935a6974c5a72434402d`  
		Last Modified: Thu, 08 Jul 2021 21:11:22 GMT  
		Size: 21.3 MB (21308810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a6b4a9d9bdbee57547a94063ad97358687fa8c834f32ae69bdbda7e30ae7f2`  
		Last Modified: Thu, 08 Jul 2021 21:11:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b848da2b7d2dc611df6b3a0f97805a3f84f9a37d2ed4c64297b3c6a599ff29`  
		Last Modified: Thu, 08 Jul 2021 23:30:27 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283276534280ca7488eedab69691a578f9a4ab1e4bce92240e245fbf2b9fe7ca`  
		Last Modified: Thu, 08 Jul 2021 23:31:12 GMT  
		Size: 79.7 MB (79748058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0a20be3baf759cd4cc371136a92a761149dd3c795690e2e6bdcf67f00888e7`  
		Last Modified: Thu, 08 Jul 2021 23:30:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972a54e8e5be6a20e8afe2b2e213c717c70d145fa74301e47e525f97563e1ce6`  
		Last Modified: Thu, 08 Jul 2021 23:30:56 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34da864d531e7092cb89dbf5aabad1503412d5ac4c443fa1b5c4392744b50a70`  
		Last Modified: Thu, 08 Jul 2021 23:30:56 GMT  
		Size: 2.5 MB (2542540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca5c55431781c4f9dc46e8e8c53d75bf6efdc54619f5e95787fa8f1338e932`  
		Last Modified: Thu, 08 Jul 2021 23:31:04 GMT  
		Size: 60.1 MB (60072722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7248a81acf81289f5e57cfc3658039b397fc876cf5b00e3c9339ea40a81997`  
		Last Modified: Thu, 08 Jul 2021 23:30:56 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; 386

```console
$ docker pull redmine@sha256:6a735b9b38729e67ecb9451ec658599d54738dd5acbeab2717922b864ba2122d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210332609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85f6591bcbd03cdbb849f6b3019e8afa5b648253bf3ae262dd6236f22c109f26`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:33:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:33:25 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:49:20 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:19:42 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:19:42 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:13:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:13:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:13:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:13:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:13:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:13:41 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:48:29 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:50:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:50:37 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:50:37 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:50:38 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:50:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:50:39 GMT
ENV REDMINE_VERSION=4.0.9
# Thu, 08 Jul 2021 22:50:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Thu, 08 Jul 2021 22:50:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:52:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:52:59 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:53:00 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:53:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:53:00 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:53:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb2041b26a9335dbdc8e6cc9bd945661b43317eb0de6d4e1e8ce82275cbea6`  
		Last Modified: Wed, 23 Jun 2021 14:14:04 GMT  
		Size: 17.2 MB (17227420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c89206098d37979fca1f31ba315796953128b80660adc5194c5541f0ac3f34`  
		Last Modified: Wed, 23 Jun 2021 14:13:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207bc054547d2959d625941a3d713cbac274d3fde559874ce3f103742021fcd0`  
		Last Modified: Thu, 08 Jul 2021 20:36:03 GMT  
		Size: 20.9 MB (20910220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bf234722053e694517615663f536b0761cb76a5ba09b68a3c42f05280985c5`  
		Last Modified: Thu, 08 Jul 2021 20:35:59 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddd76acb28134714ff2ba2109219219a0b06c2f49c2942ba8183f19f18dc444`  
		Last Modified: Thu, 08 Jul 2021 22:54:17 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40a50be1fee54ea805936c3a1d6352f729af0b25d2c7062bb99d7cc5d019042`  
		Last Modified: Thu, 08 Jul 2021 22:55:15 GMT  
		Size: 82.6 MB (82599861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743ddacf24e24c15e5268f42cbb34701c06204e7c1e751120d0fd4a318bd3a9d`  
		Last Modified: Thu, 08 Jul 2021 22:54:52 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cec94defdad3fd63509e9888c5360499bac2b283e36def24fa2967e373cd29`  
		Last Modified: Thu, 08 Jul 2021 22:54:52 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e966d65046d5b8200d729f5d93484f53da5f35e93bd20038714bdc468cf2dcc`  
		Last Modified: Thu, 08 Jul 2021 22:54:53 GMT  
		Size: 2.5 MB (2542537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d34ccf25be014b39564aef59f262065cc1325a281c8b987153b7ba7bb27156`  
		Last Modified: Thu, 08 Jul 2021 22:55:04 GMT  
		Size: 59.3 MB (59250920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf4328016e1ecb0421a0ba26f22ee328541399840b78876b099d78535697075`  
		Last Modified: Thu, 08 Jul 2021 22:54:52 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; ppc64le

```console
$ docker pull redmine@sha256:674b121945db632160b5b7507ca7edd0706929f903905f942baf05fd11757ae5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216454367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26b9902d6a319c00e6a6de6ad1c7aa140b73c3422f982eff6d185cfac90053f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 17:21:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 17:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Jul 2021 17:22:32 GMT
ENV LANG=C.UTF-8
# Sat, 10 Jul 2021 18:06:39 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Jul 2021 18:06:44 GMT
ENV RUBY_VERSION=2.6.8
# Sat, 10 Jul 2021 18:06:50 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Sat, 10 Jul 2021 18:17:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Jul 2021 18:17:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Jul 2021 18:17:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Jul 2021 18:17:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Jul 2021 18:17:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Jul 2021 18:17:54 GMT
CMD ["irb"]
# Sun, 11 Jul 2021 07:36:19 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Jul 2021 07:54:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 07:55:03 GMT
ENV RAILS_ENV=production
# Sun, 11 Jul 2021 07:55:08 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Jul 2021 07:55:12 GMT
ENV HOME=/home/redmine
# Sun, 11 Jul 2021 07:55:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Jul 2021 07:55:25 GMT
ENV REDMINE_VERSION=4.0.9
# Sun, 11 Jul 2021 07:55:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sun, 11 Jul 2021 07:55:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Jul 2021 08:14:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Jul 2021 08:14:21 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Jul 2021 08:14:24 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Jul 2021 08:14:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Jul 2021 08:14:33 GMT
EXPOSE 3000
# Sun, 11 Jul 2021 08:14:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba063dbcdd8aa55ec2183194edae6ea424d440c8c3c4ab57e29bdc8d30739f`  
		Last Modified: Sat, 10 Jul 2021 18:24:25 GMT  
		Size: 12.7 MB (12704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302bed40ec71d6898df63835eb0d9463b4672fcb74c6d77594621b1a9d96089b`  
		Last Modified: Sat, 10 Jul 2021 18:24:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae8fcb5d02ee6d84244d4abd42aa33daa130c38c85615ab4a4d0874e18a3233`  
		Last Modified: Sat, 10 Jul 2021 18:26:36 GMT  
		Size: 22.0 MB (21985630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0cda1836341e17f7519b587492ca37a7b447a8d6bfd60379f598076d411808`  
		Last Modified: Sat, 10 Jul 2021 18:26:32 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb446246ffeeee02507224564d47d57ef17f685a687ec77a197148e4ca919d6d`  
		Last Modified: Sun, 11 Jul 2021 08:16:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190d43858fa5077d6c1d4f2e08639d119b5b6762f46b9a28a85ac5a3c193f798`  
		Last Modified: Sun, 11 Jul 2021 08:17:11 GMT  
		Size: 87.9 MB (87901982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad24fee1d43ec0d26d78e1c1b9c89a1582bcecb2f2c68cd8c2b22238b4723bb0`  
		Last Modified: Sun, 11 Jul 2021 08:16:50 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbc3e255d84cdd34cf5081e18d660ac61e5cd8a0ede00fa78b5711ee41281db`  
		Last Modified: Sun, 11 Jul 2021 08:16:50 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52167f4f4ba241995b7f282ab11fd63ee3bec8fa9670bd75338b1f3478ff8d2f`  
		Last Modified: Sun, 11 Jul 2021 08:16:52 GMT  
		Size: 2.5 MB (2542551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c9e285cdc794c4508f8093c5782c93687587f21b4b4be1932583e051637728`  
		Last Modified: Sun, 11 Jul 2021 08:17:00 GMT  
		Size: 60.8 MB (60761940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c70e4ebd9b02a21a15866e9013b82d3ab23b7a2960bca79ca5a3296b96ca18e`  
		Last Modified: Sun, 11 Jul 2021 08:16:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; s390x

```console
$ docker pull redmine@sha256:2da3159861d5dc4e6220082df82d9407248c27884ee109123fb0281d48b43b69
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200266732 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1dbcbe1f46c48b583d905273acfa379157dd8e53c00e53cc24eadf2bd1094f2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:56:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:56:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 09 Jul 2021 03:56:46 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jul 2021 04:25:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 09 Jul 2021 04:25:02 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 09 Jul 2021 04:25:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 09 Jul 2021 04:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 09 Jul 2021 04:28:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 09 Jul 2021 04:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 09 Jul 2021 04:28:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Jul 2021 04:28:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 09 Jul 2021 04:28:27 GMT
CMD ["irb"]
# Sat, 10 Jul 2021 04:03:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Jul 2021 04:09:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 04:10:10 GMT
ENV RAILS_ENV=production
# Sat, 10 Jul 2021 04:10:10 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Jul 2021 04:10:11 GMT
ENV HOME=/home/redmine
# Sat, 10 Jul 2021 04:10:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Jul 2021 04:10:13 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 10 Jul 2021 04:10:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 10 Jul 2021 04:10:20 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Jul 2021 04:14:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Jul 2021 04:14:09 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Jul 2021 04:14:09 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Jul 2021 04:14:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Jul 2021 04:14:11 GMT
EXPOSE 3000
# Sat, 10 Jul 2021 04:14:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb0861b7843d74cdcb468db372740a5fbb65d1a7a489cd207e57603e23b308`  
		Last Modified: Fri, 09 Jul 2021 04:33:35 GMT  
		Size: 10.8 MB (10814494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b9cde22299f5aa53f8d9540f770e1b6ab0e6223d1d106df86a5a071f8f3ec`  
		Last Modified: Fri, 09 Jul 2021 04:33:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c567400e82e0da61d3cd0628acf038b1f660df828736d747c5f078bf89f66f`  
		Last Modified: Fri, 09 Jul 2021 04:34:45 GMT  
		Size: 21.6 MB (21620064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267c98f7b0020a56c2dea2572a1386e898081dfbd1aa8e5c5c7b637234b6106c`  
		Last Modified: Fri, 09 Jul 2021 04:34:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d2c26dc1f4a79e7f57138c4d60e18a1efefb76d1a68fea231523dd4f61280b`  
		Last Modified: Sat, 10 Jul 2021 04:15:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:873e7f0414124e21d31eb25fc989422885c98f321b6fa64904bd404c913e19ef`  
		Last Modified: Sat, 10 Jul 2021 04:15:48 GMT  
		Size: 78.9 MB (78942701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ebc5067686816d80d6f1b7f967e463030821fc3c2f520195d87bde2ca455b3`  
		Last Modified: Sat, 10 Jul 2021 04:15:34 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456e4415b0bed5eecb3aa07263296d0cd600978da5d47a5d36f70747344436aa`  
		Last Modified: Sat, 10 Jul 2021 04:15:34 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3275e25393cb571c4316ae2296a654e68d54a9f207b5033a78953de83b9365a1`  
		Last Modified: Sat, 10 Jul 2021 04:15:35 GMT  
		Size: 2.5 MB (2542545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e47c7f2c77bb3df4747513dff31d76aef484800e246df653244270ac94bf0e2`  
		Last Modified: Sat, 10 Jul 2021 04:15:42 GMT  
		Size: 60.6 MB (60581953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e405efb3e00e11c634adbe5e545a971d1b9438220d448ce05dd17403405e99e`  
		Last Modified: Sat, 10 Jul 2021 04:15:35 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9-alpine`

```console
$ docker pull redmine@sha256:9b8ec4df56622e6060cfc701a5059050c3b734da828cc8f154367d016ac22227
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0.9-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:baed7be679b02ee2f252035dbc06e0fed257f026688a9fe3da3832b0bf54ae51
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.9 MB (153900570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c69f8d92df2e7210bf95dfe2b409c178cacd6767792bbca288c47ff774f5e817`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 08 Jul 2021 21:57:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 08 Jul 2021 21:57:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 08 Jul 2021 21:57:30 GMT
ENV LANG=C.UTF-8
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_MAJOR=2.6
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:35:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:35:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:35:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:35:59 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:26:37 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jul 2021 20:32:28 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Wed, 14 Jul 2021 20:32:28 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:32:28 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:32:29 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:32:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:32:30 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 14 Jul 2021 20:32:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 14 Jul 2021 20:32:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:32:34 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jul 2021 20:34:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jul 2021 20:34:03 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:34:04 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 14 Jul 2021 20:34:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:34:04 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:34:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b0ea69e9ed42c49b5af449b703a12a4d2f2e28d87905af6fcd903fdae5689`  
		Last Modified: Thu, 08 Jul 2021 22:38:46 GMT  
		Size: 3.6 MB (3581658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad656ed833315b61ea674706f32c2d18d7412c7120926442af57b9131ee72ee`  
		Last Modified: Thu, 08 Jul 2021 22:38:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a9d07bc1851494b8935d8593efecfea98e2c4a4ff1c3eaf2e5319eb31cb3a2`  
		Last Modified: Thu, 08 Jul 2021 22:41:47 GMT  
		Size: 19.9 MB (19889336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d50c8fd3318db7f0dbb1d50a8aa4e571ae4926440e66c07be861dd4685211d`  
		Last Modified: Thu, 08 Jul 2021 22:41:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e030b8560a875bcd9c87e7dd1c8faf94a9d48cf039ee0bf125017750cc802b`  
		Last Modified: Wed, 14 Jul 2021 20:37:07 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9541899ba9d0a6bde1aaa23a83e1e1cd6a17fc0adecb390591f66b0ccb93b`  
		Last Modified: Wed, 14 Jul 2021 20:38:23 GMT  
		Size: 66.2 MB (66172712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26bc115e3ba6c2cb414f0bb5c4df5c0dad6b57442cf9044bbe1fc33e266821b4`  
		Last Modified: Wed, 14 Jul 2021 20:38:08 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0bf51497625cb7774642f214c3424e7a0e97dff3e9c1c7e96c279d965e3981`  
		Last Modified: Wed, 14 Jul 2021 20:38:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d58772bc79f2753b31d538e035d07bd09bb2731fc4843259e09b0c4be77e2f9`  
		Last Modified: Wed, 14 Jul 2021 20:38:10 GMT  
		Size: 2.5 MB (2543757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f9be46406ca851c437e457fa10b35fea3c15bda96b4f315f9514efea879beb`  
		Last Modified: Wed, 14 Jul 2021 20:38:15 GMT  
		Size: 58.9 MB (58897408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad779a0b33ba3ea1e31e4a1ee1c8bab4546aadacd48d0fb32d05adc26c02906`  
		Last Modified: Wed, 14 Jul 2021 20:38:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9-passenger`

```console
$ docker pull redmine@sha256:5c4cd06fe1b29aa7167a46cc260fc067c63cf4d674b5e23dffb8d6d5f994da00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0.9-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:da0b13e09beb165bb6b56a75ebbe1539903673281754de99f5c64d8c9938dd4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231317751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4a599ab4d7664421a016eba87a6a6596a9a32e5e583ae00aec3d5ab86eb6e12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:20:10 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:55:24 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:55:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:24:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:24:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:24:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:24:36 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:24:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:29:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:29:28 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:29:28 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:29:31 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:29:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:29:40 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 14 Jul 2021 20:29:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 14 Jul 2021 20:29:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:31:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:31:47 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:31:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:31:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:31:47 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:31:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:31:58 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:32:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:32:17 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:32:17 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:32:17 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b95c16c5624058c7516ccc9aff7fcb6ab05fd66e5e47c1228f4d1e8fec58b`  
		Last Modified: Thu, 08 Jul 2021 22:40:47 GMT  
		Size: 21.5 MB (21468025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596bd4a64fddd48add80e9f5ee6459a223843aacedfe89c777ed62847e9b45e`  
		Last Modified: Thu, 08 Jul 2021 22:40:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7eae1b0e301a4bb2e1dc9e8faf695f6a25c25fa76af391234a420401b27365`  
		Last Modified: Wed, 14 Jul 2021 20:36:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78eac6959ab00aa4aa16a8572577047e837cde31b8059a7c473709c1c5fd95a`  
		Last Modified: Wed, 14 Jul 2021 20:37:43 GMT  
		Size: 81.2 MB (81199589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770efe9534a041a263a97329ebea752bf15837faebf99a49e25457e40096ab17`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b58267e8ed59b94a5001480fd1362e24ec0054ae01393052c4782b412399d79`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dedb8a1056b6d5f7546123709ccb9fbd52ff2e4f560bff5926c130bb0237afe`  
		Last Modified: Wed, 14 Jul 2021 20:37:29 GMT  
		Size: 2.5 MB (2542552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e80e9679392005f7d3a99eba067dbd5717479b70d7e761d843367213982dd2d`  
		Last Modified: Wed, 14 Jul 2021 20:37:36 GMT  
		Size: 60.1 MB (60148220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44914decf48cf9c7f0dce9ec00797c7f2f371ce9caf3d32730543bde7a11d036`  
		Last Modified: Wed, 14 Jul 2021 20:37:28 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500a6ed36b2fa5886fdddf1c3900306c8cac410d018296ccc1e2de3220e92249`  
		Last Modified: Wed, 14 Jul 2021 20:37:58 GMT  
		Size: 21.3 MB (21327295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9ed997038310a9ec1bb536c1ba7fd7ce6674584b693e3d48b3badf23ee62ed`  
		Last Modified: Wed, 14 Jul 2021 20:37:56 GMT  
		Size: 4.9 MB (4919285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1`

```console
$ docker pull redmine@sha256:3842f8b458e034ecec57ede811de2c27a56157afbcfd04dfa171f53c98bbabcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.1` - linux; amd64

```console
$ docker pull redmine@sha256:8cb4cab2bed4c965b285663a240d5bb2fc566e08b20eafa760751342009052ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.6 MB (206647502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8deeaf98c6f43b867d4af4456933ea02db08ba0623f0f2deeb5e921ec9f90b87`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:20:10 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:55:24 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:55:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:24:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:24:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:24:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:24:36 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:24:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:25:16 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:25:16 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:25:16 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:25:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:25:17 GMT
ENV REDMINE_VERSION=4.1.3
# Wed, 14 Jul 2021 20:25:18 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Wed, 14 Jul 2021 20:25:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:26:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:26:01 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:26:01 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:26:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:26:02 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:26:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b95c16c5624058c7516ccc9aff7fcb6ab05fd66e5e47c1228f4d1e8fec58b`  
		Last Modified: Thu, 08 Jul 2021 22:40:47 GMT  
		Size: 21.5 MB (21468025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596bd4a64fddd48add80e9f5ee6459a223843aacedfe89c777ed62847e9b45e`  
		Last Modified: Thu, 08 Jul 2021 22:40:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7eae1b0e301a4bb2e1dc9e8faf695f6a25c25fa76af391234a420401b27365`  
		Last Modified: Wed, 14 Jul 2021 20:36:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267137a65ba8a2d9e353059d3da16877f506fa5ff13446e0445c0c4c3bcd784`  
		Last Modified: Wed, 14 Jul 2021 20:36:39 GMT  
		Size: 94.1 MB (94088312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443f532876e21e028bcb587e538fc650ce86a658794ac88dc47a19307ea98e3c`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2e5bbb56b3693c8317028271070258892c483ef1b2d9c0029cbd6d9788595d`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d9073f85635b6e855482f3fb205876b8d7623e0e0b2d0477f00f3f8a93e121`  
		Last Modified: Wed, 14 Jul 2021 20:36:22 GMT  
		Size: 2.7 MB (2747699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c2f3d2afd7b0a0978553d8a765d905c04663f3a050c334496ae656c755c4af`  
		Last Modified: Wed, 14 Jul 2021 20:36:27 GMT  
		Size: 48.6 MB (48630681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cf6faa89c3fe5437d036e3116d55e5185e803f18d486ae7510374d0c6a081d`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:f702db399231e0243f954b0787c2ff9dd1d59693d7f2e02dcbbe13e28220a194
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210649712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb0b3c9b3e19e2130c8ace0dc71dfd0bdd7b558fa946ac25771b4e51150df1b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:06:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:06:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:26:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:16:44 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:16:45 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:28:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:29:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:29:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:29:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:29:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:29:03 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:39:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:41:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:41:02 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:41:03 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:41:03 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:41:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:41:05 GMT
ENV REDMINE_VERSION=4.1.3
# Thu, 08 Jul 2021 22:41:06 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Thu, 08 Jul 2021 22:41:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:46:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:46:49 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:46:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:46:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:46:50 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:46:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b3ba0f03212caacd2191837bdac2f1a9abf399938b4020b315e4c6ea7ba0c7`  
		Last Modified: Wed, 23 Jun 2021 14:05:28 GMT  
		Size: 10.3 MB (10345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfab7796870f80c9db896239384ac194808f4ce5fab9f16ba155559772cc1e`  
		Last Modified: Wed, 23 Jun 2021 14:05:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7534381e53bd89c246e0ccb2c35dac17bf88c731c8d0526c63e59be51e884c`  
		Last Modified: Thu, 08 Jul 2021 20:44:48 GMT  
		Size: 20.7 MB (20733354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f2a9ffe5b789dd841f07056ea0122491118e78120d0f014d80085c602ab19c`  
		Last Modified: Thu, 08 Jul 2021 20:44:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f907c18a99e2058cc185b62d06d2138efee18b95ce1a7a7cdb625a9f526d704`  
		Last Modified: Thu, 08 Jul 2021 22:56:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9853b9e735dbc222e0627de3e38803e7f55197c1db1486b45a0acf6a829385`  
		Last Modified: Thu, 08 Jul 2021 22:57:45 GMT  
		Size: 89.6 MB (89575898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0be406a40fb9c97009fbc9316f6c0e5c1b079ae448337b08319d2fa80f9002`  
		Last Modified: Thu, 08 Jul 2021 22:56:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671df9eb690f6e5280275ad105884d35b80fca5608d9ee7bb9b6cff80c5fa113`  
		Last Modified: Thu, 08 Jul 2021 22:56:39 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ba8c671508e4cc58e6d481f258e99775cc5c1086a7425a5adf0955191b6b3d`  
		Last Modified: Thu, 08 Jul 2021 22:56:42 GMT  
		Size: 2.7 MB (2747694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265dac386bdcb11bef4564c82f342485592b05218eaf2f3c2d9a23f2fe54c742`  
		Last Modified: Thu, 08 Jul 2021 22:57:08 GMT  
		Size: 62.4 MB (62363772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45cf3cc04e0538f87ced4ea51421b041406ea6346a9feaae13ccaf61bebcd5a`  
		Last Modified: Thu, 08 Jul 2021 22:56:39 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:f98e169cbbbd1e69e7b99c2d2e5afd65fc506a2a4a0ba960712a23c5c0f7d168
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203830355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03c42097246ae6c0497adef62152905fc8745b6948196e85d759c355b92e114d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 23:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 23:18:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 23:18:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 23:58:55 GMT
ENV RUBY_MAJOR=2.6
# Thu, 08 Jul 2021 00:04:37 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 08 Jul 2021 00:04:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:55:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:56:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:56:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:56:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:56:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:56:03 GMT
CMD ["irb"]
# Fri, 09 Jul 2021 04:13:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 09 Jul 2021 04:14:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 04:14:18 GMT
ENV RAILS_ENV=production
# Fri, 09 Jul 2021 04:14:18 GMT
WORKDIR /usr/src/redmine
# Fri, 09 Jul 2021 04:14:19 GMT
ENV HOME=/home/redmine
# Fri, 09 Jul 2021 04:14:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 09 Jul 2021 04:14:21 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 09 Jul 2021 04:14:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 09 Jul 2021 04:14:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 09 Jul 2021 04:19:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 09 Jul 2021 04:19:42 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 09 Jul 2021 04:19:43 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 09 Jul 2021 04:19:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 09 Jul 2021 04:19:44 GMT
EXPOSE 3000
# Fri, 09 Jul 2021 04:19:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b763290fb30bc16e505b4aa06ba1c3041182ac9bd8be48df5e94cbbe8545d`  
		Last Modified: Thu, 24 Jun 2021 00:49:52 GMT  
		Size: 9.9 MB (9872206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f611d0cebec7d01271526d00ff39f508174641d4e952ac4954fb89f368bf331`  
		Last Modified: Thu, 24 Jun 2021 00:49:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae3ab28fbce4cee595eb301139ed362bf539fc80d87e1203e0c2d53b9f30bd5`  
		Last Modified: Thu, 08 Jul 2021 23:21:22 GMT  
		Size: 20.6 MB (20643638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7253813058a0314e3fee8530b64e5f281a4697fd64c8d4f59d4d3c1e02f8b2`  
		Last Modified: Thu, 08 Jul 2021 23:21:13 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859eb1b9e2938ba6951e9b38fb78acaaa4383e0570cc02e2b62523694adf9dd`  
		Last Modified: Fri, 09 Jul 2021 04:28:57 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e657e10c5e16645f5a4f752ea53919857cc3a3938ec16a933424e7b8c80b52a`  
		Last Modified: Fri, 09 Jul 2021 04:29:54 GMT  
		Size: 85.6 MB (85590488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95828495eb16bece32e4866d6a2567c2b1808df4c04e5a6dc6e28656da6dcf3`  
		Last Modified: Fri, 09 Jul 2021 04:28:55 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cd1318e42fa39223bed7cfbf8dd58828a6cd038585f8f9b89036054e8169c9`  
		Last Modified: Fri, 09 Jul 2021 04:28:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8aa84af383ed755d6f8f6998abd7be83a7ef724a14e8a56ba36066d3115ba34`  
		Last Modified: Fri, 09 Jul 2021 04:28:59 GMT  
		Size: 2.7 MB (2747692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112271ea3d64d4644770487201a5a69033c1302c09cefd8bc945e4bdd3fdf54b`  
		Last Modified: Fri, 09 Jul 2021 04:29:26 GMT  
		Size: 62.2 MB (62226034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20e4b35ba129dfba514cc450ea03df0146e5a7831f3f9d5cf11843b8e014391`  
		Last Modified: Fri, 09 Jul 2021 04:28:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:de07cd2752ffade4ed0c1170de0477e4d2dd9b0ab3dd1a7a1b88a2a73c064bc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217532051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97dd6f537f78477580e3d7cf8f95723ecc7fcbc8b3d94394e8bb4789ceb9fed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:53:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 03:53:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 03:53:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 04:03:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 23:54:15 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 23:54:15 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:55:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:55:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:55:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:55:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:55:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:55:12 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 23:24:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 23:24:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 23:24:22 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 23:24:22 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 23:24:22 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 23:24:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 23:24:23 GMT
ENV REDMINE_VERSION=4.1.3
# Thu, 08 Jul 2021 23:24:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Thu, 08 Jul 2021 23:24:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 23:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 23:26:29 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 23:26:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 23:26:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 23:26:30 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 23:26:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f276f053f0cad4dbf0c339099f5dd135531eb3ffb0bccc09369e7b7391b18d72`  
		Last Modified: Wed, 23 Jun 2021 04:22:18 GMT  
		Size: 11.3 MB (11263062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863be1d4664c690cf3e71cf9494c9b590ce4781e8008aef05d7cf572b8feddcc`  
		Last Modified: Wed, 23 Jun 2021 04:22:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66415307302b8ab292b3121af7b08354a3b8cdd3da935a6974c5a72434402d`  
		Last Modified: Thu, 08 Jul 2021 21:11:22 GMT  
		Size: 21.3 MB (21308810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a6b4a9d9bdbee57547a94063ad97358687fa8c834f32ae69bdbda7e30ae7f2`  
		Last Modified: Thu, 08 Jul 2021 21:11:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b848da2b7d2dc611df6b3a0f97805a3f84f9a37d2ed4c64297b3c6a599ff29`  
		Last Modified: Thu, 08 Jul 2021 23:30:27 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554949a502335a2a91d95a53e82f90e17601b6a5d0da2a74f700b31b5f6e3a8a`  
		Last Modified: Thu, 08 Jul 2021 23:30:43 GMT  
		Size: 92.6 MB (92610181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a792ac4df99887c8831f90baafac41c8639b08181cec9388e7429011eb20348c`  
		Last Modified: Thu, 08 Jul 2021 23:30:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fbe99ccee1394d284c3ca7c7aea40a908b7d463e96728d1c82336776e8b2fd`  
		Last Modified: Thu, 08 Jul 2021 23:30:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7eb23c68ed546186ae3c1f2cd91b7f2111f5ae6b766b20d1e8a2c87e22319`  
		Last Modified: Thu, 08 Jul 2021 23:30:26 GMT  
		Size: 2.7 MB (2747696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2e671f454fbbf045db7d382bf48f64118acdc5436869c619f904a16a8dd87b`  
		Last Modified: Thu, 08 Jul 2021 23:30:33 GMT  
		Size: 63.7 MB (63683060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1e8a3621686b595efaede73f25979044b720ec8e83d05f1174f0d59f8a048`  
		Last Modified: Thu, 08 Jul 2021 23:30:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; 386

```console
$ docker pull redmine@sha256:2e14e83e20d1408e0e2108c2b18b45eba248c368fe7b9fd0772f014d90e669ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213005188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56761260ee9dfd0db61d52a675d87f0ebde983702c471ab0820e99cadca4e1ab`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:33:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:33:25 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:49:20 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:19:42 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:19:42 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:13:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:13:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:13:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:13:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:13:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:13:41 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:48:29 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:49:00 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:49:00 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:49:00 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:49:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:49:02 GMT
ENV REDMINE_VERSION=4.1.3
# Thu, 08 Jul 2021 22:49:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Thu, 08 Jul 2021 22:49:05 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:49:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:49:55 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:49:55 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:49:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:49:55 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:49:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb2041b26a9335dbdc8e6cc9bd945661b43317eb0de6d4e1e8ce82275cbea6`  
		Last Modified: Wed, 23 Jun 2021 14:14:04 GMT  
		Size: 17.2 MB (17227420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c89206098d37979fca1f31ba315796953128b80660adc5194c5541f0ac3f34`  
		Last Modified: Wed, 23 Jun 2021 14:13:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207bc054547d2959d625941a3d713cbac274d3fde559874ce3f103742021fcd0`  
		Last Modified: Thu, 08 Jul 2021 20:36:03 GMT  
		Size: 20.9 MB (20910220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bf234722053e694517615663f536b0761cb76a5ba09b68a3c42f05280985c5`  
		Last Modified: Thu, 08 Jul 2021 20:35:59 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddd76acb28134714ff2ba2109219219a0b06c2f49c2942ba8183f19f18dc444`  
		Last Modified: Thu, 08 Jul 2021 22:54:17 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcbd90475437342f2a203b5d50b579606260b8df5b6bb44e97838424449c174`  
		Last Modified: Thu, 08 Jul 2021 22:54:39 GMT  
		Size: 95.7 MB (95701755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2637680a5b95a8d2bca3c146d25ef9d9ce4df35e84a9424ac9fad1df6452187`  
		Last Modified: Thu, 08 Jul 2021 22:54:14 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b3edc1a7cb5e5c17408b31a4dcb0d8abab5a18e903bf6c0865d2ed3000b8d8`  
		Last Modified: Thu, 08 Jul 2021 22:54:14 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce4e35470521f4474417b529d73651e68fa3c7b1a66b3f9e24e4d78428d1864`  
		Last Modified: Thu, 08 Jul 2021 22:54:16 GMT  
		Size: 2.7 MB (2747687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a0de80af3eeba8f8b14edd03cc1a78bc618e037ac0ef8365a167556fbb5a80`  
		Last Modified: Thu, 08 Jul 2021 22:54:23 GMT  
		Size: 48.6 MB (48616454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f132a96251c7173e4b6d07e6a3e69105aa6099d08fe84d05dacef4837f7caa3`  
		Last Modified: Thu, 08 Jul 2021 22:54:14 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:64883bedbcb8390e549569df03596c1592c1f1cf09100882a2adb30a7464f677
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234101304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071cf966f6433307edcd7bc665b2280f5ebfbd80d77ba532b25a07b3f3be3508`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 17:21:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 17:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Jul 2021 17:22:32 GMT
ENV LANG=C.UTF-8
# Sat, 10 Jul 2021 18:06:39 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Jul 2021 18:06:44 GMT
ENV RUBY_VERSION=2.6.8
# Sat, 10 Jul 2021 18:06:50 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Sat, 10 Jul 2021 18:17:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Jul 2021 18:17:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Jul 2021 18:17:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Jul 2021 18:17:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Jul 2021 18:17:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Jul 2021 18:17:54 GMT
CMD ["irb"]
# Sun, 11 Jul 2021 07:36:19 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Jul 2021 07:42:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 07:42:53 GMT
ENV RAILS_ENV=production
# Sun, 11 Jul 2021 07:42:59 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Jul 2021 07:43:08 GMT
ENV HOME=/home/redmine
# Sun, 11 Jul 2021 07:43:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Jul 2021 07:43:28 GMT
ENV REDMINE_VERSION=4.1.3
# Sun, 11 Jul 2021 07:43:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Sun, 11 Jul 2021 07:43:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Jul 2021 07:50:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Jul 2021 07:50:20 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Jul 2021 07:50:24 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Jul 2021 07:50:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Jul 2021 07:50:31 GMT
EXPOSE 3000
# Sun, 11 Jul 2021 07:50:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba063dbcdd8aa55ec2183194edae6ea424d440c8c3c4ab57e29bdc8d30739f`  
		Last Modified: Sat, 10 Jul 2021 18:24:25 GMT  
		Size: 12.7 MB (12704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302bed40ec71d6898df63835eb0d9463b4672fcb74c6d77594621b1a9d96089b`  
		Last Modified: Sat, 10 Jul 2021 18:24:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae8fcb5d02ee6d84244d4abd42aa33daa130c38c85615ab4a4d0874e18a3233`  
		Last Modified: Sat, 10 Jul 2021 18:26:36 GMT  
		Size: 22.0 MB (21985630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0cda1836341e17f7519b587492ca37a7b447a8d6bfd60379f598076d411808`  
		Last Modified: Sat, 10 Jul 2021 18:26:32 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb446246ffeeee02507224564d47d57ef17f685a687ec77a197148e4ca919d6d`  
		Last Modified: Sun, 11 Jul 2021 08:16:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12db92ff7b3432686c3cfeb8bf4e0c17267325be39418f465e7dad91e61c85`  
		Last Modified: Sun, 11 Jul 2021 08:16:37 GMT  
		Size: 101.3 MB (101328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcd9eae2a479db34f85b60dabb3c448541cf492a571c4bdf5ad96980eea4f24`  
		Last Modified: Sun, 11 Jul 2021 08:16:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d325149e44e852ef5c9117755d729156ad8f55cef5f63d673a10ac82b188f346`  
		Last Modified: Sun, 11 Jul 2021 08:16:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a42445324d562b4682195c2466cae731ce845ea83e4cb2c45d1e89d24b08fb2`  
		Last Modified: Sun, 11 Jul 2021 08:16:14 GMT  
		Size: 2.7 MB (2747692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924db074ef0d503477ef377086ba7d8dc65a4cd537fbcdb51c9c43b626cf3a86`  
		Last Modified: Sun, 11 Jul 2021 08:16:23 GMT  
		Size: 64.8 MB (64777609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243901ca86f6ec755dec21a70a11d89574c9d8a34cabd75fb30158f18034f7f4`  
		Last Modified: Sun, 11 Jul 2021 08:16:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; s390x

```console
$ docker pull redmine@sha256:56f544d99f465a37892af1c1f1e4a46510ead3d9cf83cbbb015a983eaf22a49d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216896693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:519746193a5092cc036db7e6c4987f1f2d362ffc2e3a80325935ca32b17d3803`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:56:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:56:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 09 Jul 2021 03:56:46 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jul 2021 04:25:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 09 Jul 2021 04:25:02 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 09 Jul 2021 04:25:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 09 Jul 2021 04:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 09 Jul 2021 04:28:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 09 Jul 2021 04:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 09 Jul 2021 04:28:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Jul 2021 04:28:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 09 Jul 2021 04:28:27 GMT
CMD ["irb"]
# Sat, 10 Jul 2021 04:03:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Jul 2021 04:05:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 04:05:23 GMT
ENV RAILS_ENV=production
# Sat, 10 Jul 2021 04:05:23 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Jul 2021 04:05:24 GMT
ENV HOME=/home/redmine
# Sat, 10 Jul 2021 04:05:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Jul 2021 04:05:27 GMT
ENV REDMINE_VERSION=4.1.3
# Sat, 10 Jul 2021 04:05:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Sat, 10 Jul 2021 04:05:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Jul 2021 04:08:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Jul 2021 04:08:32 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Jul 2021 04:08:33 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Jul 2021 04:08:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Jul 2021 04:08:34 GMT
EXPOSE 3000
# Sat, 10 Jul 2021 04:08:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb0861b7843d74cdcb468db372740a5fbb65d1a7a489cd207e57603e23b308`  
		Last Modified: Fri, 09 Jul 2021 04:33:35 GMT  
		Size: 10.8 MB (10814494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b9cde22299f5aa53f8d9540f770e1b6ab0e6223d1d106df86a5a071f8f3ec`  
		Last Modified: Fri, 09 Jul 2021 04:33:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c567400e82e0da61d3cd0628acf038b1f660df828736d747c5f078bf89f66f`  
		Last Modified: Fri, 09 Jul 2021 04:34:45 GMT  
		Size: 21.6 MB (21620064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267c98f7b0020a56c2dea2572a1386e898081dfbd1aa8e5c5c7b637234b6106c`  
		Last Modified: Fri, 09 Jul 2021 04:34:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d2c26dc1f4a79e7f57138c4d60e18a1efefb76d1a68fea231523dd4f61280b`  
		Last Modified: Sat, 10 Jul 2021 04:15:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2023bcadbc7a0f004c2da93fb37351dc4c05dc9941da2c0a74b1cb355e6318f`  
		Last Modified: Sat, 10 Jul 2021 04:15:26 GMT  
		Size: 91.8 MB (91789480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be589db26f20104b7d0d51e59f22288748ef178271a3cb237668a9ba4e8e3873`  
		Last Modified: Sat, 10 Jul 2021 04:15:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af0e3df0ae2fc1b6ed5a432d063589f9801d348e673aa45eb2d7e9c2ee34edf`  
		Last Modified: Sat, 10 Jul 2021 04:15:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9790215cdf9ba47d2b3dcf055017f99e27dfb80491bd0dbf6a21e5081f3670df`  
		Last Modified: Sat, 10 Jul 2021 04:15:11 GMT  
		Size: 2.7 MB (2747692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1c18585fbe6a261eb8691fe17fc2f7c39e71c91abe4849ff7a04f5dc2a06c`  
		Last Modified: Sat, 10 Jul 2021 04:15:17 GMT  
		Size: 64.2 MB (64159990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b73773553e88959f1468859ce50e418c31af41dda709211aaaf8f0ff48e50d`  
		Last Modified: Sat, 10 Jul 2021 04:15:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-alpine`

```console
$ docker pull redmine@sha256:ab4e088a86875b1b538344cd8bffecef2ae743209af62856f076991270196c4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:6fc987ac3687a985a641ecc4ffeb66fae30dfe751d67d0b96c3d7b3a0dea4939
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161071838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c092b6a7e727cff2c4ca5d85fea3f0833a29b70489519ff6fa71c81e678f27c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 08 Jul 2021 21:57:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 08 Jul 2021 21:57:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 08 Jul 2021 21:57:30 GMT
ENV LANG=C.UTF-8
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_MAJOR=2.6
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:35:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:35:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:35:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:35:59 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:26:37 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jul 2021 20:26:45 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 14 Jul 2021 20:26:46 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:26:46 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:26:46 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:26:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:26:48 GMT
ENV REDMINE_VERSION=4.1.3
# Wed, 14 Jul 2021 20:26:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Wed, 14 Jul 2021 20:26:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:26:52 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jul 2021 20:28:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jul 2021 20:28:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:28:54 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 14 Jul 2021 20:28:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:28:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:28:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b0ea69e9ed42c49b5af449b703a12a4d2f2e28d87905af6fcd903fdae5689`  
		Last Modified: Thu, 08 Jul 2021 22:38:46 GMT  
		Size: 3.6 MB (3581658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad656ed833315b61ea674706f32c2d18d7412c7120926442af57b9131ee72ee`  
		Last Modified: Thu, 08 Jul 2021 22:38:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a9d07bc1851494b8935d8593efecfea98e2c4a4ff1c3eaf2e5319eb31cb3a2`  
		Last Modified: Thu, 08 Jul 2021 22:41:47 GMT  
		Size: 19.9 MB (19889336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d50c8fd3318db7f0dbb1d50a8aa4e571ae4926440e66c07be861dd4685211d`  
		Last Modified: Thu, 08 Jul 2021 22:41:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e030b8560a875bcd9c87e7dd1c8faf94a9d48cf039ee0bf125017750cc802b`  
		Last Modified: Wed, 14 Jul 2021 20:37:07 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c0006aa2ad99f9ffc9d729323dc4d6fe56017cf11735d341570e65864f6425`  
		Last Modified: Wed, 14 Jul 2021 20:37:17 GMT  
		Size: 69.5 MB (69526405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde1c41e26debfed4512ebfbeb0a14368410a36df9e8a30216966c830eee17ad`  
		Last Modified: Wed, 14 Jul 2021 20:37:04 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968695fc5116055ee483a173dbd08fdd5e9aba5dea28a955cdc730ae9f0bba52`  
		Last Modified: Wed, 14 Jul 2021 20:37:04 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f9412f7e58bd4742f678cd456ad14d8788771c9f2bd64676be5ef15102d32c`  
		Last Modified: Wed, 14 Jul 2021 20:37:05 GMT  
		Size: 2.7 MB (2748565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ce5851323b28845c755def36a5d70eb4eb98b968fb1d0bf274beba4b0ee408`  
		Last Modified: Wed, 14 Jul 2021 20:37:10 GMT  
		Size: 62.5 MB (62510175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553a89009171bdde8e1ac3c30cb9283a86cc357db925559833d12fd7c7b7d93d`  
		Last Modified: Wed, 14 Jul 2021 20:37:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-passenger`

```console
$ docker pull redmine@sha256:4334cb7c8b95d9668f01fc9f8c8ffdd56b40964b7a4a82b0cb4eb6a3f9c74e72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:c1430615177875a68f1379e64e7c5bd75a780909650fb68487080cac12f38df2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232889438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2326128b089e53f55073cb580d592df8870f42e043d8f35b9c44a1fc630a160f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:20:10 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:55:24 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:55:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:24:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:24:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:24:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:24:36 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:24:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:25:16 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:25:16 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:25:16 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:25:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:25:17 GMT
ENV REDMINE_VERSION=4.1.3
# Wed, 14 Jul 2021 20:25:18 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Wed, 14 Jul 2021 20:25:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:26:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:26:01 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:26:01 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:26:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:26:02 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:26:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:26:14 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:26:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:26:33 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:26:33 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:26:33 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b95c16c5624058c7516ccc9aff7fcb6ab05fd66e5e47c1228f4d1e8fec58b`  
		Last Modified: Thu, 08 Jul 2021 22:40:47 GMT  
		Size: 21.5 MB (21468025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596bd4a64fddd48add80e9f5ee6459a223843aacedfe89c777ed62847e9b45e`  
		Last Modified: Thu, 08 Jul 2021 22:40:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7eae1b0e301a4bb2e1dc9e8faf695f6a25c25fa76af391234a420401b27365`  
		Last Modified: Wed, 14 Jul 2021 20:36:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267137a65ba8a2d9e353059d3da16877f506fa5ff13446e0445c0c4c3bcd784`  
		Last Modified: Wed, 14 Jul 2021 20:36:39 GMT  
		Size: 94.1 MB (94088312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443f532876e21e028bcb587e538fc650ce86a658794ac88dc47a19307ea98e3c`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2e5bbb56b3693c8317028271070258892c483ef1b2d9c0029cbd6d9788595d`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d9073f85635b6e855482f3fb205876b8d7623e0e0b2d0477f00f3f8a93e121`  
		Last Modified: Wed, 14 Jul 2021 20:36:22 GMT  
		Size: 2.7 MB (2747699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c2f3d2afd7b0a0978553d8a765d905c04663f3a050c334496ae656c755c4af`  
		Last Modified: Wed, 14 Jul 2021 20:36:27 GMT  
		Size: 48.6 MB (48630681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cf6faa89c3fe5437d036e3116d55e5185e803f18d486ae7510374d0c6a081d`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf013518a02ee1e21f728797726c8cd338e36dc5f93a2ca79d2e219176ab2cdf`  
		Last Modified: Wed, 14 Jul 2021 20:36:53 GMT  
		Size: 21.3 MB (21322651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d8dc1a16c759aa15798aa8cbca04ff8c4532a0be26e406f4f4db28aa7d4bd`  
		Last Modified: Wed, 14 Jul 2021 20:36:50 GMT  
		Size: 4.9 MB (4919285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.3`

```console
$ docker pull redmine@sha256:3842f8b458e034ecec57ede811de2c27a56157afbcfd04dfa171f53c98bbabcb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.1.3` - linux; amd64

```console
$ docker pull redmine@sha256:8cb4cab2bed4c965b285663a240d5bb2fc566e08b20eafa760751342009052ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.6 MB (206647502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8deeaf98c6f43b867d4af4456933ea02db08ba0623f0f2deeb5e921ec9f90b87`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:20:10 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:55:24 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:55:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:24:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:24:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:24:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:24:36 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:24:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:25:16 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:25:16 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:25:16 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:25:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:25:17 GMT
ENV REDMINE_VERSION=4.1.3
# Wed, 14 Jul 2021 20:25:18 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Wed, 14 Jul 2021 20:25:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:26:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:26:01 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:26:01 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:26:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:26:02 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:26:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b95c16c5624058c7516ccc9aff7fcb6ab05fd66e5e47c1228f4d1e8fec58b`  
		Last Modified: Thu, 08 Jul 2021 22:40:47 GMT  
		Size: 21.5 MB (21468025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596bd4a64fddd48add80e9f5ee6459a223843aacedfe89c777ed62847e9b45e`  
		Last Modified: Thu, 08 Jul 2021 22:40:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7eae1b0e301a4bb2e1dc9e8faf695f6a25c25fa76af391234a420401b27365`  
		Last Modified: Wed, 14 Jul 2021 20:36:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267137a65ba8a2d9e353059d3da16877f506fa5ff13446e0445c0c4c3bcd784`  
		Last Modified: Wed, 14 Jul 2021 20:36:39 GMT  
		Size: 94.1 MB (94088312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443f532876e21e028bcb587e538fc650ce86a658794ac88dc47a19307ea98e3c`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2e5bbb56b3693c8317028271070258892c483ef1b2d9c0029cbd6d9788595d`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d9073f85635b6e855482f3fb205876b8d7623e0e0b2d0477f00f3f8a93e121`  
		Last Modified: Wed, 14 Jul 2021 20:36:22 GMT  
		Size: 2.7 MB (2747699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c2f3d2afd7b0a0978553d8a765d905c04663f3a050c334496ae656c755c4af`  
		Last Modified: Wed, 14 Jul 2021 20:36:27 GMT  
		Size: 48.6 MB (48630681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cf6faa89c3fe5437d036e3116d55e5185e803f18d486ae7510374d0c6a081d`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; arm variant v5

```console
$ docker pull redmine@sha256:f702db399231e0243f954b0787c2ff9dd1d59693d7f2e02dcbbe13e28220a194
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210649712 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cb0b3c9b3e19e2130c8ace0dc71dfd0bdd7b558fa946ac25771b4e51150df1b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:06:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:06:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:26:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:16:44 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:16:45 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:28:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:29:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:29:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:29:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:29:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:29:03 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:39:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:41:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:41:02 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:41:03 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:41:03 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:41:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:41:05 GMT
ENV REDMINE_VERSION=4.1.3
# Thu, 08 Jul 2021 22:41:06 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Thu, 08 Jul 2021 22:41:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:46:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:46:49 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:46:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:46:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:46:50 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:46:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b3ba0f03212caacd2191837bdac2f1a9abf399938b4020b315e4c6ea7ba0c7`  
		Last Modified: Wed, 23 Jun 2021 14:05:28 GMT  
		Size: 10.3 MB (10345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfab7796870f80c9db896239384ac194808f4ce5fab9f16ba155559772cc1e`  
		Last Modified: Wed, 23 Jun 2021 14:05:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7534381e53bd89c246e0ccb2c35dac17bf88c731c8d0526c63e59be51e884c`  
		Last Modified: Thu, 08 Jul 2021 20:44:48 GMT  
		Size: 20.7 MB (20733354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f2a9ffe5b789dd841f07056ea0122491118e78120d0f014d80085c602ab19c`  
		Last Modified: Thu, 08 Jul 2021 20:44:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f907c18a99e2058cc185b62d06d2138efee18b95ce1a7a7cdb625a9f526d704`  
		Last Modified: Thu, 08 Jul 2021 22:56:41 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9853b9e735dbc222e0627de3e38803e7f55197c1db1486b45a0acf6a829385`  
		Last Modified: Thu, 08 Jul 2021 22:57:45 GMT  
		Size: 89.6 MB (89575898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0be406a40fb9c97009fbc9316f6c0e5c1b079ae448337b08319d2fa80f9002`  
		Last Modified: Thu, 08 Jul 2021 22:56:39 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:671df9eb690f6e5280275ad105884d35b80fca5608d9ee7bb9b6cff80c5fa113`  
		Last Modified: Thu, 08 Jul 2021 22:56:39 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01ba8c671508e4cc58e6d481f258e99775cc5c1086a7425a5adf0955191b6b3d`  
		Last Modified: Thu, 08 Jul 2021 22:56:42 GMT  
		Size: 2.7 MB (2747694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265dac386bdcb11bef4564c82f342485592b05218eaf2f3c2d9a23f2fe54c742`  
		Last Modified: Thu, 08 Jul 2021 22:57:08 GMT  
		Size: 62.4 MB (62363772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d45cf3cc04e0538f87ced4ea51421b041406ea6346a9feaae13ccaf61bebcd5a`  
		Last Modified: Thu, 08 Jul 2021 22:56:39 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; arm variant v7

```console
$ docker pull redmine@sha256:f98e169cbbbd1e69e7b99c2d2e5afd65fc506a2a4a0ba960712a23c5c0f7d168
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203830355 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03c42097246ae6c0497adef62152905fc8745b6948196e85d759c355b92e114d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 23:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 23:18:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 23:18:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 23:58:55 GMT
ENV RUBY_MAJOR=2.6
# Thu, 08 Jul 2021 00:04:37 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 08 Jul 2021 00:04:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:55:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:56:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:56:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:56:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:56:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:56:03 GMT
CMD ["irb"]
# Fri, 09 Jul 2021 04:13:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 09 Jul 2021 04:14:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 04:14:18 GMT
ENV RAILS_ENV=production
# Fri, 09 Jul 2021 04:14:18 GMT
WORKDIR /usr/src/redmine
# Fri, 09 Jul 2021 04:14:19 GMT
ENV HOME=/home/redmine
# Fri, 09 Jul 2021 04:14:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 09 Jul 2021 04:14:21 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 09 Jul 2021 04:14:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 09 Jul 2021 04:14:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 09 Jul 2021 04:19:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 09 Jul 2021 04:19:42 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 09 Jul 2021 04:19:43 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 09 Jul 2021 04:19:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 09 Jul 2021 04:19:44 GMT
EXPOSE 3000
# Fri, 09 Jul 2021 04:19:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b763290fb30bc16e505b4aa06ba1c3041182ac9bd8be48df5e94cbbe8545d`  
		Last Modified: Thu, 24 Jun 2021 00:49:52 GMT  
		Size: 9.9 MB (9872206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f611d0cebec7d01271526d00ff39f508174641d4e952ac4954fb89f368bf331`  
		Last Modified: Thu, 24 Jun 2021 00:49:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae3ab28fbce4cee595eb301139ed362bf539fc80d87e1203e0c2d53b9f30bd5`  
		Last Modified: Thu, 08 Jul 2021 23:21:22 GMT  
		Size: 20.6 MB (20643638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7253813058a0314e3fee8530b64e5f281a4697fd64c8d4f59d4d3c1e02f8b2`  
		Last Modified: Thu, 08 Jul 2021 23:21:13 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9859eb1b9e2938ba6951e9b38fb78acaaa4383e0570cc02e2b62523694adf9dd`  
		Last Modified: Fri, 09 Jul 2021 04:28:57 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e657e10c5e16645f5a4f752ea53919857cc3a3938ec16a933424e7b8c80b52a`  
		Last Modified: Fri, 09 Jul 2021 04:29:54 GMT  
		Size: 85.6 MB (85590488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c95828495eb16bece32e4866d6a2567c2b1808df4c04e5a6dc6e28656da6dcf3`  
		Last Modified: Fri, 09 Jul 2021 04:28:55 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cd1318e42fa39223bed7cfbf8dd58828a6cd038585f8f9b89036054e8169c9`  
		Last Modified: Fri, 09 Jul 2021 04:28:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8aa84af383ed755d6f8f6998abd7be83a7ef724a14e8a56ba36066d3115ba34`  
		Last Modified: Fri, 09 Jul 2021 04:28:59 GMT  
		Size: 2.7 MB (2747692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112271ea3d64d4644770487201a5a69033c1302c09cefd8bc945e4bdd3fdf54b`  
		Last Modified: Fri, 09 Jul 2021 04:29:26 GMT  
		Size: 62.2 MB (62226034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20e4b35ba129dfba514cc450ea03df0146e5a7831f3f9d5cf11843b8e014391`  
		Last Modified: Fri, 09 Jul 2021 04:28:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:de07cd2752ffade4ed0c1170de0477e4d2dd9b0ab3dd1a7a1b88a2a73c064bc1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217532051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a97dd6f537f78477580e3d7cf8f95723ecc7fcbc8b3d94394e8bb4789ceb9fed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:53:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 03:53:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 03:53:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 04:03:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 23:54:15 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 23:54:15 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:55:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:55:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:55:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:55:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:55:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:55:12 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 23:24:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 23:24:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 23:24:22 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 23:24:22 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 23:24:22 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 23:24:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 23:24:23 GMT
ENV REDMINE_VERSION=4.1.3
# Thu, 08 Jul 2021 23:24:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Thu, 08 Jul 2021 23:24:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 23:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 23:26:29 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 23:26:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 23:26:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 23:26:30 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 23:26:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f276f053f0cad4dbf0c339099f5dd135531eb3ffb0bccc09369e7b7391b18d72`  
		Last Modified: Wed, 23 Jun 2021 04:22:18 GMT  
		Size: 11.3 MB (11263062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863be1d4664c690cf3e71cf9494c9b590ce4781e8008aef05d7cf572b8feddcc`  
		Last Modified: Wed, 23 Jun 2021 04:22:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac66415307302b8ab292b3121af7b08354a3b8cdd3da935a6974c5a72434402d`  
		Last Modified: Thu, 08 Jul 2021 21:11:22 GMT  
		Size: 21.3 MB (21308810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a6b4a9d9bdbee57547a94063ad97358687fa8c834f32ae69bdbda7e30ae7f2`  
		Last Modified: Thu, 08 Jul 2021 21:11:20 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b848da2b7d2dc611df6b3a0f97805a3f84f9a37d2ed4c64297b3c6a599ff29`  
		Last Modified: Thu, 08 Jul 2021 23:30:27 GMT  
		Size: 1.7 KB (1749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554949a502335a2a91d95a53e82f90e17601b6a5d0da2a74f700b31b5f6e3a8a`  
		Last Modified: Thu, 08 Jul 2021 23:30:43 GMT  
		Size: 92.6 MB (92610181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a792ac4df99887c8831f90baafac41c8639b08181cec9388e7429011eb20348c`  
		Last Modified: Thu, 08 Jul 2021 23:30:25 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fbe99ccee1394d284c3ca7c7aea40a908b7d463e96728d1c82336776e8b2fd`  
		Last Modified: Thu, 08 Jul 2021 23:30:25 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4f7eb23c68ed546186ae3c1f2cd91b7f2111f5ae6b766b20d1e8a2c87e22319`  
		Last Modified: Thu, 08 Jul 2021 23:30:26 GMT  
		Size: 2.7 MB (2747696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2e671f454fbbf045db7d382bf48f64118acdc5436869c619f904a16a8dd87b`  
		Last Modified: Thu, 08 Jul 2021 23:30:33 GMT  
		Size: 63.7 MB (63683060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e1e8a3621686b595efaede73f25979044b720ec8e83d05f1174f0d59f8a048`  
		Last Modified: Thu, 08 Jul 2021 23:30:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; 386

```console
$ docker pull redmine@sha256:2e14e83e20d1408e0e2108c2b18b45eba248c368fe7b9fd0772f014d90e669ad
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213005188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56761260ee9dfd0db61d52a675d87f0ebde983702c471ab0820e99cadca4e1ab`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:33:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:33:25 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:49:20 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:19:42 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:19:42 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 20:13:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:13:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:13:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:13:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:13:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:13:41 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:48:29 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:48:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:49:00 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:49:00 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:49:00 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:49:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:49:02 GMT
ENV REDMINE_VERSION=4.1.3
# Thu, 08 Jul 2021 22:49:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Thu, 08 Jul 2021 22:49:05 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:49:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:49:55 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:49:55 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:49:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:49:55 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:49:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb2041b26a9335dbdc8e6cc9bd945661b43317eb0de6d4e1e8ce82275cbea6`  
		Last Modified: Wed, 23 Jun 2021 14:14:04 GMT  
		Size: 17.2 MB (17227420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c89206098d37979fca1f31ba315796953128b80660adc5194c5541f0ac3f34`  
		Last Modified: Wed, 23 Jun 2021 14:13:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207bc054547d2959d625941a3d713cbac274d3fde559874ce3f103742021fcd0`  
		Last Modified: Thu, 08 Jul 2021 20:36:03 GMT  
		Size: 20.9 MB (20910220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bf234722053e694517615663f536b0761cb76a5ba09b68a3c42f05280985c5`  
		Last Modified: Thu, 08 Jul 2021 20:35:59 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddd76acb28134714ff2ba2109219219a0b06c2f49c2942ba8183f19f18dc444`  
		Last Modified: Thu, 08 Jul 2021 22:54:17 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fcbd90475437342f2a203b5d50b579606260b8df5b6bb44e97838424449c174`  
		Last Modified: Thu, 08 Jul 2021 22:54:39 GMT  
		Size: 95.7 MB (95701755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2637680a5b95a8d2bca3c146d25ef9d9ce4df35e84a9424ac9fad1df6452187`  
		Last Modified: Thu, 08 Jul 2021 22:54:14 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b3edc1a7cb5e5c17408b31a4dcb0d8abab5a18e903bf6c0865d2ed3000b8d8`  
		Last Modified: Thu, 08 Jul 2021 22:54:14 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce4e35470521f4474417b529d73651e68fa3c7b1a66b3f9e24e4d78428d1864`  
		Last Modified: Thu, 08 Jul 2021 22:54:16 GMT  
		Size: 2.7 MB (2747687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a0de80af3eeba8f8b14edd03cc1a78bc618e037ac0ef8365a167556fbb5a80`  
		Last Modified: Thu, 08 Jul 2021 22:54:23 GMT  
		Size: 48.6 MB (48616454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f132a96251c7173e4b6d07e6a3e69105aa6099d08fe84d05dacef4837f7caa3`  
		Last Modified: Thu, 08 Jul 2021 22:54:14 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; ppc64le

```console
$ docker pull redmine@sha256:64883bedbcb8390e549569df03596c1592c1f1cf09100882a2adb30a7464f677
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234101304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071cf966f6433307edcd7bc665b2280f5ebfbd80d77ba532b25a07b3f3be3508`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 17:21:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 17:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Jul 2021 17:22:32 GMT
ENV LANG=C.UTF-8
# Sat, 10 Jul 2021 18:06:39 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Jul 2021 18:06:44 GMT
ENV RUBY_VERSION=2.6.8
# Sat, 10 Jul 2021 18:06:50 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Sat, 10 Jul 2021 18:17:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Jul 2021 18:17:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Jul 2021 18:17:31 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Jul 2021 18:17:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Jul 2021 18:17:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Jul 2021 18:17:54 GMT
CMD ["irb"]
# Sun, 11 Jul 2021 07:36:19 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Jul 2021 07:42:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 07:42:53 GMT
ENV RAILS_ENV=production
# Sun, 11 Jul 2021 07:42:59 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Jul 2021 07:43:08 GMT
ENV HOME=/home/redmine
# Sun, 11 Jul 2021 07:43:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Jul 2021 07:43:28 GMT
ENV REDMINE_VERSION=4.1.3
# Sun, 11 Jul 2021 07:43:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Sun, 11 Jul 2021 07:43:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Jul 2021 07:50:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Jul 2021 07:50:20 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Jul 2021 07:50:24 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Jul 2021 07:50:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Jul 2021 07:50:31 GMT
EXPOSE 3000
# Sun, 11 Jul 2021 07:50:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba063dbcdd8aa55ec2183194edae6ea424d440c8c3c4ab57e29bdc8d30739f`  
		Last Modified: Sat, 10 Jul 2021 18:24:25 GMT  
		Size: 12.7 MB (12704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302bed40ec71d6898df63835eb0d9463b4672fcb74c6d77594621b1a9d96089b`  
		Last Modified: Sat, 10 Jul 2021 18:24:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae8fcb5d02ee6d84244d4abd42aa33daa130c38c85615ab4a4d0874e18a3233`  
		Last Modified: Sat, 10 Jul 2021 18:26:36 GMT  
		Size: 22.0 MB (21985630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0cda1836341e17f7519b587492ca37a7b447a8d6bfd60379f598076d411808`  
		Last Modified: Sat, 10 Jul 2021 18:26:32 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb446246ffeeee02507224564d47d57ef17f685a687ec77a197148e4ca919d6d`  
		Last Modified: Sun, 11 Jul 2021 08:16:17 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b12db92ff7b3432686c3cfeb8bf4e0c17267325be39418f465e7dad91e61c85`  
		Last Modified: Sun, 11 Jul 2021 08:16:37 GMT  
		Size: 101.3 MB (101328108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcd9eae2a479db34f85b60dabb3c448541cf492a571c4bdf5ad96980eea4f24`  
		Last Modified: Sun, 11 Jul 2021 08:16:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d325149e44e852ef5c9117755d729156ad8f55cef5f63d673a10ac82b188f346`  
		Last Modified: Sun, 11 Jul 2021 08:16:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a42445324d562b4682195c2466cae731ce845ea83e4cb2c45d1e89d24b08fb2`  
		Last Modified: Sun, 11 Jul 2021 08:16:14 GMT  
		Size: 2.7 MB (2747692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924db074ef0d503477ef377086ba7d8dc65a4cd537fbcdb51c9c43b626cf3a86`  
		Last Modified: Sun, 11 Jul 2021 08:16:23 GMT  
		Size: 64.8 MB (64777609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:243901ca86f6ec755dec21a70a11d89574c9d8a34cabd75fb30158f18034f7f4`  
		Last Modified: Sun, 11 Jul 2021 08:16:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; s390x

```console
$ docker pull redmine@sha256:56f544d99f465a37892af1c1f1e4a46510ead3d9cf83cbbb015a983eaf22a49d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216896693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:519746193a5092cc036db7e6c4987f1f2d362ffc2e3a80325935ca32b17d3803`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:56:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:56:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 09 Jul 2021 03:56:46 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jul 2021 04:25:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 09 Jul 2021 04:25:02 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 09 Jul 2021 04:25:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 09 Jul 2021 04:28:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 09 Jul 2021 04:28:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 09 Jul 2021 04:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 09 Jul 2021 04:28:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Jul 2021 04:28:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 09 Jul 2021 04:28:27 GMT
CMD ["irb"]
# Sat, 10 Jul 2021 04:03:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Jul 2021 04:05:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 04:05:23 GMT
ENV RAILS_ENV=production
# Sat, 10 Jul 2021 04:05:23 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Jul 2021 04:05:24 GMT
ENV HOME=/home/redmine
# Sat, 10 Jul 2021 04:05:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Jul 2021 04:05:27 GMT
ENV REDMINE_VERSION=4.1.3
# Sat, 10 Jul 2021 04:05:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Sat, 10 Jul 2021 04:05:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Jul 2021 04:08:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Jul 2021 04:08:32 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Jul 2021 04:08:33 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Jul 2021 04:08:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Jul 2021 04:08:34 GMT
EXPOSE 3000
# Sat, 10 Jul 2021 04:08:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb0861b7843d74cdcb468db372740a5fbb65d1a7a489cd207e57603e23b308`  
		Last Modified: Fri, 09 Jul 2021 04:33:35 GMT  
		Size: 10.8 MB (10814494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b9cde22299f5aa53f8d9540f770e1b6ab0e6223d1d106df86a5a071f8f3ec`  
		Last Modified: Fri, 09 Jul 2021 04:33:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c567400e82e0da61d3cd0628acf038b1f660df828736d747c5f078bf89f66f`  
		Last Modified: Fri, 09 Jul 2021 04:34:45 GMT  
		Size: 21.6 MB (21620064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267c98f7b0020a56c2dea2572a1386e898081dfbd1aa8e5c5c7b637234b6106c`  
		Last Modified: Fri, 09 Jul 2021 04:34:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d2c26dc1f4a79e7f57138c4d60e18a1efefb76d1a68fea231523dd4f61280b`  
		Last Modified: Sat, 10 Jul 2021 04:15:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2023bcadbc7a0f004c2da93fb37351dc4c05dc9941da2c0a74b1cb355e6318f`  
		Last Modified: Sat, 10 Jul 2021 04:15:26 GMT  
		Size: 91.8 MB (91789480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be589db26f20104b7d0d51e59f22288748ef178271a3cb237668a9ba4e8e3873`  
		Last Modified: Sat, 10 Jul 2021 04:15:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af0e3df0ae2fc1b6ed5a432d063589f9801d348e673aa45eb2d7e9c2ee34edf`  
		Last Modified: Sat, 10 Jul 2021 04:15:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9790215cdf9ba47d2b3dcf055017f99e27dfb80491bd0dbf6a21e5081f3670df`  
		Last Modified: Sat, 10 Jul 2021 04:15:11 GMT  
		Size: 2.7 MB (2747692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e1c18585fbe6a261eb8691fe17fc2f7c39e71c91abe4849ff7a04f5dc2a06c`  
		Last Modified: Sat, 10 Jul 2021 04:15:17 GMT  
		Size: 64.2 MB (64159990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b73773553e88959f1468859ce50e418c31af41dda709211aaaf8f0ff48e50d`  
		Last Modified: Sat, 10 Jul 2021 04:15:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.3-alpine`

```console
$ docker pull redmine@sha256:ab4e088a86875b1b538344cd8bffecef2ae743209af62856f076991270196c4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1.3-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:6fc987ac3687a985a641ecc4ffeb66fae30dfe751d67d0b96c3d7b3a0dea4939
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161071838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c092b6a7e727cff2c4ca5d85fea3f0833a29b70489519ff6fa71c81e678f27c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 08 Jul 2021 21:57:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 08 Jul 2021 21:57:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 08 Jul 2021 21:57:30 GMT
ENV LANG=C.UTF-8
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_MAJOR=2.6
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 08 Jul 2021 22:33:03 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:35:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:35:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:35:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:35:59 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:26:37 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jul 2021 20:26:45 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 14 Jul 2021 20:26:46 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:26:46 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:26:46 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:26:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:26:48 GMT
ENV REDMINE_VERSION=4.1.3
# Wed, 14 Jul 2021 20:26:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Wed, 14 Jul 2021 20:26:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:26:52 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jul 2021 20:28:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jul 2021 20:28:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:28:54 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 14 Jul 2021 20:28:54 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:28:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:28:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b0ea69e9ed42c49b5af449b703a12a4d2f2e28d87905af6fcd903fdae5689`  
		Last Modified: Thu, 08 Jul 2021 22:38:46 GMT  
		Size: 3.6 MB (3581658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad656ed833315b61ea674706f32c2d18d7412c7120926442af57b9131ee72ee`  
		Last Modified: Thu, 08 Jul 2021 22:38:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2a9d07bc1851494b8935d8593efecfea98e2c4a4ff1c3eaf2e5319eb31cb3a2`  
		Last Modified: Thu, 08 Jul 2021 22:41:47 GMT  
		Size: 19.9 MB (19889336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34d50c8fd3318db7f0dbb1d50a8aa4e571ae4926440e66c07be861dd4685211d`  
		Last Modified: Thu, 08 Jul 2021 22:41:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e030b8560a875bcd9c87e7dd1c8faf94a9d48cf039ee0bf125017750cc802b`  
		Last Modified: Wed, 14 Jul 2021 20:37:07 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70c0006aa2ad99f9ffc9d729323dc4d6fe56017cf11735d341570e65864f6425`  
		Last Modified: Wed, 14 Jul 2021 20:37:17 GMT  
		Size: 69.5 MB (69526405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde1c41e26debfed4512ebfbeb0a14368410a36df9e8a30216966c830eee17ad`  
		Last Modified: Wed, 14 Jul 2021 20:37:04 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968695fc5116055ee483a173dbd08fdd5e9aba5dea28a955cdc730ae9f0bba52`  
		Last Modified: Wed, 14 Jul 2021 20:37:04 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53f9412f7e58bd4742f678cd456ad14d8788771c9f2bd64676be5ef15102d32c`  
		Last Modified: Wed, 14 Jul 2021 20:37:05 GMT  
		Size: 2.7 MB (2748565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ce5851323b28845c755def36a5d70eb4eb98b968fb1d0bf274beba4b0ee408`  
		Last Modified: Wed, 14 Jul 2021 20:37:10 GMT  
		Size: 62.5 MB (62510175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553a89009171bdde8e1ac3c30cb9283a86cc357db925559833d12fd7c7b7d93d`  
		Last Modified: Wed, 14 Jul 2021 20:37:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.3-passenger`

```console
$ docker pull redmine@sha256:4334cb7c8b95d9668f01fc9f8c8ffdd56b40964b7a4a82b0cb4eb6a3f9c74e72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1.3-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:c1430615177875a68f1379e64e7c5bd75a780909650fb68487080cac12f38df2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232889438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2326128b089e53f55073cb580d592df8870f42e043d8f35b9c44a1fc630a160f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:20:10 GMT
ENV RUBY_MAJOR=2.6
# Wed, 07 Jul 2021 19:55:24 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 07 Jul 2021 19:55:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 08 Jul 2021 22:24:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:24:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:24:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:24:36 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:24:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:25:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:25:16 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:25:16 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:25:16 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:25:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:25:17 GMT
ENV REDMINE_VERSION=4.1.3
# Wed, 14 Jul 2021 20:25:18 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Wed, 14 Jul 2021 20:25:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:26:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:26:01 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:26:01 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:26:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:26:02 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:26:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:26:14 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:26:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:26:33 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:26:33 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:26:33 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6b95c16c5624058c7516ccc9aff7fcb6ab05fd66e5e47c1228f4d1e8fec58b`  
		Last Modified: Thu, 08 Jul 2021 22:40:47 GMT  
		Size: 21.5 MB (21468025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0596bd4a64fddd48add80e9f5ee6459a223843aacedfe89c777ed62847e9b45e`  
		Last Modified: Thu, 08 Jul 2021 22:40:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7eae1b0e301a4bb2e1dc9e8faf695f6a25c25fa76af391234a420401b27365`  
		Last Modified: Wed, 14 Jul 2021 20:36:24 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c267137a65ba8a2d9e353059d3da16877f506fa5ff13446e0445c0c4c3bcd784`  
		Last Modified: Wed, 14 Jul 2021 20:36:39 GMT  
		Size: 94.1 MB (94088312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443f532876e21e028bcb587e538fc650ce86a658794ac88dc47a19307ea98e3c`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2e5bbb56b3693c8317028271070258892c483ef1b2d9c0029cbd6d9788595d`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d9073f85635b6e855482f3fb205876b8d7623e0e0b2d0477f00f3f8a93e121`  
		Last Modified: Wed, 14 Jul 2021 20:36:22 GMT  
		Size: 2.7 MB (2747699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c2f3d2afd7b0a0978553d8a765d905c04663f3a050c334496ae656c755c4af`  
		Last Modified: Wed, 14 Jul 2021 20:36:27 GMT  
		Size: 48.6 MB (48630681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cf6faa89c3fe5437d036e3116d55e5185e803f18d486ae7510374d0c6a081d`  
		Last Modified: Wed, 14 Jul 2021 20:36:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf013518a02ee1e21f728797726c8cd338e36dc5f93a2ca79d2e219176ab2cdf`  
		Last Modified: Wed, 14 Jul 2021 20:36:53 GMT  
		Size: 21.3 MB (21322651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39d8dc1a16c759aa15798aa8cbca04ff8c4532a0be26e406f4f4db28aa7d4bd`  
		Last Modified: Wed, 14 Jul 2021 20:36:50 GMT  
		Size: 4.9 MB (4919285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2`

```console
$ docker pull redmine@sha256:cae6a4d4227606764c6a75b180a5b675e4d7415888b5a1261069761a7cd84eac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.2` - linux; amd64

```console
$ docker pull redmine@sha256:c303bc0f5596613dabea4516d47172296178fa21f6db17497624805f778cb357
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195475758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:338c47d4bca896733efe021ec38c0d595cf043de470eba5e45d6e3dde1a485c3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v5

```console
$ docker pull redmine@sha256:504785f157b11fc0cf462141bdae1564241f3417ea1c8371d3c2e4c7dd41c552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196972163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217c8956d29925ec9e63ffbf48e3d04a71ec25911566cd968e65a03abbcef198`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:06:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:06:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:17:20 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:05:54 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:05:55 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:19:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:19:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:20:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:20:00 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:20:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:20:03 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:32:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:33:44 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:33:45 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:33:45 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:33:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:33:48 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 22:33:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 22:33:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:39:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:39:30 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:39:30 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:39:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:39:32 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:39:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b3ba0f03212caacd2191837bdac2f1a9abf399938b4020b315e4c6ea7ba0c7`  
		Last Modified: Wed, 23 Jun 2021 14:05:28 GMT  
		Size: 10.3 MB (10345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfab7796870f80c9db896239384ac194808f4ce5fab9f16ba155559772cc1e`  
		Last Modified: Wed, 23 Jun 2021 14:05:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4340642939f48d099081c75a2712db898b9985ae54a619b2452aac1d6d5811`  
		Last Modified: Thu, 08 Jul 2021 20:43:39 GMT  
		Size: 13.9 MB (13871335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695fcd3bc334ffbc54deec488d9db9eda8fec160e0a45fb2eaf1cb3c40fe5d17`  
		Last Modified: Thu, 08 Jul 2021 20:43:31 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e84c1768026dd91ab7c8b588e6bca6eb786ae29dbdbcb5cfe9942272bcfc56b`  
		Last Modified: Thu, 08 Jul 2021 22:55:15 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7075123429263b675529579bcba18589d90fc77e59eb5919484dedb6d1c64c1f`  
		Last Modified: Thu, 08 Jul 2021 22:56:17 GMT  
		Size: 89.6 MB (89576320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e64c6c915303586fcbdb5e1921c304efd17cae07d4aabc1d6ebae70a889fd8`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b203953be51a5b5e20215561ddbcf8db375b9ca69dd0f7ba4d114fa962f6d7d`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ac40a10c440649c65c501f24a90d153143ce98bcf9b9bf731f6e22a347570`  
		Last Modified: Thu, 08 Jul 2021 22:55:17 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14230d92bd82d511c4f7398fd0d256fb2c88bc9039691884c1a0a90a6b9b7d56`  
		Last Modified: Thu, 08 Jul 2021 22:55:35 GMT  
		Size: 55.2 MB (55236836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eea4df7ac799e61a3b26a4195f6641617e2e656b4b38cd6c47240821584be3`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:918c928c44808884e8f314ba4798c35f6c33f66f3af9808185b7cb6632829c4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4523ba6f474f4b705844d9e15d89345a8277bfdbf939337c277171f2733bc896`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 23:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 23:18:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 23:18:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 23:36:25 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 23:43:24 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 23:43:24 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:35:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:35:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:35:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:35:12 GMT
CMD ["irb"]
# Fri, 09 Jul 2021 04:06:25 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 09 Jul 2021 04:07:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 04:07:27 GMT
ENV RAILS_ENV=production
# Fri, 09 Jul 2021 04:07:27 GMT
WORKDIR /usr/src/redmine
# Fri, 09 Jul 2021 04:07:28 GMT
ENV HOME=/home/redmine
# Fri, 09 Jul 2021 04:07:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 09 Jul 2021 04:07:30 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 09 Jul 2021 04:07:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 09 Jul 2021 04:07:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 09 Jul 2021 04:12:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 09 Jul 2021 04:12:52 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 09 Jul 2021 04:12:53 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 09 Jul 2021 04:12:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 09 Jul 2021 04:12:54 GMT
EXPOSE 3000
# Fri, 09 Jul 2021 04:12:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b763290fb30bc16e505b4aa06ba1c3041182ac9bd8be48df5e94cbbe8545d`  
		Last Modified: Thu, 24 Jun 2021 00:49:52 GMT  
		Size: 9.9 MB (9872206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f611d0cebec7d01271526d00ff39f508174641d4e952ac4954fb89f368bf331`  
		Last Modified: Thu, 24 Jun 2021 00:49:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c081e6813d08a36724de201912dcf2049b4b63e901379b09265fff1f204332`  
		Last Modified: Thu, 08 Jul 2021 23:20:14 GMT  
		Size: 13.8 MB (13766804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47e03b2ecd26a74249ee57a56b50a959f58fbcaca622b530a671eca71a7384d`  
		Last Modified: Thu, 08 Jul 2021 23:20:07 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5ad0520989f495616ff11a4e507a10e68c9135a8387cf52dfca8fefd1fa348`  
		Last Modified: Fri, 09 Jul 2021 04:27:36 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23a4b1761119307dc0dd899befff1a28684d45a780a3b964aef62e5ea8c5147`  
		Last Modified: Fri, 09 Jul 2021 04:28:33 GMT  
		Size: 85.6 MB (85590504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089aa8086891a0e5b87d68a89f8621e084085b5786ee8e0c05539a337161a184`  
		Last Modified: Fri, 09 Jul 2021 04:27:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57d7596e26caaeafa01d35cfbd470f7a013b174e7c5c25852729c10b10448c`  
		Last Modified: Fri, 09 Jul 2021 04:27:33 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2efb117cd99001cc83a98b5a1277459f26c1b985c59ae03866ca74c7d1380`  
		Last Modified: Fri, 09 Jul 2021 04:27:38 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ab3b3250933a12c6c93d662c3198824bef82b64f0d7f119675b68e1cec76a6`  
		Last Modified: Fri, 09 Jul 2021 04:27:59 GMT  
		Size: 55.1 MB (55076972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3916fdc65621036c0f5ddd98394f1e47796b2f19531e4ab24c86648449214c16`  
		Last Modified: Fri, 09 Jul 2021 04:27:33 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:0741f6999c4d2a4e13afe1af9a34785c48f61a2feb89930198909593b569e246
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203231922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3d2c5023b434e055c0449d22553bc2ecc42a9e53a462c79fada428177c6180`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:53:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 03:53:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 03:53:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 03:58:54 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 23:45:12 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 23:45:13 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:45:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:45:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:45:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:45:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:45:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:45:29 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 23:21:02 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 23:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 23:21:24 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 23:21:25 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 23:21:25 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 23:21:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 23:21:26 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 23:21:26 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 23:21:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 23:23:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 23:23:52 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 23:23:53 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 23:23:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 23:23:53 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 23:23:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f276f053f0cad4dbf0c339099f5dd135531eb3ffb0bccc09369e7b7391b18d72`  
		Last Modified: Wed, 23 Jun 2021 04:22:18 GMT  
		Size: 11.3 MB (11263062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863be1d4664c690cf3e71cf9494c9b590ce4781e8008aef05d7cf572b8feddcc`  
		Last Modified: Wed, 23 Jun 2021 04:22:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f5d2c58688ac84743d00ab7bbdc6b4093e20d9a833d6af3496cc62e935a25`  
		Last Modified: Thu, 08 Jul 2021 21:09:46 GMT  
		Size: 14.4 MB (14356604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4dfdc14b449c213e94db8cd01bdfa232be4fa72040ffeebb4ea881ffa8634`  
		Last Modified: Thu, 08 Jul 2021 21:09:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df641efdceaa2aee736b0b2ed3580d9cc12941e9d5b47754238e2832b4290d`  
		Last Modified: Thu, 08 Jul 2021 23:29:47 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e08f5ce73ad17307002bfba119f4a63a0edae9959555829f15c37ec8f76c2`  
		Last Modified: Thu, 08 Jul 2021 23:30:04 GMT  
		Size: 92.6 MB (92610656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4765b269f180b2c2704772dd7d776ea01a9075ed5d1d8cd8f0882ca083129c2c`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6329e48a16d3a91d290cfbae3c0a552cfe96c6b792fcb231df35ff3c039a1`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feadd8be638a909710f31206aa67f01ca6d2a8ebec560b39b0dc3523c0211f6`  
		Last Modified: Thu, 08 Jul 2021 23:29:46 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5a01cee6465420071dfb449649aebee78fb947eecd0b3b279df2405c1c4d9d`  
		Last Modified: Thu, 08 Jul 2021 23:29:51 GMT  
		Size: 56.0 MB (56023674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbbcb4d6ad95bc21ed907d86fa7e683a21628ed441ad64f891f7322fc156b12`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; 386

```console
$ docker pull redmine@sha256:38c75a4b236bb825b9ee8fa35034d33dab94661ce6f8ce26c59869e809aa60ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202116586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cab517b8b53a6715a276de085b7d54ac6b3054ed3ee985c2ec4022d275a36e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:33:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:33:25 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:42:41 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:08:54 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:08:54 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:01:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:01:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:01:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:01:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:01:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:01:08 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:46:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:47:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:47:20 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:47:20 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:47:20 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:47:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:47:21 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 22:47:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 22:47:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:48:13 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:48:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:48:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:48:14 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:48:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb2041b26a9335dbdc8e6cc9bd945661b43317eb0de6d4e1e8ce82275cbea6`  
		Last Modified: Wed, 23 Jun 2021 14:14:04 GMT  
		Size: 17.2 MB (17227420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c89206098d37979fca1f31ba315796953128b80660adc5194c5541f0ac3f34`  
		Last Modified: Wed, 23 Jun 2021 14:13:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce027bc021a8f988e98283d7e7edb0812da70bec1469306b760a90237fb460ac`  
		Last Modified: Thu, 08 Jul 2021 20:34:09 GMT  
		Size: 14.0 MB (13991996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f914d412069980e7e91c9e3b27cd62e1d17cffdd9dd8b8d86e009a47a54d257`  
		Last Modified: Thu, 08 Jul 2021 20:34:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ddcca7d90497767f04b499a232298ba4b6b367a55fc644281d45884b4904c4`  
		Last Modified: Thu, 08 Jul 2021 22:53:29 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a07456067d7c014c80d85bba6d608010bf9baaa1cbf62bfefc070f9e197d5`  
		Last Modified: Thu, 08 Jul 2021 22:53:53 GMT  
		Size: 95.7 MB (95703052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b637a32b9c8c0c921586600afc7d5867c46a31465bbb953d9f07412725c8f280`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe31a7355aa80ea3975b5e2ea081a34279b494c8636489851f5bb2adabbb9ba9`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc4f8125c232b162083e88887968149ff3e94b419b661c0c98ab1c249ae8e82`  
		Last Modified: Thu, 08 Jul 2021 22:53:28 GMT  
		Size: 3.1 MB (3058670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c938aebe09af0b44a41d919513d737720f30afcb71bcdfe7ff6ed289be406cdb`  
		Last Modified: Thu, 08 Jul 2021 22:53:34 GMT  
		Size: 44.3 MB (44333801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2250ccc831a8ba36b5f9238e570ea872df977ed50651174c22510dcdc699d`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; ppc64le

```console
$ docker pull redmine@sha256:8fb1ccf561c68fe89d8bcbae5ff084cf0abd84fd2363b4ec1789794b2dbc7a31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219629876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5d606a69ac811e24028853731ce3876c2081c9926124809b5369c40d3e38d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 17:21:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 17:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Jul 2021 17:22:32 GMT
ENV LANG=C.UTF-8
# Sat, 10 Jul 2021 17:45:35 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Jul 2021 17:45:38 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 10 Jul 2021 17:45:45 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 10 Jul 2021 17:57:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Jul 2021 17:57:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Jul 2021 17:57:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Jul 2021 17:57:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Jul 2021 17:57:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Jul 2021 17:57:59 GMT
CMD ["irb"]
# Sun, 11 Jul 2021 07:19:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Jul 2021 07:27:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 07:27:27 GMT
ENV RAILS_ENV=production
# Sun, 11 Jul 2021 07:27:31 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Jul 2021 07:27:38 GMT
ENV HOME=/home/redmine
# Sun, 11 Jul 2021 07:27:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Jul 2021 07:27:56 GMT
ENV REDMINE_VERSION=4.2.1
# Sun, 11 Jul 2021 07:27:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Sun, 11 Jul 2021 07:28:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Jul 2021 07:35:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Jul 2021 07:35:26 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Jul 2021 07:35:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Jul 2021 07:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Jul 2021 07:35:45 GMT
EXPOSE 3000
# Sun, 11 Jul 2021 07:35:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba063dbcdd8aa55ec2183194edae6ea424d440c8c3c4ab57e29bdc8d30739f`  
		Last Modified: Sat, 10 Jul 2021 18:24:25 GMT  
		Size: 12.7 MB (12704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302bed40ec71d6898df63835eb0d9463b4672fcb74c6d77594621b1a9d96089b`  
		Last Modified: Sat, 10 Jul 2021 18:24:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d142b79f0a553ffa66e8c2525798e544895249d98562aa21710905ebcdc6ed`  
		Last Modified: Sat, 10 Jul 2021 18:25:40 GMT  
		Size: 15.0 MB (14997790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3641aa4022fa299e9c8ba11982ead0ef3ba6b4e176be30a9d1f232615c99c`  
		Last Modified: Sat, 10 Jul 2021 18:25:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4804b39acc72bb6d81a7bfc7c05f56e803d5b3e9d2ed1c298bbd2eb44c7e5356`  
		Last Modified: Sun, 11 Jul 2021 08:15:25 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9073dd583be35eadb9e9e25a07f78b0a111fca6d47e69f14431eeb4b81f0682a`  
		Last Modified: Sun, 11 Jul 2021 08:15:45 GMT  
		Size: 101.3 MB (101327909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae14e6cdfd8bc5a68ed3c6f67843101b5677d40266ab29f2da8d3c24724ad20`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346cf33cfa1c3ae728b01723b2eacfc89d22db906bbb468ad356ffe6f80188b8`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4551ad703a6bab86fb1132fc6ecfd00620f4079d4d10d5c9d3f6b78a66d698a0`  
		Last Modified: Sun, 11 Jul 2021 08:15:22 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f790f7d0d86286c2d1129fa246d6eb23d09db45923ec78d8d0e2402cfd8660`  
		Last Modified: Sun, 11 Jul 2021 08:15:30 GMT  
		Size: 57.0 MB (56983237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dff610884a2816b07cde2af44a25989e11404807fe565fed2cee5ba172a03bc`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; s390x

```console
$ docker pull redmine@sha256:73d6f4443ca8fb63dbad4f2d16c45bd208f75b21472cd8dd96cc1307bd1e2773
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202549125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f90d1267f56ffe9dd1410a3837ccbf93c9da343fe9ff0a822248352eaeb441`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:56:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:56:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 09 Jul 2021 03:56:46 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jul 2021 04:10:42 GMT
ENV RUBY_MAJOR=2.7
# Fri, 09 Jul 2021 04:10:43 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 09 Jul 2021 04:10:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 09 Jul 2021 04:13:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 09 Jul 2021 04:13:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 09 Jul 2021 04:13:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 09 Jul 2021 04:13:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Jul 2021 04:13:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 09 Jul 2021 04:13:29 GMT
CMD ["irb"]
# Sat, 10 Jul 2021 03:58:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Jul 2021 03:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 03:59:51 GMT
ENV RAILS_ENV=production
# Sat, 10 Jul 2021 03:59:51 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Jul 2021 03:59:52 GMT
ENV HOME=/home/redmine
# Sat, 10 Jul 2021 03:59:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Jul 2021 03:59:54 GMT
ENV REDMINE_VERSION=4.2.1
# Sat, 10 Jul 2021 03:59:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Sat, 10 Jul 2021 04:00:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Jul 2021 04:03:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Jul 2021 04:03:24 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Jul 2021 04:03:25 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Jul 2021 04:03:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Jul 2021 04:03:26 GMT
EXPOSE 3000
# Sat, 10 Jul 2021 04:03:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb0861b7843d74cdcb468db372740a5fbb65d1a7a489cd207e57603e23b308`  
		Last Modified: Fri, 09 Jul 2021 04:33:35 GMT  
		Size: 10.8 MB (10814494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b9cde22299f5aa53f8d9540f770e1b6ab0e6223d1d106df86a5a071f8f3ec`  
		Last Modified: Fri, 09 Jul 2021 04:33:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf70f667dcd7c81ea6676bf03ad1d287575af1b2eceb425583be290e010897d`  
		Last Modified: Fri, 09 Jul 2021 04:34:14 GMT  
		Size: 14.7 MB (14697234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db437741211099211d57153dd52a63267f0affc47f39380dcd6da3552b8d5d5`  
		Last Modified: Fri, 09 Jul 2021 04:34:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a890c47c8baf9911890e19680c177f40232d060ba3cb040b2769a783f1ef98`  
		Last Modified: Sat, 10 Jul 2021 04:14:43 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95693198ef1207b35d9efaf8262d24914419aa240f3df8e04fc6369e5dcb55d8`  
		Last Modified: Sat, 10 Jul 2021 04:14:57 GMT  
		Size: 91.8 MB (91789992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5150ba28aa600261d40392db78998b0639dce33fa135a4749a3e03046b57ab38`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6faf8f4361902faa3aab0a419eeb7f8819ad29e5e3daf830099ed96210ec9fe`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472586cc07848d25dd2f1f9438ec666dc78b643ede7d89344b5da229b412a5c3`  
		Last Modified: Sat, 10 Jul 2021 04:14:42 GMT  
		Size: 3.1 MB (3058671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384911646e488885a18a1fc8217f5f547cde94a5281986d7b69f117e363381ea`  
		Last Modified: Sat, 10 Jul 2021 04:14:46 GMT  
		Size: 56.4 MB (56423763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051ac5465ae61ddb401a283b21e69175949f1424f30cea6aa203408b2ea9c214`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-alpine`

```console
$ docker pull redmine@sha256:7de4015773da4d105b5f43705556003eb3071d781612fa6e7f6010981e4e56e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.2-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:7fb14bb9edbf56cf78406c149b3015cfd560d8ab4b036edebde5aa5e4b83f5af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150068908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74c717ce35a7872383b67fe6276f951c39395fcba0eda36625d7e2eaa9a32932`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 08 Jul 2021 21:57:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 08 Jul 2021 21:57:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 08 Jul 2021 21:57:30 GMT
ENV LANG=C.UTF-8
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_MAJOR=2.7
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:18:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:18:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:18:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:18:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:18:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:18:51 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:22:24 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jul 2021 20:22:32 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 14 Jul 2021 20:22:33 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:22:33 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:22:33 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:22:34 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:22:35 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:22:35 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:22:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:22:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jul 2021 20:24:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jul 2021 20:24:42 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:24:42 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 14 Jul 2021 20:24:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:24:42 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:24:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b0ea69e9ed42c49b5af449b703a12a4d2f2e28d87905af6fcd903fdae5689`  
		Last Modified: Thu, 08 Jul 2021 22:38:46 GMT  
		Size: 3.6 MB (3581658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad656ed833315b61ea674706f32c2d18d7412c7120926442af57b9131ee72ee`  
		Last Modified: Thu, 08 Jul 2021 22:38:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626f6830afc6fb7a05a8f18f2b98e4ea4db3d2dd50803e5cd2c627fe25150dc8`  
		Last Modified: Thu, 08 Jul 2021 22:40:13 GMT  
		Size: 14.4 MB (14373123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5375389679c9573d241b22905aee17b20981e2628989561698087f107fcfed4a`  
		Last Modified: Thu, 08 Jul 2021 22:40:11 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76a82132aeb154f32b80803eecedc3e27e062a35ae1e05284dc2d7e6c7f4f59`  
		Last Modified: Wed, 14 Jul 2021 20:35:42 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb4af997128346f54fa569d3a04180c718e02a90e90eff7161241d54deef92`  
		Last Modified: Wed, 14 Jul 2021 20:35:52 GMT  
		Size: 69.5 MB (69526214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14da2816c58ef08b826f823d7b6a4126bb63594ed1109880b795c28cc4d3f032`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f34be07349b94807cc58a0e31cecec279d0591b9a6f1f65f1dbe94a4713462`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b05ead31106734fcef5216d256a8536461fa7935f729e67262c90f55e683b`  
		Last Modified: Wed, 14 Jul 2021 20:35:40 GMT  
		Size: 3.1 MB (3060004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c586852175065725ae48c5682f1ecea003599fbc0028c3387f5de00cc28f34`  
		Last Modified: Wed, 14 Jul 2021 20:36:03 GMT  
		Size: 56.7 MB (56712212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d1559a239e3bf1260f693961d40d28b32673907100b077a797e55d543f072c`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-passenger`

```console
$ docker pull redmine@sha256:9b780f98151823e0e84e1e41974c548143cae7090cd367eb711d44d3bc8a966b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.2-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:a320947c8461cd8bafad0bcfda90b4f5ac840389345003324df81de7b46ad296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3049f679e04c98a7643e800733c59f85c960a686a186192d9b12a222bed1592`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:22:01 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:22:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:22:20 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:22:20 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:22:20 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41f4f9e9b7629be3e6e9666279b940b489648484da4e41725e7b22c1c94b1b`  
		Last Modified: Wed, 14 Jul 2021 20:35:22 GMT  
		Size: 21.1 MB (21131700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436698f0e4aec6d6e7c991fd623ae0d4eab48e62193c564b2fa25de8f4a52e`  
		Last Modified: Wed, 14 Jul 2021 20:35:20 GMT  
		Size: 4.9 MB (4919284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.1`

```console
$ docker pull redmine@sha256:cae6a4d4227606764c6a75b180a5b675e4d7415888b5a1261069761a7cd84eac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.2.1` - linux; amd64

```console
$ docker pull redmine@sha256:c303bc0f5596613dabea4516d47172296178fa21f6db17497624805f778cb357
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195475758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:338c47d4bca896733efe021ec38c0d595cf043de470eba5e45d6e3dde1a485c3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:504785f157b11fc0cf462141bdae1564241f3417ea1c8371d3c2e4c7dd41c552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196972163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217c8956d29925ec9e63ffbf48e3d04a71ec25911566cd968e65a03abbcef198`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:06:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:06:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:17:20 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:05:54 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:05:55 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:19:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:19:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:20:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:20:00 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:20:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:20:03 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:32:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:33:44 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:33:45 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:33:45 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:33:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:33:48 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 22:33:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 22:33:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:39:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:39:30 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:39:30 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:39:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:39:32 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:39:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b3ba0f03212caacd2191837bdac2f1a9abf399938b4020b315e4c6ea7ba0c7`  
		Last Modified: Wed, 23 Jun 2021 14:05:28 GMT  
		Size: 10.3 MB (10345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfab7796870f80c9db896239384ac194808f4ce5fab9f16ba155559772cc1e`  
		Last Modified: Wed, 23 Jun 2021 14:05:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4340642939f48d099081c75a2712db898b9985ae54a619b2452aac1d6d5811`  
		Last Modified: Thu, 08 Jul 2021 20:43:39 GMT  
		Size: 13.9 MB (13871335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695fcd3bc334ffbc54deec488d9db9eda8fec160e0a45fb2eaf1cb3c40fe5d17`  
		Last Modified: Thu, 08 Jul 2021 20:43:31 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e84c1768026dd91ab7c8b588e6bca6eb786ae29dbdbcb5cfe9942272bcfc56b`  
		Last Modified: Thu, 08 Jul 2021 22:55:15 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7075123429263b675529579bcba18589d90fc77e59eb5919484dedb6d1c64c1f`  
		Last Modified: Thu, 08 Jul 2021 22:56:17 GMT  
		Size: 89.6 MB (89576320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e64c6c915303586fcbdb5e1921c304efd17cae07d4aabc1d6ebae70a889fd8`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b203953be51a5b5e20215561ddbcf8db375b9ca69dd0f7ba4d114fa962f6d7d`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ac40a10c440649c65c501f24a90d153143ce98bcf9b9bf731f6e22a347570`  
		Last Modified: Thu, 08 Jul 2021 22:55:17 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14230d92bd82d511c4f7398fd0d256fb2c88bc9039691884c1a0a90a6b9b7d56`  
		Last Modified: Thu, 08 Jul 2021 22:55:35 GMT  
		Size: 55.2 MB (55236836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eea4df7ac799e61a3b26a4195f6641617e2e656b4b38cd6c47240821584be3`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:918c928c44808884e8f314ba4798c35f6c33f66f3af9808185b7cb6632829c4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4523ba6f474f4b705844d9e15d89345a8277bfdbf939337c277171f2733bc896`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 23:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 23:18:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 23:18:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 23:36:25 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 23:43:24 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 23:43:24 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:35:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:35:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:35:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:35:12 GMT
CMD ["irb"]
# Fri, 09 Jul 2021 04:06:25 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 09 Jul 2021 04:07:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 04:07:27 GMT
ENV RAILS_ENV=production
# Fri, 09 Jul 2021 04:07:27 GMT
WORKDIR /usr/src/redmine
# Fri, 09 Jul 2021 04:07:28 GMT
ENV HOME=/home/redmine
# Fri, 09 Jul 2021 04:07:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 09 Jul 2021 04:07:30 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 09 Jul 2021 04:07:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 09 Jul 2021 04:07:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 09 Jul 2021 04:12:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 09 Jul 2021 04:12:52 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 09 Jul 2021 04:12:53 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 09 Jul 2021 04:12:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 09 Jul 2021 04:12:54 GMT
EXPOSE 3000
# Fri, 09 Jul 2021 04:12:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b763290fb30bc16e505b4aa06ba1c3041182ac9bd8be48df5e94cbbe8545d`  
		Last Modified: Thu, 24 Jun 2021 00:49:52 GMT  
		Size: 9.9 MB (9872206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f611d0cebec7d01271526d00ff39f508174641d4e952ac4954fb89f368bf331`  
		Last Modified: Thu, 24 Jun 2021 00:49:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c081e6813d08a36724de201912dcf2049b4b63e901379b09265fff1f204332`  
		Last Modified: Thu, 08 Jul 2021 23:20:14 GMT  
		Size: 13.8 MB (13766804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47e03b2ecd26a74249ee57a56b50a959f58fbcaca622b530a671eca71a7384d`  
		Last Modified: Thu, 08 Jul 2021 23:20:07 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5ad0520989f495616ff11a4e507a10e68c9135a8387cf52dfca8fefd1fa348`  
		Last Modified: Fri, 09 Jul 2021 04:27:36 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23a4b1761119307dc0dd899befff1a28684d45a780a3b964aef62e5ea8c5147`  
		Last Modified: Fri, 09 Jul 2021 04:28:33 GMT  
		Size: 85.6 MB (85590504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089aa8086891a0e5b87d68a89f8621e084085b5786ee8e0c05539a337161a184`  
		Last Modified: Fri, 09 Jul 2021 04:27:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57d7596e26caaeafa01d35cfbd470f7a013b174e7c5c25852729c10b10448c`  
		Last Modified: Fri, 09 Jul 2021 04:27:33 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2efb117cd99001cc83a98b5a1277459f26c1b985c59ae03866ca74c7d1380`  
		Last Modified: Fri, 09 Jul 2021 04:27:38 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ab3b3250933a12c6c93d662c3198824bef82b64f0d7f119675b68e1cec76a6`  
		Last Modified: Fri, 09 Jul 2021 04:27:59 GMT  
		Size: 55.1 MB (55076972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3916fdc65621036c0f5ddd98394f1e47796b2f19531e4ab24c86648449214c16`  
		Last Modified: Fri, 09 Jul 2021 04:27:33 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:0741f6999c4d2a4e13afe1af9a34785c48f61a2feb89930198909593b569e246
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203231922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3d2c5023b434e055c0449d22553bc2ecc42a9e53a462c79fada428177c6180`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:53:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 03:53:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 03:53:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 03:58:54 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 23:45:12 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 23:45:13 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:45:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:45:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:45:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:45:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:45:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:45:29 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 23:21:02 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 23:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 23:21:24 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 23:21:25 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 23:21:25 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 23:21:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 23:21:26 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 23:21:26 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 23:21:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 23:23:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 23:23:52 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 23:23:53 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 23:23:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 23:23:53 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 23:23:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f276f053f0cad4dbf0c339099f5dd135531eb3ffb0bccc09369e7b7391b18d72`  
		Last Modified: Wed, 23 Jun 2021 04:22:18 GMT  
		Size: 11.3 MB (11263062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863be1d4664c690cf3e71cf9494c9b590ce4781e8008aef05d7cf572b8feddcc`  
		Last Modified: Wed, 23 Jun 2021 04:22:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f5d2c58688ac84743d00ab7bbdc6b4093e20d9a833d6af3496cc62e935a25`  
		Last Modified: Thu, 08 Jul 2021 21:09:46 GMT  
		Size: 14.4 MB (14356604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4dfdc14b449c213e94db8cd01bdfa232be4fa72040ffeebb4ea881ffa8634`  
		Last Modified: Thu, 08 Jul 2021 21:09:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df641efdceaa2aee736b0b2ed3580d9cc12941e9d5b47754238e2832b4290d`  
		Last Modified: Thu, 08 Jul 2021 23:29:47 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e08f5ce73ad17307002bfba119f4a63a0edae9959555829f15c37ec8f76c2`  
		Last Modified: Thu, 08 Jul 2021 23:30:04 GMT  
		Size: 92.6 MB (92610656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4765b269f180b2c2704772dd7d776ea01a9075ed5d1d8cd8f0882ca083129c2c`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6329e48a16d3a91d290cfbae3c0a552cfe96c6b792fcb231df35ff3c039a1`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feadd8be638a909710f31206aa67f01ca6d2a8ebec560b39b0dc3523c0211f6`  
		Last Modified: Thu, 08 Jul 2021 23:29:46 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5a01cee6465420071dfb449649aebee78fb947eecd0b3b279df2405c1c4d9d`  
		Last Modified: Thu, 08 Jul 2021 23:29:51 GMT  
		Size: 56.0 MB (56023674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbbcb4d6ad95bc21ed907d86fa7e683a21628ed441ad64f891f7322fc156b12`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; 386

```console
$ docker pull redmine@sha256:38c75a4b236bb825b9ee8fa35034d33dab94661ce6f8ce26c59869e809aa60ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202116586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cab517b8b53a6715a276de085b7d54ac6b3054ed3ee985c2ec4022d275a36e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:33:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:33:25 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:42:41 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:08:54 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:08:54 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:01:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:01:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:01:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:01:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:01:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:01:08 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:46:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:47:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:47:20 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:47:20 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:47:20 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:47:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:47:21 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 22:47:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 22:47:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:48:13 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:48:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:48:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:48:14 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:48:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb2041b26a9335dbdc8e6cc9bd945661b43317eb0de6d4e1e8ce82275cbea6`  
		Last Modified: Wed, 23 Jun 2021 14:14:04 GMT  
		Size: 17.2 MB (17227420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c89206098d37979fca1f31ba315796953128b80660adc5194c5541f0ac3f34`  
		Last Modified: Wed, 23 Jun 2021 14:13:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce027bc021a8f988e98283d7e7edb0812da70bec1469306b760a90237fb460ac`  
		Last Modified: Thu, 08 Jul 2021 20:34:09 GMT  
		Size: 14.0 MB (13991996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f914d412069980e7e91c9e3b27cd62e1d17cffdd9dd8b8d86e009a47a54d257`  
		Last Modified: Thu, 08 Jul 2021 20:34:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ddcca7d90497767f04b499a232298ba4b6b367a55fc644281d45884b4904c4`  
		Last Modified: Thu, 08 Jul 2021 22:53:29 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a07456067d7c014c80d85bba6d608010bf9baaa1cbf62bfefc070f9e197d5`  
		Last Modified: Thu, 08 Jul 2021 22:53:53 GMT  
		Size: 95.7 MB (95703052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b637a32b9c8c0c921586600afc7d5867c46a31465bbb953d9f07412725c8f280`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe31a7355aa80ea3975b5e2ea081a34279b494c8636489851f5bb2adabbb9ba9`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc4f8125c232b162083e88887968149ff3e94b419b661c0c98ab1c249ae8e82`  
		Last Modified: Thu, 08 Jul 2021 22:53:28 GMT  
		Size: 3.1 MB (3058670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c938aebe09af0b44a41d919513d737720f30afcb71bcdfe7ff6ed289be406cdb`  
		Last Modified: Thu, 08 Jul 2021 22:53:34 GMT  
		Size: 44.3 MB (44333801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2250ccc831a8ba36b5f9238e570ea872df977ed50651174c22510dcdc699d`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:8fb1ccf561c68fe89d8bcbae5ff084cf0abd84fd2363b4ec1789794b2dbc7a31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219629876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5d606a69ac811e24028853731ce3876c2081c9926124809b5369c40d3e38d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 17:21:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 17:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Jul 2021 17:22:32 GMT
ENV LANG=C.UTF-8
# Sat, 10 Jul 2021 17:45:35 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Jul 2021 17:45:38 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 10 Jul 2021 17:45:45 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 10 Jul 2021 17:57:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Jul 2021 17:57:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Jul 2021 17:57:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Jul 2021 17:57:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Jul 2021 17:57:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Jul 2021 17:57:59 GMT
CMD ["irb"]
# Sun, 11 Jul 2021 07:19:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Jul 2021 07:27:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 07:27:27 GMT
ENV RAILS_ENV=production
# Sun, 11 Jul 2021 07:27:31 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Jul 2021 07:27:38 GMT
ENV HOME=/home/redmine
# Sun, 11 Jul 2021 07:27:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Jul 2021 07:27:56 GMT
ENV REDMINE_VERSION=4.2.1
# Sun, 11 Jul 2021 07:27:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Sun, 11 Jul 2021 07:28:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Jul 2021 07:35:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Jul 2021 07:35:26 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Jul 2021 07:35:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Jul 2021 07:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Jul 2021 07:35:45 GMT
EXPOSE 3000
# Sun, 11 Jul 2021 07:35:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba063dbcdd8aa55ec2183194edae6ea424d440c8c3c4ab57e29bdc8d30739f`  
		Last Modified: Sat, 10 Jul 2021 18:24:25 GMT  
		Size: 12.7 MB (12704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302bed40ec71d6898df63835eb0d9463b4672fcb74c6d77594621b1a9d96089b`  
		Last Modified: Sat, 10 Jul 2021 18:24:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d142b79f0a553ffa66e8c2525798e544895249d98562aa21710905ebcdc6ed`  
		Last Modified: Sat, 10 Jul 2021 18:25:40 GMT  
		Size: 15.0 MB (14997790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3641aa4022fa299e9c8ba11982ead0ef3ba6b4e176be30a9d1f232615c99c`  
		Last Modified: Sat, 10 Jul 2021 18:25:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4804b39acc72bb6d81a7bfc7c05f56e803d5b3e9d2ed1c298bbd2eb44c7e5356`  
		Last Modified: Sun, 11 Jul 2021 08:15:25 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9073dd583be35eadb9e9e25a07f78b0a111fca6d47e69f14431eeb4b81f0682a`  
		Last Modified: Sun, 11 Jul 2021 08:15:45 GMT  
		Size: 101.3 MB (101327909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae14e6cdfd8bc5a68ed3c6f67843101b5677d40266ab29f2da8d3c24724ad20`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346cf33cfa1c3ae728b01723b2eacfc89d22db906bbb468ad356ffe6f80188b8`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4551ad703a6bab86fb1132fc6ecfd00620f4079d4d10d5c9d3f6b78a66d698a0`  
		Last Modified: Sun, 11 Jul 2021 08:15:22 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f790f7d0d86286c2d1129fa246d6eb23d09db45923ec78d8d0e2402cfd8660`  
		Last Modified: Sun, 11 Jul 2021 08:15:30 GMT  
		Size: 57.0 MB (56983237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dff610884a2816b07cde2af44a25989e11404807fe565fed2cee5ba172a03bc`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; s390x

```console
$ docker pull redmine@sha256:73d6f4443ca8fb63dbad4f2d16c45bd208f75b21472cd8dd96cc1307bd1e2773
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202549125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f90d1267f56ffe9dd1410a3837ccbf93c9da343fe9ff0a822248352eaeb441`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:56:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:56:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 09 Jul 2021 03:56:46 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jul 2021 04:10:42 GMT
ENV RUBY_MAJOR=2.7
# Fri, 09 Jul 2021 04:10:43 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 09 Jul 2021 04:10:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 09 Jul 2021 04:13:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 09 Jul 2021 04:13:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 09 Jul 2021 04:13:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 09 Jul 2021 04:13:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Jul 2021 04:13:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 09 Jul 2021 04:13:29 GMT
CMD ["irb"]
# Sat, 10 Jul 2021 03:58:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Jul 2021 03:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 03:59:51 GMT
ENV RAILS_ENV=production
# Sat, 10 Jul 2021 03:59:51 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Jul 2021 03:59:52 GMT
ENV HOME=/home/redmine
# Sat, 10 Jul 2021 03:59:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Jul 2021 03:59:54 GMT
ENV REDMINE_VERSION=4.2.1
# Sat, 10 Jul 2021 03:59:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Sat, 10 Jul 2021 04:00:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Jul 2021 04:03:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Jul 2021 04:03:24 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Jul 2021 04:03:25 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Jul 2021 04:03:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Jul 2021 04:03:26 GMT
EXPOSE 3000
# Sat, 10 Jul 2021 04:03:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb0861b7843d74cdcb468db372740a5fbb65d1a7a489cd207e57603e23b308`  
		Last Modified: Fri, 09 Jul 2021 04:33:35 GMT  
		Size: 10.8 MB (10814494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b9cde22299f5aa53f8d9540f770e1b6ab0e6223d1d106df86a5a071f8f3ec`  
		Last Modified: Fri, 09 Jul 2021 04:33:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf70f667dcd7c81ea6676bf03ad1d287575af1b2eceb425583be290e010897d`  
		Last Modified: Fri, 09 Jul 2021 04:34:14 GMT  
		Size: 14.7 MB (14697234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db437741211099211d57153dd52a63267f0affc47f39380dcd6da3552b8d5d5`  
		Last Modified: Fri, 09 Jul 2021 04:34:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a890c47c8baf9911890e19680c177f40232d060ba3cb040b2769a783f1ef98`  
		Last Modified: Sat, 10 Jul 2021 04:14:43 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95693198ef1207b35d9efaf8262d24914419aa240f3df8e04fc6369e5dcb55d8`  
		Last Modified: Sat, 10 Jul 2021 04:14:57 GMT  
		Size: 91.8 MB (91789992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5150ba28aa600261d40392db78998b0639dce33fa135a4749a3e03046b57ab38`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6faf8f4361902faa3aab0a419eeb7f8819ad29e5e3daf830099ed96210ec9fe`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472586cc07848d25dd2f1f9438ec666dc78b643ede7d89344b5da229b412a5c3`  
		Last Modified: Sat, 10 Jul 2021 04:14:42 GMT  
		Size: 3.1 MB (3058671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384911646e488885a18a1fc8217f5f547cde94a5281986d7b69f117e363381ea`  
		Last Modified: Sat, 10 Jul 2021 04:14:46 GMT  
		Size: 56.4 MB (56423763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051ac5465ae61ddb401a283b21e69175949f1424f30cea6aa203408b2ea9c214`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.1-alpine`

```console
$ docker pull redmine@sha256:7de4015773da4d105b5f43705556003eb3071d781612fa6e7f6010981e4e56e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.2.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:7fb14bb9edbf56cf78406c149b3015cfd560d8ab4b036edebde5aa5e4b83f5af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150068908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74c717ce35a7872383b67fe6276f951c39395fcba0eda36625d7e2eaa9a32932`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 08 Jul 2021 21:57:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 08 Jul 2021 21:57:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 08 Jul 2021 21:57:30 GMT
ENV LANG=C.UTF-8
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_MAJOR=2.7
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:18:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:18:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:18:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:18:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:18:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:18:51 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:22:24 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jul 2021 20:22:32 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 14 Jul 2021 20:22:33 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:22:33 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:22:33 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:22:34 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:22:35 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:22:35 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:22:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:22:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jul 2021 20:24:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jul 2021 20:24:42 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:24:42 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 14 Jul 2021 20:24:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:24:42 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:24:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b0ea69e9ed42c49b5af449b703a12a4d2f2e28d87905af6fcd903fdae5689`  
		Last Modified: Thu, 08 Jul 2021 22:38:46 GMT  
		Size: 3.6 MB (3581658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad656ed833315b61ea674706f32c2d18d7412c7120926442af57b9131ee72ee`  
		Last Modified: Thu, 08 Jul 2021 22:38:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626f6830afc6fb7a05a8f18f2b98e4ea4db3d2dd50803e5cd2c627fe25150dc8`  
		Last Modified: Thu, 08 Jul 2021 22:40:13 GMT  
		Size: 14.4 MB (14373123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5375389679c9573d241b22905aee17b20981e2628989561698087f107fcfed4a`  
		Last Modified: Thu, 08 Jul 2021 22:40:11 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76a82132aeb154f32b80803eecedc3e27e062a35ae1e05284dc2d7e6c7f4f59`  
		Last Modified: Wed, 14 Jul 2021 20:35:42 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb4af997128346f54fa569d3a04180c718e02a90e90eff7161241d54deef92`  
		Last Modified: Wed, 14 Jul 2021 20:35:52 GMT  
		Size: 69.5 MB (69526214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14da2816c58ef08b826f823d7b6a4126bb63594ed1109880b795c28cc4d3f032`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f34be07349b94807cc58a0e31cecec279d0591b9a6f1f65f1dbe94a4713462`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b05ead31106734fcef5216d256a8536461fa7935f729e67262c90f55e683b`  
		Last Modified: Wed, 14 Jul 2021 20:35:40 GMT  
		Size: 3.1 MB (3060004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c586852175065725ae48c5682f1ecea003599fbc0028c3387f5de00cc28f34`  
		Last Modified: Wed, 14 Jul 2021 20:36:03 GMT  
		Size: 56.7 MB (56712212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d1559a239e3bf1260f693961d40d28b32673907100b077a797e55d543f072c`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.1-passenger`

```console
$ docker pull redmine@sha256:9b780f98151823e0e84e1e41974c548143cae7090cd367eb711d44d3bc8a966b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.2.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:a320947c8461cd8bafad0bcfda90b4f5ac840389345003324df81de7b46ad296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3049f679e04c98a7643e800733c59f85c960a686a186192d9b12a222bed1592`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:22:01 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:22:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:22:20 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:22:20 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:22:20 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41f4f9e9b7629be3e6e9666279b940b489648484da4e41725e7b22c1c94b1b`  
		Last Modified: Wed, 14 Jul 2021 20:35:22 GMT  
		Size: 21.1 MB (21131700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436698f0e4aec6d6e7c991fd623ae0d4eab48e62193c564b2fa25de8f4a52e`  
		Last Modified: Wed, 14 Jul 2021 20:35:20 GMT  
		Size: 4.9 MB (4919284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:alpine`

```console
$ docker pull redmine@sha256:7de4015773da4d105b5f43705556003eb3071d781612fa6e7f6010981e4e56e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:7fb14bb9edbf56cf78406c149b3015cfd560d8ab4b036edebde5aa5e4b83f5af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150068908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74c717ce35a7872383b67fe6276f951c39395fcba0eda36625d7e2eaa9a32932`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Thu, 08 Jul 2021 21:57:27 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Thu, 08 Jul 2021 21:57:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 08 Jul 2021 21:57:30 GMT
ENV LANG=C.UTF-8
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_MAJOR=2.7
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 08 Jul 2021 22:15:57 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:18:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:18:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:18:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:18:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:18:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:18:51 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:22:24 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 14 Jul 2021 20:22:32 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 14 Jul 2021 20:22:33 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:22:33 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:22:33 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:22:34 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:22:35 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:22:35 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:22:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:22:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 14 Jul 2021 20:24:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 14 Jul 2021 20:24:42 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:24:42 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 14 Jul 2021 20:24:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:24:42 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:24:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5b0ea69e9ed42c49b5af449b703a12a4d2f2e28d87905af6fcd903fdae5689`  
		Last Modified: Thu, 08 Jul 2021 22:38:46 GMT  
		Size: 3.6 MB (3581658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad656ed833315b61ea674706f32c2d18d7412c7120926442af57b9131ee72ee`  
		Last Modified: Thu, 08 Jul 2021 22:38:45 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:626f6830afc6fb7a05a8f18f2b98e4ea4db3d2dd50803e5cd2c627fe25150dc8`  
		Last Modified: Thu, 08 Jul 2021 22:40:13 GMT  
		Size: 14.4 MB (14373123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5375389679c9573d241b22905aee17b20981e2628989561698087f107fcfed4a`  
		Last Modified: Thu, 08 Jul 2021 22:40:11 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76a82132aeb154f32b80803eecedc3e27e062a35ae1e05284dc2d7e6c7f4f59`  
		Last Modified: Wed, 14 Jul 2021 20:35:42 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cb4af997128346f54fa569d3a04180c718e02a90e90eff7161241d54deef92`  
		Last Modified: Wed, 14 Jul 2021 20:35:52 GMT  
		Size: 69.5 MB (69526214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14da2816c58ef08b826f823d7b6a4126bb63594ed1109880b795c28cc4d3f032`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f34be07349b94807cc58a0e31cecec279d0591b9a6f1f65f1dbe94a4713462`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98b05ead31106734fcef5216d256a8536461fa7935f729e67262c90f55e683b`  
		Last Modified: Wed, 14 Jul 2021 20:35:40 GMT  
		Size: 3.1 MB (3060004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c586852175065725ae48c5682f1ecea003599fbc0028c3387f5de00cc28f34`  
		Last Modified: Wed, 14 Jul 2021 20:36:03 GMT  
		Size: 56.7 MB (56712212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d1559a239e3bf1260f693961d40d28b32673907100b077a797e55d543f072c`  
		Last Modified: Wed, 14 Jul 2021 20:35:39 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:latest`

```console
$ docker pull redmine@sha256:cae6a4d4227606764c6a75b180a5b675e4d7415888b5a1261069761a7cd84eac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:latest` - linux; amd64

```console
$ docker pull redmine@sha256:c303bc0f5596613dabea4516d47172296178fa21f6db17497624805f778cb357
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195475758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:338c47d4bca896733efe021ec38c0d595cf043de470eba5e45d6e3dde1a485c3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:504785f157b11fc0cf462141bdae1564241f3417ea1c8371d3c2e4c7dd41c552
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196972163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:217c8956d29925ec9e63ffbf48e3d04a71ec25911566cd968e65a03abbcef198`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:50:09 GMT
ADD file:78d4ced31112d85490c684f350aceeebfc72a804262c7ad3e033257e3894f5c4 in / 
# Tue, 22 Jun 2021 23:50:11 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:06:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:06:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:06:50 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:17:20 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:05:54 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:05:55 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:19:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:19:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:20:00 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:20:00 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:20:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:20:03 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:32:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:33:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:33:44 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:33:45 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:33:45 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:33:47 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:33:48 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 22:33:48 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 22:33:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:39:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:39:30 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:39:30 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:39:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:39:32 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:39:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:532d6df30af5174ac6e1b379c32b8f464d44651ac060376a560c4a76a87704a7`  
		Last Modified: Wed, 23 Jun 2021 00:01:46 GMT  
		Size: 24.9 MB (24878945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8b3ba0f03212caacd2191837bdac2f1a9abf399938b4020b315e4c6ea7ba0c7`  
		Last Modified: Wed, 23 Jun 2021 14:05:28 GMT  
		Size: 10.3 MB (10345811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cfab7796870f80c9db896239384ac194808f4ce5fab9f16ba155559772cc1e`  
		Last Modified: Wed, 23 Jun 2021 14:05:23 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4340642939f48d099081c75a2712db898b9985ae54a619b2452aac1d6d5811`  
		Last Modified: Thu, 08 Jul 2021 20:43:39 GMT  
		Size: 13.9 MB (13871335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:695fcd3bc334ffbc54deec488d9db9eda8fec160e0a45fb2eaf1cb3c40fe5d17`  
		Last Modified: Thu, 08 Jul 2021 20:43:31 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e84c1768026dd91ab7c8b588e6bca6eb786ae29dbdbcb5cfe9942272bcfc56b`  
		Last Modified: Thu, 08 Jul 2021 22:55:15 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7075123429263b675529579bcba18589d90fc77e59eb5919484dedb6d1c64c1f`  
		Last Modified: Thu, 08 Jul 2021 22:56:17 GMT  
		Size: 89.6 MB (89576320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e64c6c915303586fcbdb5e1921c304efd17cae07d4aabc1d6ebae70a889fd8`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b203953be51a5b5e20215561ddbcf8db375b9ca69dd0f7ba4d114fa962f6d7d`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4ac40a10c440649c65c501f24a90d153143ce98bcf9b9bf731f6e22a347570`  
		Last Modified: Thu, 08 Jul 2021 22:55:17 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14230d92bd82d511c4f7398fd0d256fb2c88bc9039691884c1a0a90a6b9b7d56`  
		Last Modified: Thu, 08 Jul 2021 22:55:35 GMT  
		Size: 55.2 MB (55236836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eea4df7ac799e61a3b26a4195f6641617e2e656b4b38cd6c47240821584be3`  
		Last Modified: Thu, 08 Jul 2021 22:55:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:918c928c44808884e8f314ba4798c35f6c33f66f3af9808185b7cb6632829c4f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4523ba6f474f4b705844d9e15d89345a8277bfdbf939337c277171f2733bc896`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:31 GMT
ADD file:8d200a3bbe985ff355343675c5555852f27550a9e367969df6bc98034efb8fd4 in / 
# Wed, 23 Jun 2021 00:20:31 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 23:18:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 23:18:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 23:18:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 23:36:25 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 23:43:24 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 23:43:24 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:35:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:35:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:35:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:35:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:35:12 GMT
CMD ["irb"]
# Fri, 09 Jul 2021 04:06:25 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 09 Jul 2021 04:07:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 04:07:27 GMT
ENV RAILS_ENV=production
# Fri, 09 Jul 2021 04:07:27 GMT
WORKDIR /usr/src/redmine
# Fri, 09 Jul 2021 04:07:28 GMT
ENV HOME=/home/redmine
# Fri, 09 Jul 2021 04:07:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 09 Jul 2021 04:07:30 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 09 Jul 2021 04:07:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 09 Jul 2021 04:07:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 09 Jul 2021 04:12:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 09 Jul 2021 04:12:52 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 09 Jul 2021 04:12:53 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 09 Jul 2021 04:12:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 09 Jul 2021 04:12:54 GMT
EXPOSE 3000
# Fri, 09 Jul 2021 04:12:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8452be1adf00f91570fe21a8e61aaf4c12e014daf67d7de65d984f4e8ecca2f1`  
		Last Modified: Wed, 23 Jun 2021 00:31:49 GMT  
		Size: 22.7 MB (22746055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08b763290fb30bc16e505b4aa06ba1c3041182ac9bd8be48df5e94cbbe8545d`  
		Last Modified: Thu, 24 Jun 2021 00:49:52 GMT  
		Size: 9.9 MB (9872206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f611d0cebec7d01271526d00ff39f508174641d4e952ac4954fb89f368bf331`  
		Last Modified: Thu, 24 Jun 2021 00:49:44 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c081e6813d08a36724de201912dcf2049b4b63e901379b09265fff1f204332`  
		Last Modified: Thu, 08 Jul 2021 23:20:14 GMT  
		Size: 13.8 MB (13766804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47e03b2ecd26a74249ee57a56b50a959f58fbcaca622b530a671eca71a7384d`  
		Last Modified: Thu, 08 Jul 2021 23:20:07 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5ad0520989f495616ff11a4e507a10e68c9135a8387cf52dfca8fefd1fa348`  
		Last Modified: Fri, 09 Jul 2021 04:27:36 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a23a4b1761119307dc0dd899befff1a28684d45a780a3b964aef62e5ea8c5147`  
		Last Modified: Fri, 09 Jul 2021 04:28:33 GMT  
		Size: 85.6 MB (85590504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:089aa8086891a0e5b87d68a89f8621e084085b5786ee8e0c05539a337161a184`  
		Last Modified: Fri, 09 Jul 2021 04:27:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57d7596e26caaeafa01d35cfbd470f7a013b174e7c5c25852729c10b10448c`  
		Last Modified: Fri, 09 Jul 2021 04:27:33 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e2efb117cd99001cc83a98b5a1277459f26c1b985c59ae03866ca74c7d1380`  
		Last Modified: Fri, 09 Jul 2021 04:27:38 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ab3b3250933a12c6c93d662c3198824bef82b64f0d7f119675b68e1cec76a6`  
		Last Modified: Fri, 09 Jul 2021 04:27:59 GMT  
		Size: 55.1 MB (55076972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3916fdc65621036c0f5ddd98394f1e47796b2f19531e4ab24c86648449214c16`  
		Last Modified: Fri, 09 Jul 2021 04:27:33 GMT  
		Size: 1.8 KB (1793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:0741f6999c4d2a4e13afe1af9a34785c48f61a2feb89930198909593b569e246
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203231922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3d2c5023b434e055c0449d22553bc2ecc42a9e53a462c79fada428177c6180`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:40 GMT
ADD file:beee00b59da720f68e12e2ba2a8134207c80c777ddb4ceb03c71e3e4c3f51c93 in / 
# Tue, 22 Jun 2021 23:49:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 03:53:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 03:53:54 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 03:53:54 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 03:58:54 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 23:45:12 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 23:45:13 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:45:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:45:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:45:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:45:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:45:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:45:29 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 23:21:02 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 23:21:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 23:21:24 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 23:21:25 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 23:21:25 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 23:21:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 23:21:26 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 23:21:26 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 23:21:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 23:23:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 23:23:52 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 23:23:53 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 23:23:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 23:23:53 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 23:23:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:448f6bf000e31217a7c202c659b03b7f8ac8d3ae6b03ef7a2f8339be2f00ff4a`  
		Last Modified: Tue, 22 Jun 2021 23:55:25 GMT  
		Size: 25.9 MB (25914993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f276f053f0cad4dbf0c339099f5dd135531eb3ffb0bccc09369e7b7391b18d72`  
		Last Modified: Wed, 23 Jun 2021 04:22:18 GMT  
		Size: 11.3 MB (11263062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863be1d4664c690cf3e71cf9494c9b590ce4781e8008aef05d7cf572b8feddcc`  
		Last Modified: Wed, 23 Jun 2021 04:22:16 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038f5d2c58688ac84743d00ab7bbdc6b4093e20d9a833d6af3496cc62e935a25`  
		Last Modified: Thu, 08 Jul 2021 21:09:46 GMT  
		Size: 14.4 MB (14356604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e4dfdc14b449c213e94db8cd01bdfa232be4fa72040ffeebb4ea881ffa8634`  
		Last Modified: Thu, 08 Jul 2021 21:09:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04df641efdceaa2aee736b0b2ed3580d9cc12941e9d5b47754238e2832b4290d`  
		Last Modified: Thu, 08 Jul 2021 23:29:47 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e08f5ce73ad17307002bfba119f4a63a0edae9959555829f15c37ec8f76c2`  
		Last Modified: Thu, 08 Jul 2021 23:30:04 GMT  
		Size: 92.6 MB (92610656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4765b269f180b2c2704772dd7d776ea01a9075ed5d1d8cd8f0882ca083129c2c`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6329e48a16d3a91d290cfbae3c0a552cfe96c6b792fcb231df35ff3c039a1`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6feadd8be638a909710f31206aa67f01ca6d2a8ebec560b39b0dc3523c0211f6`  
		Last Modified: Thu, 08 Jul 2021 23:29:46 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5a01cee6465420071dfb449649aebee78fb947eecd0b3b279df2405c1c4d9d`  
		Last Modified: Thu, 08 Jul 2021 23:29:51 GMT  
		Size: 56.0 MB (56023674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbbcb4d6ad95bc21ed907d86fa7e683a21628ed441ad64f891f7322fc156b12`  
		Last Modified: Thu, 08 Jul 2021 23:29:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:38c75a4b236bb825b9ee8fa35034d33dab94661ce6f8ce26c59869e809aa60ab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202116586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cab517b8b53a6715a276de085b7d54ac6b3054ed3ee985c2ec4022d275a36e6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:35 GMT
ADD file:48f656ac6733911048b3de850490438d0233b3badc11861fca62062d4edfaf40 in / 
# Tue, 22 Jun 2021 23:39:35 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 13:33:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 13:33:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 13:33:25 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 13:42:41 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:08:54 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:08:54 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 20:01:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 20:01:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 20:01:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 20:01:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 20:01:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 20:01:08 GMT
CMD ["irb"]
# Thu, 08 Jul 2021 22:46:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 08 Jul 2021 22:47:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 08 Jul 2021 22:47:20 GMT
ENV RAILS_ENV=production
# Thu, 08 Jul 2021 22:47:20 GMT
WORKDIR /usr/src/redmine
# Thu, 08 Jul 2021 22:47:20 GMT
ENV HOME=/home/redmine
# Thu, 08 Jul 2021 22:47:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 08 Jul 2021 22:47:21 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 08 Jul 2021 22:47:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 08 Jul 2021 22:47:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 08 Jul 2021 22:48:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 08 Jul 2021 22:48:13 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 08 Jul 2021 22:48:14 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 08 Jul 2021 22:48:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 08 Jul 2021 22:48:14 GMT
EXPOSE 3000
# Thu, 08 Jul 2021 22:48:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33af2dcb865e65d53cdeb843b67a0ef62151fa32df292293e7c6b0eb728ac5ac`  
		Last Modified: Tue, 22 Jun 2021 23:46:23 GMT  
		Size: 27.8 MB (27797411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb2041b26a9335dbdc8e6cc9bd945661b43317eb0de6d4e1e8ce82275cbea6`  
		Last Modified: Wed, 23 Jun 2021 14:14:04 GMT  
		Size: 17.2 MB (17227420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c89206098d37979fca1f31ba315796953128b80660adc5194c5541f0ac3f34`  
		Last Modified: Wed, 23 Jun 2021 14:13:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce027bc021a8f988e98283d7e7edb0812da70bec1469306b760a90237fb460ac`  
		Last Modified: Thu, 08 Jul 2021 20:34:09 GMT  
		Size: 14.0 MB (13991996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f914d412069980e7e91c9e3b27cd62e1d17cffdd9dd8b8d86e009a47a54d257`  
		Last Modified: Thu, 08 Jul 2021 20:34:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96ddcca7d90497767f04b499a232298ba4b6b367a55fc644281d45884b4904c4`  
		Last Modified: Thu, 08 Jul 2021 22:53:29 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512a07456067d7c014c80d85bba6d608010bf9baaa1cbf62bfefc070f9e197d5`  
		Last Modified: Thu, 08 Jul 2021 22:53:53 GMT  
		Size: 95.7 MB (95703052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b637a32b9c8c0c921586600afc7d5867c46a31465bbb953d9f07412725c8f280`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe31a7355aa80ea3975b5e2ea081a34279b494c8636489851f5bb2adabbb9ba9`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc4f8125c232b162083e88887968149ff3e94b419b661c0c98ab1c249ae8e82`  
		Last Modified: Thu, 08 Jul 2021 22:53:28 GMT  
		Size: 3.1 MB (3058670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c938aebe09af0b44a41d919513d737720f30afcb71bcdfe7ff6ed289be406cdb`  
		Last Modified: Thu, 08 Jul 2021 22:53:34 GMT  
		Size: 44.3 MB (44333801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a2250ccc831a8ba36b5f9238e570ea872df977ed50651174c22510dcdc699d`  
		Last Modified: Thu, 08 Jul 2021 22:53:26 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:8fb1ccf561c68fe89d8bcbae5ff084cf0abd84fd2363b4ec1789794b2dbc7a31
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.6 MB (219629876 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa5d606a69ac811e24028853731ce3876c2081c9926124809b5369c40d3e38d4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 15:58:12 GMT
ADD file:e599654230c9fe95fe2c591dbe60e8a0a886cd053b6117230fbae47561145731 in / 
# Fri, 09 Jul 2021 15:58:14 GMT
CMD ["bash"]
# Sat, 10 Jul 2021 17:21:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 17:22:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Jul 2021 17:22:32 GMT
ENV LANG=C.UTF-8
# Sat, 10 Jul 2021 17:45:35 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Jul 2021 17:45:38 GMT
ENV RUBY_VERSION=2.7.4
# Sat, 10 Jul 2021 17:45:45 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Sat, 10 Jul 2021 17:57:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Jul 2021 17:57:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Jul 2021 17:57:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Jul 2021 17:57:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Jul 2021 17:57:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Jul 2021 17:57:59 GMT
CMD ["irb"]
# Sun, 11 Jul 2021 07:19:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Jul 2021 07:27:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Jul 2021 07:27:27 GMT
ENV RAILS_ENV=production
# Sun, 11 Jul 2021 07:27:31 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Jul 2021 07:27:38 GMT
ENV HOME=/home/redmine
# Sun, 11 Jul 2021 07:27:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Jul 2021 07:27:56 GMT
ENV REDMINE_VERSION=4.2.1
# Sun, 11 Jul 2021 07:27:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Sun, 11 Jul 2021 07:28:13 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Jul 2021 07:35:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Jul 2021 07:35:26 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Jul 2021 07:35:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Jul 2021 07:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Jul 2021 07:35:45 GMT
EXPOSE 3000
# Sun, 11 Jul 2021 07:35:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f9cb1946299ce1824ee44809cd0c8b419528fee2f0f89e86400787a14b666f59`  
		Last Modified: Wed, 23 Jun 2021 00:37:07 GMT  
		Size: 30.6 MB (30553627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceba063dbcdd8aa55ec2183194edae6ea424d440c8c3c4ab57e29bdc8d30739f`  
		Last Modified: Sat, 10 Jul 2021 18:24:25 GMT  
		Size: 12.7 MB (12704380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302bed40ec71d6898df63835eb0d9463b4672fcb74c6d77594621b1a9d96089b`  
		Last Modified: Sat, 10 Jul 2021 18:24:22 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d142b79f0a553ffa66e8c2525798e544895249d98562aa21710905ebcdc6ed`  
		Last Modified: Sat, 10 Jul 2021 18:25:40 GMT  
		Size: 15.0 MB (14997790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb3641aa4022fa299e9c8ba11982ead0ef3ba6b4e176be30a9d1f232615c99c`  
		Last Modified: Sat, 10 Jul 2021 18:25:37 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4804b39acc72bb6d81a7bfc7c05f56e803d5b3e9d2ed1c298bbd2eb44c7e5356`  
		Last Modified: Sun, 11 Jul 2021 08:15:25 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9073dd583be35eadb9e9e25a07f78b0a111fca6d47e69f14431eeb4b81f0682a`  
		Last Modified: Sun, 11 Jul 2021 08:15:45 GMT  
		Size: 101.3 MB (101327909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae14e6cdfd8bc5a68ed3c6f67843101b5677d40266ab29f2da8d3c24724ad20`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346cf33cfa1c3ae728b01723b2eacfc89d22db906bbb468ad356ffe6f80188b8`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4551ad703a6bab86fb1132fc6ecfd00620f4079d4d10d5c9d3f6b78a66d698a0`  
		Last Modified: Sun, 11 Jul 2021 08:15:22 GMT  
		Size: 3.1 MB (3058680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f790f7d0d86286c2d1129fa246d6eb23d09db45923ec78d8d0e2402cfd8660`  
		Last Modified: Sun, 11 Jul 2021 08:15:30 GMT  
		Size: 57.0 MB (56983237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dff610884a2816b07cde2af44a25989e11404807fe565fed2cee5ba172a03bc`  
		Last Modified: Sun, 11 Jul 2021 08:15:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:73d6f4443ca8fb63dbad4f2d16c45bd208f75b21472cd8dd96cc1307bd1e2773
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202549125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32f90d1267f56ffe9dd1410a3837ccbf93c9da343fe9ff0a822248352eaeb441`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 09 Jul 2021 02:50:32 GMT
ADD file:a53e5772eefa4592eeff989f279dcc870986db7207b419dc3ae61cae85fce41f in / 
# Fri, 09 Jul 2021 02:50:33 GMT
CMD ["bash"]
# Fri, 09 Jul 2021 03:56:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 09 Jul 2021 03:56:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 09 Jul 2021 03:56:46 GMT
ENV LANG=C.UTF-8
# Fri, 09 Jul 2021 04:10:42 GMT
ENV RUBY_MAJOR=2.7
# Fri, 09 Jul 2021 04:10:43 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 09 Jul 2021 04:10:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 09 Jul 2021 04:13:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 09 Jul 2021 04:13:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 09 Jul 2021 04:13:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 09 Jul 2021 04:13:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 09 Jul 2021 04:13:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 09 Jul 2021 04:13:29 GMT
CMD ["irb"]
# Sat, 10 Jul 2021 03:58:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Jul 2021 03:59:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Jul 2021 03:59:51 GMT
ENV RAILS_ENV=production
# Sat, 10 Jul 2021 03:59:51 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Jul 2021 03:59:52 GMT
ENV HOME=/home/redmine
# Sat, 10 Jul 2021 03:59:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Jul 2021 03:59:54 GMT
ENV REDMINE_VERSION=4.2.1
# Sat, 10 Jul 2021 03:59:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Sat, 10 Jul 2021 04:00:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Jul 2021 04:03:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Jul 2021 04:03:24 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Jul 2021 04:03:25 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Jul 2021 04:03:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Jul 2021 04:03:26 GMT
EXPOSE 3000
# Sat, 10 Jul 2021 04:03:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d08eb187b3111e87e1b138f7b93df64c5470da613a64d0adc804e17e12aed4dc`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 25.8 MB (25760716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2fb0861b7843d74cdcb468db372740a5fbb65d1a7a489cd207e57603e23b308`  
		Last Modified: Fri, 09 Jul 2021 04:33:35 GMT  
		Size: 10.8 MB (10814494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5b9cde22299f5aa53f8d9540f770e1b6ab0e6223d1d106df86a5a071f8f3ec`  
		Last Modified: Fri, 09 Jul 2021 04:33:33 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bf70f667dcd7c81ea6676bf03ad1d287575af1b2eceb425583be290e010897d`  
		Last Modified: Fri, 09 Jul 2021 04:34:14 GMT  
		Size: 14.7 MB (14697234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db437741211099211d57153dd52a63267f0affc47f39380dcd6da3552b8d5d5`  
		Last Modified: Fri, 09 Jul 2021 04:34:12 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a890c47c8baf9911890e19680c177f40232d060ba3cb040b2769a783f1ef98`  
		Last Modified: Sat, 10 Jul 2021 04:14:43 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95693198ef1207b35d9efaf8262d24914419aa240f3df8e04fc6369e5dcb55d8`  
		Last Modified: Sat, 10 Jul 2021 04:14:57 GMT  
		Size: 91.8 MB (91789992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5150ba28aa600261d40392db78998b0639dce33fa135a4749a3e03046b57ab38`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6faf8f4361902faa3aab0a419eeb7f8819ad29e5e3daf830099ed96210ec9fe`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472586cc07848d25dd2f1f9438ec666dc78b643ede7d89344b5da229b412a5c3`  
		Last Modified: Sat, 10 Jul 2021 04:14:42 GMT  
		Size: 3.1 MB (3058671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:384911646e488885a18a1fc8217f5f547cde94a5281986d7b69f117e363381ea`  
		Last Modified: Sat, 10 Jul 2021 04:14:46 GMT  
		Size: 56.4 MB (56423763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:051ac5465ae61ddb401a283b21e69175949f1424f30cea6aa203408b2ea9c214`  
		Last Modified: Sat, 10 Jul 2021 04:14:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:passenger`

```console
$ docker pull redmine@sha256:9b780f98151823e0e84e1e41974c548143cae7090cd367eb711d44d3bc8a966b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:a320947c8461cd8bafad0bcfda90b4f5ac840389345003324df81de7b46ad296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3049f679e04c98a7643e800733c59f85c960a686a186192d9b12a222bed1592`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:22:01 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:22:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:22:20 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:22:20 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:22:20 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41f4f9e9b7629be3e6e9666279b940b489648484da4e41725e7b22c1c94b1b`  
		Last Modified: Wed, 14 Jul 2021 20:35:22 GMT  
		Size: 21.1 MB (21131700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436698f0e4aec6d6e7c991fd623ae0d4eab48e62193c564b2fa25de8f4a52e`  
		Last Modified: Wed, 14 Jul 2021 20:35:20 GMT  
		Size: 4.9 MB (4919284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
