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
$ docker pull redmine@sha256:95435c3e6e2d0815459d7c44520b2743dbb8806cba32184ba0bfdf143d5af0b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4` - linux; amd64

```console
$ docker pull redmine@sha256:e28ea2b1f675569c4763cf0cd04ff101d384a263d952858b8e7533b7f335f34a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195475927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be97e87738155b1d102c2b0b7286bd39b06e62a5a8184e8fb0e21b7a2e819743`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 17:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:28:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:28:25 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:03:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:04:03 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:04:03 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:04:03 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:04:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 11:04:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:04:49 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:04:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:49 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:04:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e582c090726ff249b7e30253c7f0c11aa2cd14282a8b6cd0e8055c8615e5586`  
		Last Modified: Thu, 22 Jul 2021 17:42:40 GMT  
		Size: 14.5 MB (14509812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f96a83aedee46aef2be1d4f73cc6990dc7e756981b022462100ac16fad345`  
		Last Modified: Thu, 22 Jul 2021 17:42:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9466f2ac94d013cc74523ee4ad44d9720c72baa51d8aecc2afcba41c3754be44`  
		Last Modified: Fri, 23 Jul 2021 11:10:32 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbad6372ccefa1ce14b5eefe2fe718c0cd234b40bf9a70e3d02e131a9dd65d26`  
		Last Modified: Fri, 23 Jul 2021 11:10:45 GMT  
		Size: 94.1 MB (94087869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93724991108aa18238773a3122f3fcd80f69331610c0a7f00656f690ac7692`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19466676666dc7f1a145b5b2534855e6f32c152cd3da118bc5536badc24da33d`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc48a22ec231d5048d556cd637291655083a29acb695b0073039d36315929da`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 3.1 MB (3058677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00b1336ee6986b3f2923502d082ce45ebccea58e21f85ddd12812be6796e1f`  
		Last Modified: Fri, 23 Jul 2021 11:10:33 GMT  
		Size: 44.1 MB (44106755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fe342d55cb9155ec0d7a14a371258946d43b0b4e3df44e3f1bbe9b166a5ef`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:9ef48dcd233199a54171d5bf678c6fc5245453cdd9827c68ce9b91796501de9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196974351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25105893bd633c389af7ab7f4e947fa0ff2172ac3cd182d70b9bc2d2a45607e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:39:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:48:33 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 14:48:33 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 14:48:34 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 14:52:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:52:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:52:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:52:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:52:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:52:55 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:25:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:26:16 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:26:17 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:26:17 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:26:18 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:26:19 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 01:26:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 01:26:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:32:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:32:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:32:10 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:32:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:32:11 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:32:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9237058b7c5120d5c6315b5d17a8c1d783be09a228b83772111ce9436c29d078`  
		Last Modified: Thu, 22 Jul 2021 15:15:34 GMT  
		Size: 10.3 MB (10345807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144b4344f580222d2fbc2f0d80fc139ab1a1ddb9a245b6073c41fdca9a93c23e`  
		Last Modified: Thu, 22 Jul 2021 15:15:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8ddbd20410764a5a44de2520de7417bddfcc0fdf2f4fa1b1d4e9ac785ce253`  
		Last Modified: Thu, 22 Jul 2021 15:17:00 GMT  
		Size: 13.9 MB (13871315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1fe10899466e387c0fc9cc130a0a900ffeb91af92c09301e387e444836d74f`  
		Last Modified: Thu, 22 Jul 2021 15:16:52 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b419523e1af1c8a3f9891c74f5e29e5697be8bf7bf57f23880ac551c460f07`  
		Last Modified: Fri, 23 Jul 2021 01:48:00 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d44a2001e78eed6fc3a85dbe0059a0bfae376949cda406c9304941ed617a23`  
		Last Modified: Fri, 23 Jul 2021 01:49:01 GMT  
		Size: 89.6 MB (89576912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2901c80e9a45cf66afe7fb2306719b195ec9c983783f4058ef68246bb10b95`  
		Last Modified: Fri, 23 Jul 2021 01:47:58 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0cf9a21c70c0994e217daf5f71efd9d2f8ce8f36e062be7c831492162e99a`  
		Last Modified: Fri, 23 Jul 2021 01:47:57 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5daae06ca7c40f7fa2e94d4be701850020a63374c01cb310471f056eda7498`  
		Last Modified: Fri, 23 Jul 2021 01:48:01 GMT  
		Size: 3.1 MB (3058682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d9118a275db8a49fd1b15511383b91ac8b867604e68e255d097c4a7880a8ff`  
		Last Modified: Fri, 23 Jul 2021 01:48:21 GMT  
		Size: 55.2 MB (55238308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d94f744aa1ad4af6e0d39600d4e4bf9e68e942510443afa0d8ecf37e30835`  
		Last Modified: Fri, 23 Jul 2021 01:47:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:3aca8dadb5407c0d388ac5baf1a99dbeeabc4fe3da1c506883b1c394c7fe7610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9074a5390b69761aca8dcac7078799a4f869792b8311bc2280916419daa31aca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:15:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 02:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 02:25:03 GMT
ENV RUBY_MAJOR=2.7
# Fri, 23 Jul 2021 02:25:04 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 23 Jul 2021 02:25:04 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 23 Jul 2021 02:29:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 02:29:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 02:29:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 02:29:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:29:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 02:29:10 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 21:18:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 21:19:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 21:19:37 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 21:19:37 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 21:19:38 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 21:19:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 21:19:40 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 21:19:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 21:19:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 21:25:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 21:25:05 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 21:25:06 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 21:25:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 21:25:06 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 21:25:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b8c791d70de7f22816846fbb07e0a1d7d419841c7e539a7cf57ef05fd50c5`  
		Last Modified: Fri, 23 Jul 2021 03:05:10 GMT  
		Size: 9.9 MB (9872218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12a7edb0af862efa24dc389d7901cd2a894f2e106a1cef931ba0a6d675e2c0`  
		Last Modified: Fri, 23 Jul 2021 03:05:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b75d257bf75804e51385b730af2aaba386a501ef50517b8379966d4372c8597`  
		Last Modified: Fri, 23 Jul 2021 03:06:48 GMT  
		Size: 13.8 MB (13766962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc7c7e0536ed6ba4a99c1b8960d7c1d7365c8bc52d230b8af44d07d085916f`  
		Last Modified: Fri, 23 Jul 2021 03:06:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9cbdbb67af5c0b986c2fd6f93a2bacf3c795b046bfdf19e8f483dbc780c643`  
		Last Modified: Fri, 23 Jul 2021 21:39:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823bb8e3702405c250a7cc3dadba844fef162cbd0f5b9fb70a107f618dffeddf`  
		Last Modified: Fri, 23 Jul 2021 21:40:51 GMT  
		Size: 85.6 MB (85590187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930c9cc4f262f629914e37abf7b88697bc949d34260a237f8d740ea30ddf5902`  
		Last Modified: Fri, 23 Jul 2021 21:39:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e7aa3a63516ee59c6e77fd1a74b1ce0b303c09b2a97dd0ca3b0af594021030`  
		Last Modified: Fri, 23 Jul 2021 21:39:55 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b8cbe774bbfa06d5d0e463126138a655e455605ce81a4b4799b6495959723`  
		Last Modified: Fri, 23 Jul 2021 21:39:58 GMT  
		Size: 3.1 MB (3058685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231b30773994af4c612b2b73b0a33eef728b235396a59b1c34d64b17c2289dd`  
		Last Modified: Fri, 23 Jul 2021 21:40:19 GMT  
		Size: 55.1 MB (55076883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af42513ad3b3f3a0291481c9f4b6a077a9e62fc8cd14736897d28d5f70687618`  
		Last Modified: Fri, 23 Jul 2021 21:39:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:b7a96326ffb8fc77358a78fac0448fd3c56dd2fb1feb29dd3528e6cac29cd155
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203231883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e4b31ef3849045f66d5846fad154cbaf41e73cd54c0a5afcf7bed7817d16a5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 12:36:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 12:41:08 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 12:41:08 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 12:41:09 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 12:43:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 12:43:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 12:43:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 12:43:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 12:43:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 12:43:05 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:57:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:58:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:58:04 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:58:04 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:58:04 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:58:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:58:05 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 00:58:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 00:58:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:00:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:00:36 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:00:36 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:00:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:00:36 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:00:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a77364b6ec6cfc9422903e0f9d3f5cab5ee0ac4b62cfac6fc7c3d544ad7f57`  
		Last Modified: Thu, 22 Jul 2021 12:55:11 GMT  
		Size: 11.3 MB (11263053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a68321ef048d82e4480bc2de1681a811f18b2e1d04b5aa9dec38030570eaa40`  
		Last Modified: Thu, 22 Jul 2021 12:55:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ec69cd14df7f6066799b20f9268ae3ce6e5e0564c2b560a10804765f4c7cf`  
		Last Modified: Thu, 22 Jul 2021 12:56:22 GMT  
		Size: 14.4 MB (14356675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4a2f06c1cec263f641737334f76372caff218cb8312bc8375c4e69c7289147`  
		Last Modified: Thu, 22 Jul 2021 12:56:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02fa466075ed10ab6e904b032ad10baf66dce45f41bb930b1ea5728647d32c`  
		Last Modified: Fri, 23 Jul 2021 01:06:41 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde3ab2a527d4e47aafb6f9cf0128ee08d754d6bed600addccaa4309e29f6437`  
		Last Modified: Fri, 23 Jul 2021 01:06:56 GMT  
		Size: 92.6 MB (92610625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f378e820ad759f627889603226956c607d864e95e967c969aa7965d93fb45816`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8291e2aab5ca9a9c51cc69c4cab741f3d46369744adec4f04f120329ed36f48d`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314b7425fd6ac642e912d76f7f9dafe5eda902a1abd7ab0ad23662da1bb75d73`  
		Last Modified: Fri, 23 Jul 2021 01:06:39 GMT  
		Size: 3.1 MB (3058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9b783db9ec2f80081bb3fc6226424e234ca9e33e9da8e7e6784a9e8b2a4b9f`  
		Last Modified: Fri, 23 Jul 2021 01:06:44 GMT  
		Size: 56.0 MB (56023809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f20fa5c3f8387a262408432f792b73cb61c7957e5c6ba4edd46d4da28d05a6c`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; 386

```console
$ docker pull redmine@sha256:e0c39c52abc9d57cf5bd97523c15db6fe60284390d12d89bd95e1d8ff7ea69dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202117810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6402098c31c9ce288516e50c34618b6cdce5229aaefc10ad583c89f4e4144289`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:38:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:39:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 15:39:00 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 15:49:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:49:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:49:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:49:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:49:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:49:39 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:10:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:11:45 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:11:45 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:11:46 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:11:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:11:48 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 00:11:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 00:11:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 00:13:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 00:13:26 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 00:13:26 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 00:13:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 00:13:27 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 00:13:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d04ca5200ad3b98494cfde36960022dbd29c9afc33d685ac499fae8a05d63`  
		Last Modified: Thu, 22 Jul 2021 16:06:57 GMT  
		Size: 17.2 MB (17227285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d9d06c9e919afbd9358b702cad5bc0f28b8150722ffedb25ece16dc1f19b2`  
		Last Modified: Thu, 22 Jul 2021 16:06:48 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9e06bdf88f28c2f5d5893c862c6da8a6a73eb098cb2cd8eec57656d9a79b69`  
		Last Modified: Thu, 22 Jul 2021 16:08:14 GMT  
		Size: 14.0 MB (13992268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4f84633b2fe0d1dff5a1fd6ab3a5506af8978d94ded4f5a0f2727ce06805d4`  
		Last Modified: Thu, 22 Jul 2021 16:08:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57ef59b51318d382563cb5fdab4577df04d06c56bd8885926c9a9374a31ed7c`  
		Last Modified: Fri, 23 Jul 2021 00:22:32 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2922ffac0f77cf1fd832a20d48b586a6621e1d75610c055227f6d76e34928b16`  
		Last Modified: Fri, 23 Jul 2021 00:23:09 GMT  
		Size: 95.7 MB (95703233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb8c5967872202784509fa53a811f849c714ef794dd53a40047d0c81585ce4`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c1ffe6294aae5e8df812aee47c20e59fe0f4ec3593946e4ed069116ebb9f1`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f26aa32bafd59c6d9237ded27dc8ab964a91915e3b9a678b76d587899376ec`  
		Last Modified: Fri, 23 Jul 2021 00:22:31 GMT  
		Size: 3.1 MB (3058690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba425f932ee35d618a7e2a024cf68062985ba8dbbedbfd829e6af8cb1d1978b6`  
		Last Modified: Fri, 23 Jul 2021 00:22:45 GMT  
		Size: 44.3 MB (44334640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bca1f4ee34a1ccde3aac51ad07cafbaa3d857e77059427b1f928f48da6a0134`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 1.8 KB (1797 bytes)  
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
$ docker pull redmine@sha256:37201304a98b29096c65aff1082800685f8811d091fecfdbbfbc4b02ce56c712
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202549844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cceccec5920cb372b1e0e6536384018db9d2cf92a8ccf57721c5e55ec24b272`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:03:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:03:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:03:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:23:01 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 14:23:02 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 14:23:03 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 14:26:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:26:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:26:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:26:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:26:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:26:30 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 02:07:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:08:34 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 02:08:34 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 02:08:34 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 02:08:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 02:08:35 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 02:08:36 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 02:08:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 02:10:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 02:10:31 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 02:10:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 02:10:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:10:32 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 02:10:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d658cd93dd34abb2452544d10308c796ec6310f6d1ca2d2762c8e85402e3e`  
		Last Modified: Thu, 22 Jul 2021 14:48:41 GMT  
		Size: 10.8 MB (10814518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bebc1f15c6904197539abc99a69885fa65493d7fae9f27d2529be2fa05491e`  
		Last Modified: Thu, 22 Jul 2021 14:48:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa61230ad4685d16dfcb4b68dd88f40b84ddf598a2031852e9881218e137c19a`  
		Last Modified: Thu, 22 Jul 2021 14:49:27 GMT  
		Size: 14.7 MB (14697201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f9ff30668a8bd8fd8341049bbebd3d1db4e433d0116f70111daa596abf7e7a`  
		Last Modified: Thu, 22 Jul 2021 14:49:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91522d35fa6424129e9d5eb39ac436e70fd9e80337413131aa3401b1496857ff`  
		Last Modified: Fri, 23 Jul 2021 02:17:18 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5900d840b86d971e896fc6c7451e9a176bd80fa994f5090d5dbcf5ef6e48b14`  
		Last Modified: Fri, 23 Jul 2021 02:17:31 GMT  
		Size: 91.8 MB (91790782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede4b68f2bb6676b42e076513a0c075e3da52f75acb4070789e5d12196646541`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add04b7bc101933c98b8043337844f9e18f272fd13d47b87100f4fd9f52710b2`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51111bc126246f79519ed7c546b73f24285cc97694e205b48267a20ba50637f2`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 3.1 MB (3058684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad5d1e67f7c62f6d33343a9632c4aca3d5c808a4a4a18a476fcad4acf39bdb`  
		Last Modified: Fri, 23 Jul 2021 02:17:26 GMT  
		Size: 56.4 MB (56423655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c540e32ed87a6e82bdca054e93ee83775afa16fab29404772b98d2a047156a0c`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:7de4015773da4d105b5f43705556003eb3071d781612fa6e7f6010981e4e56e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull redmine@sha256:4198d395967db00ec073ed9d714c41b00472e77e49b0dcae51f259d9b78dbc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:43a77f34a70b4e12264df8bff7377b5ae47895166cfd156a903cb28b641fec29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0604330a8f415b11297aee811ea898c9a092e3255eb53a843e412e37469ba9d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 17:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:28:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:28:25 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:03:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:04:03 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:04:03 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:04:03 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:04:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 11:04:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:04:49 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:04:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:49 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:04:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 23 Jul 2021 11:04:59 GMT
ENV PASSENGER_VERSION=6.0.10
# Fri, 23 Jul 2021 11:05:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:05:16 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 23 Jul 2021 11:05:17 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 23 Jul 2021 11:05:17 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e582c090726ff249b7e30253c7f0c11aa2cd14282a8b6cd0e8055c8615e5586`  
		Last Modified: Thu, 22 Jul 2021 17:42:40 GMT  
		Size: 14.5 MB (14509812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f96a83aedee46aef2be1d4f73cc6990dc7e756981b022462100ac16fad345`  
		Last Modified: Thu, 22 Jul 2021 17:42:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9466f2ac94d013cc74523ee4ad44d9720c72baa51d8aecc2afcba41c3754be44`  
		Last Modified: Fri, 23 Jul 2021 11:10:32 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbad6372ccefa1ce14b5eefe2fe718c0cd234b40bf9a70e3d02e131a9dd65d26`  
		Last Modified: Fri, 23 Jul 2021 11:10:45 GMT  
		Size: 94.1 MB (94087869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93724991108aa18238773a3122f3fcd80f69331610c0a7f00656f690ac7692`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19466676666dc7f1a145b5b2534855e6f32c152cd3da118bc5536badc24da33d`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc48a22ec231d5048d556cd637291655083a29acb695b0073039d36315929da`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 3.1 MB (3058677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00b1336ee6986b3f2923502d082ce45ebccea58e21f85ddd12812be6796e1f`  
		Last Modified: Fri, 23 Jul 2021 11:10:33 GMT  
		Size: 44.1 MB (44106755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fe342d55cb9155ec0d7a14a371258946d43b0b4e3df44e3f1bbe9b166a5ef`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8e911f2db9cefa3945c1c8bbcc4e9dc79575560305045da7e987dfa48fa522`  
		Last Modified: Fri, 23 Jul 2021 11:11:07 GMT  
		Size: 21.1 MB (21131293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab210a34ab4fa48ee042162c1b27897332d05666f95bb001a39f2d04a7df605`  
		Last Modified: Fri, 23 Jul 2021 11:11:05 GMT  
		Size: 4.9 MB (4919283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0`

```console
$ docker pull redmine@sha256:caba7437e2d76511c65b3cb4c928935b4e3ba976c73e8854233716e0930c3bec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.0` - linux; amd64

```console
$ docker pull redmine@sha256:a30cd3dc5580f5966689be984309a4c58b44a1ecb3ce8a989f0712765b575b6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205072160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fd81a2ff1ed6cd5076a6a870886dec018329cd0f3bdf1047393351eed3a2b4f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 17:31:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 17:34:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:34:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:34:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:34:07 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:05:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:07:36 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:07:36 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:07:37 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:07:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:07:38 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 11:07:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 11:07:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:09:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:09:35 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:09:35 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:09:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:09:35 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:09:36 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b7373cf9d9195064da3c92860c7157644c595720fffd5bb48615ac96985d5`  
		Last Modified: Thu, 22 Jul 2021 17:43:38 GMT  
		Size: 21.5 MB (21468044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb83e25b0fb68c5c98194adb0ad3740bc7d2242801c213e7d7949281f901679`  
		Last Modified: Thu, 22 Jul 2021 17:43:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61371aadcf232eb667c47dbba436a5611088d97ba4c8a9bd0c271f36882b027d`  
		Last Modified: Fri, 23 Jul 2021 11:11:30 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0527440fec380cb5ffab3044cdb10895391dd8c0967dbf50c94f5a6ac54cbe48`  
		Last Modified: Fri, 23 Jul 2021 11:12:23 GMT  
		Size: 81.2 MB (81200505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ead518ac18671d74e03ee9c8d93c71f9ced66c21ba86bcc2c503a8e5c8326b`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f008d376270911f79e7e6c177b16b77b13d0309adcd8dd7266e1bf0b2b4dd9`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9566b0985629bf3ebfee385cb50b88bb50798e5ae4b5c4dbb87298c9baedf66e`  
		Last Modified: Fri, 23 Jul 2021 11:12:09 GMT  
		Size: 2.5 MB (2542546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe2b1704c38fcd44f73cfa4cd5ed3ee7c7c9182e905d3bda2bad7457e7478f2`  
		Last Modified: Fri, 23 Jul 2021 11:12:15 GMT  
		Size: 60.1 MB (60148250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0011d8346df5b8d0b6540960e13a4a200f5fd7cd2283b3d0c7e0e3d61856f2c5`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:f68b890b9070068d1d1e4d2e129b6a2588f712889ef062ee4ba10ed3208024de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194719441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb736ee279c270380b4ea5b0c9aeef3d9e76b9e17b589c178f12c5e569445a2b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:39:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 15:01:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:02:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:02:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:02:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:02:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:02:04 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:32:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:40:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:40:50 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:40:51 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:40:51 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:40:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:40:53 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 01:40:53 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 01:40:59 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:47:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:47:02 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:47:02 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:47:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:47:03 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:47:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9237058b7c5120d5c6315b5d17a8c1d783be09a228b83772111ce9436c29d078`  
		Last Modified: Thu, 22 Jul 2021 15:15:34 GMT  
		Size: 10.3 MB (10345807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144b4344f580222d2fbc2f0d80fc139ab1a1ddb9a245b6073c41fdca9a93c23e`  
		Last Modified: Thu, 22 Jul 2021 15:15:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae149ea188f1e064a0256560e0273ae4b331a42ab93326fd9a79753cfb63299d`  
		Last Modified: Thu, 22 Jul 2021 15:18:00 GMT  
		Size: 20.7 MB (20733368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5d2d97d7d53265f79bb7d6b5cfc05f237e3d237d9cf22475536aa4fd57ccde`  
		Last Modified: Thu, 22 Jul 2021 15:17:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822c77937c7bc9bc3d506cf3a12ef2ada0bdbc4c0db3af2efaecc31c4191df4a`  
		Last Modified: Fri, 23 Jul 2021 01:49:24 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf88d0b525291c8ed7e29e9e8ba21a25a8c186e2b45bbe036f6b45b60dbb725`  
		Last Modified: Fri, 23 Jul 2021 01:51:32 GMT  
		Size: 77.0 MB (76965230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fc97807986ce68b1adaf43768244b0f7feb0b45a3693494d303a9bde78206`  
		Last Modified: Fri, 23 Jul 2021 01:50:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da90621c3344a001d962d4e9ee37ee08502d9a1d4c1a26e40082177f7d78eb9`  
		Last Modified: Fri, 23 Jul 2021 01:50:40 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d126519049a526572ad6fbdff768305806b6cf0b42a0707007187491835a6`  
		Last Modified: Fri, 23 Jul 2021 01:50:43 GMT  
		Size: 2.5 MB (2542540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457820c2404a0f956447bb7bde617741101e1b6ac11c79c7dc9e4ba284f06fb`  
		Last Modified: Fri, 23 Jul 2021 01:51:09 GMT  
		Size: 59.2 MB (59249171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae53e60f882218b768c0d7ea4a5a40fbe5512f79710f794079f92caa7a225d1`  
		Last Modified: Fri, 23 Jul 2021 01:50:40 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:adaecf942bcbf470ce5a40970bf2c079bcdcc70921efddada7897d7966c86313
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.1 MB (188053580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afae75ed20002c892916b188691ea63f8643a55ed5c8b26670d0ad3c396ed670`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:15:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 02:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 02:46:35 GMT
ENV RUBY_MAJOR=2.6
# Fri, 23 Jul 2021 02:46:35 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 23 Jul 2021 02:46:36 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 23 Jul 2021 02:50:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 02:50:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 02:50:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 02:50:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:50:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 02:50:43 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 21:25:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 21:33:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 21:33:10 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 21:33:11 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 21:33:11 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 21:33:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 21:33:13 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 21:33:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 21:33:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 21:38:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 21:38:54 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 21:38:55 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 21:38:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 21:38:56 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 21:38:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b8c791d70de7f22816846fbb07e0a1d7d419841c7e539a7cf57ef05fd50c5`  
		Last Modified: Fri, 23 Jul 2021 03:05:10 GMT  
		Size: 9.9 MB (9872218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12a7edb0af862efa24dc389d7901cd2a894f2e106a1cef931ba0a6d675e2c0`  
		Last Modified: Fri, 23 Jul 2021 03:05:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0837e4e34dc8fe0ec9567b99bb7b1397a813fca3b43abfbbd75ee231a946a979`  
		Last Modified: Fri, 23 Jul 2021 03:07:54 GMT  
		Size: 20.6 MB (20643760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c76309d8689f06c398ddc0f6b5ec99a408c65c613d73d63fb9f5101ebe3e2a1`  
		Last Modified: Fri, 23 Jul 2021 03:07:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c349a607ae692434577c905a1f4029d996cee89a0c9f214fa866ac935ceddf23`  
		Last Modified: Fri, 23 Jul 2021 21:41:16 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8cee36193dcad9a6170ac7b62624990e45bd8e40f280263cbc385102b815b5`  
		Last Modified: Fri, 23 Jul 2021 21:43:15 GMT  
		Size: 73.3 MB (73264161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cab5b19ebed7ef72637004e6d5caa4c8e6339b68a5858b092f7969de48022`  
		Last Modified: Fri, 23 Jul 2021 21:42:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19aa70a44bb3a34cdec8010dc14c194820f60d59bb588e122bb488dc1c65dc40`  
		Last Modified: Fri, 23 Jul 2021 21:42:27 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f27c773a3f3c9a852c5331d84ab63be28de904da75fa384a2b36a9ebc45b27`  
		Last Modified: Fri, 23 Jul 2021 21:42:31 GMT  
		Size: 2.5 MB (2542541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ac45246d6c17b1fb3dd54ad65b762e50f7ca0eb448a4137ada4f6896ef5925`  
		Last Modified: Fri, 23 Jul 2021 21:42:55 GMT  
		Size: 59.0 MB (58980689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a33b1a2d4b8fa224e96757684c0e214ff8c5922ab1ca4606c39b3ee25dcadfd`  
		Last Modified: Fri, 23 Jul 2021 21:42:27 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:93221f748263c5d02e684d36684199936fdf7a8ef79b13c0852a6d0d3eb59d48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200855495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9a898ad3f81579b3d202a6989d413b2a30bfe263d48c4835794cfb61b4bf14`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 12:36:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 12:45:29 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 12:45:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 12:45:30 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 12:47:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 12:47:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 12:47:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 12:47:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 12:47:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 12:47:36 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:00:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:03:54 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:03:54 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:03:55 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:03:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:03:56 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 01:03:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 01:03:59 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:06:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:06:08 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:06:08 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:06:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:06:09 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:06:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a77364b6ec6cfc9422903e0f9d3f5cab5ee0ac4b62cfac6fc7c3d544ad7f57`  
		Last Modified: Thu, 22 Jul 2021 12:55:11 GMT  
		Size: 11.3 MB (11263053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a68321ef048d82e4480bc2de1681a811f18b2e1d04b5aa9dec38030570eaa40`  
		Last Modified: Thu, 22 Jul 2021 12:55:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319f6f39ac757356a2f054631df2eaa6a111934c0e9128d04df9f2296eef143`  
		Last Modified: Thu, 22 Jul 2021 12:57:16 GMT  
		Size: 21.3 MB (21308954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3246f58f273186efdfacba513b296257ca20afe8e09b07635bf20c90f80cc2eb`  
		Last Modified: Thu, 22 Jul 2021 12:57:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11d0bb585455c7f2d643b57d83d2bc79e83d4fa6102af98583c50395fdd42c`  
		Last Modified: Fri, 23 Jul 2021 01:07:19 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375134184cebc606b89095d0b132416bd9b69c73df8b06ea6af8c485bb0b9adc`  
		Last Modified: Fri, 23 Jul 2021 01:08:02 GMT  
		Size: 79.7 MB (79748997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf089d6b3f78baf81252c1eae0ab3a7a82944009d9316388ff73eab9f144560`  
		Last Modified: Fri, 23 Jul 2021 01:07:46 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987ebf8a8028e228f7478bd868eb128cb45c42266e298d26ceb7bc0de2066378`  
		Last Modified: Fri, 23 Jul 2021 01:07:46 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a9636a7b709451a363ff59ac6bd72369775c7c0f0d92987983c86782837328`  
		Last Modified: Fri, 23 Jul 2021 01:07:47 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692c6cb8ddbfb8f182f8660aef3067b7a2620eb33dde49301c5a2fa894ac7629`  
		Last Modified: Fri, 23 Jul 2021 01:07:54 GMT  
		Size: 60.1 MB (60072909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4579613c66cfd03c2c406bfb0c96a8776c47c96dd408ec22bd55db34227ebf89`  
		Last Modified: Fri, 23 Jul 2021 01:07:46 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; 386

```console
$ docker pull redmine@sha256:9b4b725043561fc6f093b1805ecf81bd81c278ff9900fe39a00e413d9864647c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210332451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21c08cabd048f1e2a1a723cb64800b532c989486494956a12e85e74c7cbd805`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:38:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:39:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 15:39:00 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 15:53:08 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 15:53:09 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 15:53:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 15:56:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:56:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:56:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:56:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:56:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:56:29 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:13:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:17:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:17:17 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:17:18 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:17:18 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:17:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:17:20 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 00:17:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 00:17:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 00:21:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 00:21:42 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 00:21:43 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 00:21:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 00:21:44 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 00:21:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d04ca5200ad3b98494cfde36960022dbd29c9afc33d685ac499fae8a05d63`  
		Last Modified: Thu, 22 Jul 2021 16:06:57 GMT  
		Size: 17.2 MB (17227285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d9d06c9e919afbd9358b702cad5bc0f28b8150722ffedb25ece16dc1f19b2`  
		Last Modified: Thu, 22 Jul 2021 16:06:48 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3172650cf56a46da1b8438a86468d4053edf77c17eaad06d10b7c7a4f89d13ff`  
		Last Modified: Thu, 22 Jul 2021 16:09:12 GMT  
		Size: 20.9 MB (20910118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686761ac4b88297af44e82ba027c5c73411fe3e728b11bbdc631ea19cae4207`  
		Last Modified: Thu, 22 Jul 2021 16:09:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd85881cfa469c977c54673a6f7a5069bd5524e91c3dcc68765e8c34126cabe2`  
		Last Modified: Fri, 23 Jul 2021 00:23:41 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50e9554d325af14ff7a934082d622c3943218047ed2aa4294b0c7535581244b`  
		Last Modified: Fri, 23 Jul 2021 00:25:08 GMT  
		Size: 82.6 MB (82599806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a2d230fb36dab9b19e500fa31f006d0eeee505ceff2925ba4be6e11f79e7cb`  
		Last Modified: Fri, 23 Jul 2021 00:24:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab5662ff0e835add5c4df375cbd7a031f48ab605541cefdee4c0d951b6a724`  
		Last Modified: Fri, 23 Jul 2021 00:24:33 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fb67e4236a41bcff9cbb8e3a50fb0448092b2e9c48698898fd97c9be5596d6`  
		Last Modified: Fri, 23 Jul 2021 00:24:35 GMT  
		Size: 2.5 MB (2542547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce6344df4fd2a77ff42e131656f0ecabf7e82245e9baa99c29bbd0d0f746fbf`  
		Last Modified: Fri, 23 Jul 2021 00:24:54 GMT  
		Size: 59.3 MB (59251004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9705ef65a1f1f76bc1e8bc800dc07a0a770e8e1bf07b138f90cf1d3126ba5f38`  
		Last Modified: Fri, 23 Jul 2021 00:24:33 GMT  
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
$ docker pull redmine@sha256:ba02f2b9d3a6c7c5a90d3826a617672508f538c3ab9adf92805e6ae7482fa60c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200266058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e599e96ea8b62cc503927450a3747d1038fbd79e8e031f8012a4e42ff48357b7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:03:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:03:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:03:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:38:29 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 14:38:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 14:38:31 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 14:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:42:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:42:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:42:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:42:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:42:37 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 02:10:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 02:14:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:14:15 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 02:14:15 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 02:14:15 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 02:14:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 02:14:17 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 02:14:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 02:14:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 02:16:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 02:16:48 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 02:16:48 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 02:16:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:16:48 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 02:16:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d658cd93dd34abb2452544d10308c796ec6310f6d1ca2d2762c8e85402e3e`  
		Last Modified: Thu, 22 Jul 2021 14:48:41 GMT  
		Size: 10.8 MB (10814518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bebc1f15c6904197539abc99a69885fa65493d7fae9f27d2529be2fa05491e`  
		Last Modified: Thu, 22 Jul 2021 14:48:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f561c255d99a491c5b43abff939ba38e74ae544c4075fb8c14e7c01f0a932d`  
		Last Modified: Thu, 22 Jul 2021 14:50:04 GMT  
		Size: 21.6 MB (21620156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556bb48ca77fd1659ce0e0ef9979115f34bd73b84af8bdc963902aa6ee99b83d`  
		Last Modified: Thu, 22 Jul 2021 14:50:02 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eb91b4d29f39917d9f1202634b78d331a8353110334caeaaf943d784e262`  
		Last Modified: Fri, 23 Jul 2021 02:17:45 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72298f76fa86070ebb18972e0cd30af4095a1aa64e23d895bc1455c95d83170`  
		Last Modified: Fri, 23 Jul 2021 02:18:19 GMT  
		Size: 78.9 MB (78942606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60556b795d8017dbeaacd27a9fd9099b77593ea2a3a1811135b26d4d3d08df2`  
		Last Modified: Fri, 23 Jul 2021 02:18:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6696136f4aba936491ab5a63b3e9cd6b7bd9097956ec53fd8ed0ef38b37910a7`  
		Last Modified: Fri, 23 Jul 2021 02:18:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4ac44b925e628705888a936de35c7be3d4171c45572c99b7159bb3395b845`  
		Last Modified: Fri, 23 Jul 2021 02:18:08 GMT  
		Size: 2.5 MB (2542547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06cbb89aa31f54918a30c35b4d6d57d5af81a2d923ec2d3c0382d50d676e9d3`  
		Last Modified: Fri, 23 Jul 2021 02:18:13 GMT  
		Size: 60.6 MB (60581220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c5fa94f6e8c4822a33c9a285684513c449af6d1719265b047273d3d92c3576`  
		Last Modified: Fri, 23 Jul 2021 02:18:06 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-alpine`

```console
$ docker pull redmine@sha256:9b8ec4df56622e6060cfc701a5059050c3b734da828cc8f154367d016ac22227
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull redmine@sha256:319dd08d03106ba06b96a6c2c211c7bdbdf6671de495c0b1a1e270098bf3cb85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:0d1a0ccbcaa59efb65e98fbf387d0cf046cb38a46c274cb0e25ca9e2aa13d165
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231318767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c59b0c8114ee55abb9152e916fd05b8ced427af548ff6d169917a286874784`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 17:31:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 17:34:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:34:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:34:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:34:07 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:05:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:07:36 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:07:36 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:07:37 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:07:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:07:38 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 11:07:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 11:07:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:09:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:09:35 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:09:35 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:09:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:09:35 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:09:36 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 23 Jul 2021 11:09:39 GMT
ENV PASSENGER_VERSION=6.0.10
# Fri, 23 Jul 2021 11:09:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:09:57 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 23 Jul 2021 11:09:57 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 23 Jul 2021 11:09:58 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b7373cf9d9195064da3c92860c7157644c595720fffd5bb48615ac96985d5`  
		Last Modified: Thu, 22 Jul 2021 17:43:38 GMT  
		Size: 21.5 MB (21468044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb83e25b0fb68c5c98194adb0ad3740bc7d2242801c213e7d7949281f901679`  
		Last Modified: Thu, 22 Jul 2021 17:43:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61371aadcf232eb667c47dbba436a5611088d97ba4c8a9bd0c271f36882b027d`  
		Last Modified: Fri, 23 Jul 2021 11:11:30 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0527440fec380cb5ffab3044cdb10895391dd8c0967dbf50c94f5a6ac54cbe48`  
		Last Modified: Fri, 23 Jul 2021 11:12:23 GMT  
		Size: 81.2 MB (81200505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ead518ac18671d74e03ee9c8d93c71f9ced66c21ba86bcc2c503a8e5c8326b`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f008d376270911f79e7e6c177b16b77b13d0309adcd8dd7266e1bf0b2b4dd9`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9566b0985629bf3ebfee385cb50b88bb50798e5ae4b5c4dbb87298c9baedf66e`  
		Last Modified: Fri, 23 Jul 2021 11:12:09 GMT  
		Size: 2.5 MB (2542546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe2b1704c38fcd44f73cfa4cd5ed3ee7c7c9182e905d3bda2bad7457e7478f2`  
		Last Modified: Fri, 23 Jul 2021 11:12:15 GMT  
		Size: 60.1 MB (60148250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0011d8346df5b8d0b6540960e13a4a200f5fd7cd2283b3d0c7e0e3d61856f2c5`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4115f43d92079ea0e1fd41e8d42467fc73d3b96a655e7eeaf1ceed99049832cf`  
		Last Modified: Fri, 23 Jul 2021 11:12:37 GMT  
		Size: 21.3 MB (21327322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923adc728211126334159e16d7a0931ea37967801e506f3f0eb071d26ced3762`  
		Last Modified: Fri, 23 Jul 2021 11:12:35 GMT  
		Size: 4.9 MB (4919285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9`

```console
$ docker pull redmine@sha256:caba7437e2d76511c65b3cb4c928935b4e3ba976c73e8854233716e0930c3bec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.0.9` - linux; amd64

```console
$ docker pull redmine@sha256:a30cd3dc5580f5966689be984309a4c58b44a1ecb3ce8a989f0712765b575b6a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205072160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fd81a2ff1ed6cd5076a6a870886dec018329cd0f3bdf1047393351eed3a2b4f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 17:31:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 17:34:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:34:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:34:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:34:07 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:05:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:07:36 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:07:36 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:07:37 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:07:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:07:38 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 11:07:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 11:07:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:09:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:09:35 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:09:35 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:09:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:09:35 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:09:36 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b7373cf9d9195064da3c92860c7157644c595720fffd5bb48615ac96985d5`  
		Last Modified: Thu, 22 Jul 2021 17:43:38 GMT  
		Size: 21.5 MB (21468044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb83e25b0fb68c5c98194adb0ad3740bc7d2242801c213e7d7949281f901679`  
		Last Modified: Thu, 22 Jul 2021 17:43:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61371aadcf232eb667c47dbba436a5611088d97ba4c8a9bd0c271f36882b027d`  
		Last Modified: Fri, 23 Jul 2021 11:11:30 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0527440fec380cb5ffab3044cdb10895391dd8c0967dbf50c94f5a6ac54cbe48`  
		Last Modified: Fri, 23 Jul 2021 11:12:23 GMT  
		Size: 81.2 MB (81200505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ead518ac18671d74e03ee9c8d93c71f9ced66c21ba86bcc2c503a8e5c8326b`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f008d376270911f79e7e6c177b16b77b13d0309adcd8dd7266e1bf0b2b4dd9`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9566b0985629bf3ebfee385cb50b88bb50798e5ae4b5c4dbb87298c9baedf66e`  
		Last Modified: Fri, 23 Jul 2021 11:12:09 GMT  
		Size: 2.5 MB (2542546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe2b1704c38fcd44f73cfa4cd5ed3ee7c7c9182e905d3bda2bad7457e7478f2`  
		Last Modified: Fri, 23 Jul 2021 11:12:15 GMT  
		Size: 60.1 MB (60148250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0011d8346df5b8d0b6540960e13a4a200f5fd7cd2283b3d0c7e0e3d61856f2c5`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm variant v5

```console
$ docker pull redmine@sha256:f68b890b9070068d1d1e4d2e129b6a2588f712889ef062ee4ba10ed3208024de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194719441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb736ee279c270380b4ea5b0c9aeef3d9e76b9e17b589c178f12c5e569445a2b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:39:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 15:01:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:02:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:02:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:02:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:02:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:02:04 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:32:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:40:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:40:50 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:40:51 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:40:51 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:40:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:40:53 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 01:40:53 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 01:40:59 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:47:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:47:02 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:47:02 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:47:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:47:03 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:47:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9237058b7c5120d5c6315b5d17a8c1d783be09a228b83772111ce9436c29d078`  
		Last Modified: Thu, 22 Jul 2021 15:15:34 GMT  
		Size: 10.3 MB (10345807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144b4344f580222d2fbc2f0d80fc139ab1a1ddb9a245b6073c41fdca9a93c23e`  
		Last Modified: Thu, 22 Jul 2021 15:15:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae149ea188f1e064a0256560e0273ae4b331a42ab93326fd9a79753cfb63299d`  
		Last Modified: Thu, 22 Jul 2021 15:18:00 GMT  
		Size: 20.7 MB (20733368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5d2d97d7d53265f79bb7d6b5cfc05f237e3d237d9cf22475536aa4fd57ccde`  
		Last Modified: Thu, 22 Jul 2021 15:17:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822c77937c7bc9bc3d506cf3a12ef2ada0bdbc4c0db3af2efaecc31c4191df4a`  
		Last Modified: Fri, 23 Jul 2021 01:49:24 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf88d0b525291c8ed7e29e9e8ba21a25a8c186e2b45bbe036f6b45b60dbb725`  
		Last Modified: Fri, 23 Jul 2021 01:51:32 GMT  
		Size: 77.0 MB (76965230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259fc97807986ce68b1adaf43768244b0f7feb0b45a3693494d303a9bde78206`  
		Last Modified: Fri, 23 Jul 2021 01:50:40 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da90621c3344a001d962d4e9ee37ee08502d9a1d4c1a26e40082177f7d78eb9`  
		Last Modified: Fri, 23 Jul 2021 01:50:40 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6d126519049a526572ad6fbdff768305806b6cf0b42a0707007187491835a6`  
		Last Modified: Fri, 23 Jul 2021 01:50:43 GMT  
		Size: 2.5 MB (2542540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8457820c2404a0f956447bb7bde617741101e1b6ac11c79c7dc9e4ba284f06fb`  
		Last Modified: Fri, 23 Jul 2021 01:51:09 GMT  
		Size: 59.2 MB (59249171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae53e60f882218b768c0d7ea4a5a40fbe5512f79710f794079f92caa7a225d1`  
		Last Modified: Fri, 23 Jul 2021 01:50:40 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm variant v7

```console
$ docker pull redmine@sha256:adaecf942bcbf470ce5a40970bf2c079bcdcc70921efddada7897d7966c86313
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.1 MB (188053580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afae75ed20002c892916b188691ea63f8643a55ed5c8b26670d0ad3c396ed670`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:15:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 02:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 02:46:35 GMT
ENV RUBY_MAJOR=2.6
# Fri, 23 Jul 2021 02:46:35 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 23 Jul 2021 02:46:36 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 23 Jul 2021 02:50:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 02:50:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 02:50:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 02:50:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:50:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 02:50:43 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 21:25:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 21:33:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 21:33:10 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 21:33:11 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 21:33:11 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 21:33:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 21:33:13 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 21:33:14 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 21:33:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 21:38:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 21:38:54 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 21:38:55 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 21:38:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 21:38:56 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 21:38:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b8c791d70de7f22816846fbb07e0a1d7d419841c7e539a7cf57ef05fd50c5`  
		Last Modified: Fri, 23 Jul 2021 03:05:10 GMT  
		Size: 9.9 MB (9872218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12a7edb0af862efa24dc389d7901cd2a894f2e106a1cef931ba0a6d675e2c0`  
		Last Modified: Fri, 23 Jul 2021 03:05:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0837e4e34dc8fe0ec9567b99bb7b1397a813fca3b43abfbbd75ee231a946a979`  
		Last Modified: Fri, 23 Jul 2021 03:07:54 GMT  
		Size: 20.6 MB (20643760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c76309d8689f06c398ddc0f6b5ec99a408c65c613d73d63fb9f5101ebe3e2a1`  
		Last Modified: Fri, 23 Jul 2021 03:07:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c349a607ae692434577c905a1f4029d996cee89a0c9f214fa866ac935ceddf23`  
		Last Modified: Fri, 23 Jul 2021 21:41:16 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8cee36193dcad9a6170ac7b62624990e45bd8e40f280263cbc385102b815b5`  
		Last Modified: Fri, 23 Jul 2021 21:43:15 GMT  
		Size: 73.3 MB (73264161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51cab5b19ebed7ef72637004e6d5caa4c8e6339b68a5858b092f7969de48022`  
		Last Modified: Fri, 23 Jul 2021 21:42:27 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19aa70a44bb3a34cdec8010dc14c194820f60d59bb588e122bb488dc1c65dc40`  
		Last Modified: Fri, 23 Jul 2021 21:42:27 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f27c773a3f3c9a852c5331d84ab63be28de904da75fa384a2b36a9ebc45b27`  
		Last Modified: Fri, 23 Jul 2021 21:42:31 GMT  
		Size: 2.5 MB (2542541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ac45246d6c17b1fb3dd54ad65b762e50f7ca0eb448a4137ada4f6896ef5925`  
		Last Modified: Fri, 23 Jul 2021 21:42:55 GMT  
		Size: 59.0 MB (58980689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a33b1a2d4b8fa224e96757684c0e214ff8c5922ab1ca4606c39b3ee25dcadfd`  
		Last Modified: Fri, 23 Jul 2021 21:42:27 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:93221f748263c5d02e684d36684199936fdf7a8ef79b13c0852a6d0d3eb59d48
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200855495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9a898ad3f81579b3d202a6989d413b2a30bfe263d48c4835794cfb61b4bf14`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 12:36:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 12:45:29 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 12:45:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 12:45:30 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 12:47:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 12:47:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 12:47:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 12:47:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 12:47:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 12:47:36 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:00:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:03:54 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:03:54 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:03:55 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:03:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:03:56 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 01:03:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 01:03:59 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:06:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:06:08 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:06:08 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:06:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:06:09 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:06:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a77364b6ec6cfc9422903e0f9d3f5cab5ee0ac4b62cfac6fc7c3d544ad7f57`  
		Last Modified: Thu, 22 Jul 2021 12:55:11 GMT  
		Size: 11.3 MB (11263053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a68321ef048d82e4480bc2de1681a811f18b2e1d04b5aa9dec38030570eaa40`  
		Last Modified: Thu, 22 Jul 2021 12:55:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319f6f39ac757356a2f054631df2eaa6a111934c0e9128d04df9f2296eef143`  
		Last Modified: Thu, 22 Jul 2021 12:57:16 GMT  
		Size: 21.3 MB (21308954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3246f58f273186efdfacba513b296257ca20afe8e09b07635bf20c90f80cc2eb`  
		Last Modified: Thu, 22 Jul 2021 12:57:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11d0bb585455c7f2d643b57d83d2bc79e83d4fa6102af98583c50395fdd42c`  
		Last Modified: Fri, 23 Jul 2021 01:07:19 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375134184cebc606b89095d0b132416bd9b69c73df8b06ea6af8c485bb0b9adc`  
		Last Modified: Fri, 23 Jul 2021 01:08:02 GMT  
		Size: 79.7 MB (79748997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf089d6b3f78baf81252c1eae0ab3a7a82944009d9316388ff73eab9f144560`  
		Last Modified: Fri, 23 Jul 2021 01:07:46 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987ebf8a8028e228f7478bd868eb128cb45c42266e298d26ceb7bc0de2066378`  
		Last Modified: Fri, 23 Jul 2021 01:07:46 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a9636a7b709451a363ff59ac6bd72369775c7c0f0d92987983c86782837328`  
		Last Modified: Fri, 23 Jul 2021 01:07:47 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692c6cb8ddbfb8f182f8660aef3067b7a2620eb33dde49301c5a2fa894ac7629`  
		Last Modified: Fri, 23 Jul 2021 01:07:54 GMT  
		Size: 60.1 MB (60072909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4579613c66cfd03c2c406bfb0c96a8776c47c96dd408ec22bd55db34227ebf89`  
		Last Modified: Fri, 23 Jul 2021 01:07:46 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; 386

```console
$ docker pull redmine@sha256:9b4b725043561fc6f093b1805ecf81bd81c278ff9900fe39a00e413d9864647c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210332451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d21c08cabd048f1e2a1a723cb64800b532c989486494956a12e85e74c7cbd805`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:38:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:39:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 15:39:00 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 15:53:08 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 15:53:09 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 15:53:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 15:56:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:56:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:56:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:56:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:56:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:56:29 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:13:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:17:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:17:17 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:17:18 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:17:18 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:17:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:17:20 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 00:17:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 00:17:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 00:21:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 00:21:42 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 00:21:43 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 00:21:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 00:21:44 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 00:21:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d04ca5200ad3b98494cfde36960022dbd29c9afc33d685ac499fae8a05d63`  
		Last Modified: Thu, 22 Jul 2021 16:06:57 GMT  
		Size: 17.2 MB (17227285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d9d06c9e919afbd9358b702cad5bc0f28b8150722ffedb25ece16dc1f19b2`  
		Last Modified: Thu, 22 Jul 2021 16:06:48 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3172650cf56a46da1b8438a86468d4053edf77c17eaad06d10b7c7a4f89d13ff`  
		Last Modified: Thu, 22 Jul 2021 16:09:12 GMT  
		Size: 20.9 MB (20910118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686761ac4b88297af44e82ba027c5c73411fe3e728b11bbdc631ea19cae4207`  
		Last Modified: Thu, 22 Jul 2021 16:09:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd85881cfa469c977c54673a6f7a5069bd5524e91c3dcc68765e8c34126cabe2`  
		Last Modified: Fri, 23 Jul 2021 00:23:41 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d50e9554d325af14ff7a934082d622c3943218047ed2aa4294b0c7535581244b`  
		Last Modified: Fri, 23 Jul 2021 00:25:08 GMT  
		Size: 82.6 MB (82599806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a2d230fb36dab9b19e500fa31f006d0eeee505ceff2925ba4be6e11f79e7cb`  
		Last Modified: Fri, 23 Jul 2021 00:24:33 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ab5662ff0e835add5c4df375cbd7a031f48ab605541cefdee4c0d951b6a724`  
		Last Modified: Fri, 23 Jul 2021 00:24:33 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64fb67e4236a41bcff9cbb8e3a50fb0448092b2e9c48698898fd97c9be5596d6`  
		Last Modified: Fri, 23 Jul 2021 00:24:35 GMT  
		Size: 2.5 MB (2542547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce6344df4fd2a77ff42e131656f0ecabf7e82245e9baa99c29bbd0d0f746fbf`  
		Last Modified: Fri, 23 Jul 2021 00:24:54 GMT  
		Size: 59.3 MB (59251004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9705ef65a1f1f76bc1e8bc800dc07a0a770e8e1bf07b138f90cf1d3126ba5f38`  
		Last Modified: Fri, 23 Jul 2021 00:24:33 GMT  
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
$ docker pull redmine@sha256:ba02f2b9d3a6c7c5a90d3826a617672508f538c3ab9adf92805e6ae7482fa60c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200266058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e599e96ea8b62cc503927450a3747d1038fbd79e8e031f8012a4e42ff48357b7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:03:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:03:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:03:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:38:29 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 14:38:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 14:38:31 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 14:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:42:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:42:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:42:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:42:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:42:37 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 02:10:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 02:14:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:14:15 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 02:14:15 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 02:14:15 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 02:14:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 02:14:17 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 02:14:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 02:14:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 02:16:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 02:16:48 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 02:16:48 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 02:16:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:16:48 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 02:16:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d658cd93dd34abb2452544d10308c796ec6310f6d1ca2d2762c8e85402e3e`  
		Last Modified: Thu, 22 Jul 2021 14:48:41 GMT  
		Size: 10.8 MB (10814518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bebc1f15c6904197539abc99a69885fa65493d7fae9f27d2529be2fa05491e`  
		Last Modified: Thu, 22 Jul 2021 14:48:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f561c255d99a491c5b43abff939ba38e74ae544c4075fb8c14e7c01f0a932d`  
		Last Modified: Thu, 22 Jul 2021 14:50:04 GMT  
		Size: 21.6 MB (21620156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556bb48ca77fd1659ce0e0ef9979115f34bd73b84af8bdc963902aa6ee99b83d`  
		Last Modified: Thu, 22 Jul 2021 14:50:02 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eb91b4d29f39917d9f1202634b78d331a8353110334caeaaf943d784e262`  
		Last Modified: Fri, 23 Jul 2021 02:17:45 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f72298f76fa86070ebb18972e0cd30af4095a1aa64e23d895bc1455c95d83170`  
		Last Modified: Fri, 23 Jul 2021 02:18:19 GMT  
		Size: 78.9 MB (78942606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60556b795d8017dbeaacd27a9fd9099b77593ea2a3a1811135b26d4d3d08df2`  
		Last Modified: Fri, 23 Jul 2021 02:18:08 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6696136f4aba936491ab5a63b3e9cd6b7bd9097956ec53fd8ed0ef38b37910a7`  
		Last Modified: Fri, 23 Jul 2021 02:18:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b4ac44b925e628705888a936de35c7be3d4171c45572c99b7159bb3395b845`  
		Last Modified: Fri, 23 Jul 2021 02:18:08 GMT  
		Size: 2.5 MB (2542547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06cbb89aa31f54918a30c35b4d6d57d5af81a2d923ec2d3c0382d50d676e9d3`  
		Last Modified: Fri, 23 Jul 2021 02:18:13 GMT  
		Size: 60.6 MB (60581220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c5fa94f6e8c4822a33c9a285684513c449af6d1719265b047273d3d92c3576`  
		Last Modified: Fri, 23 Jul 2021 02:18:06 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9-alpine`

```console
$ docker pull redmine@sha256:9b8ec4df56622e6060cfc701a5059050c3b734da828cc8f154367d016ac22227
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull redmine@sha256:319dd08d03106ba06b96a6c2c211c7bdbdf6671de495c0b1a1e270098bf3cb85
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0.9-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:0d1a0ccbcaa59efb65e98fbf387d0cf046cb38a46c274cb0e25ca9e2aa13d165
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231318767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2c59b0c8114ee55abb9152e916fd05b8ced427af548ff6d169917a286874784`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 17:31:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 17:34:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:34:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:34:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:34:07 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:05:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:07:36 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:07:36 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:07:37 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:07:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:07:38 GMT
ENV REDMINE_VERSION=4.0.9
# Fri, 23 Jul 2021 11:07:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Fri, 23 Jul 2021 11:07:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:09:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:09:35 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:09:35 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:09:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:09:35 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:09:36 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 23 Jul 2021 11:09:39 GMT
ENV PASSENGER_VERSION=6.0.10
# Fri, 23 Jul 2021 11:09:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:09:57 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 23 Jul 2021 11:09:57 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 23 Jul 2021 11:09:58 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b7373cf9d9195064da3c92860c7157644c595720fffd5bb48615ac96985d5`  
		Last Modified: Thu, 22 Jul 2021 17:43:38 GMT  
		Size: 21.5 MB (21468044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb83e25b0fb68c5c98194adb0ad3740bc7d2242801c213e7d7949281f901679`  
		Last Modified: Thu, 22 Jul 2021 17:43:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61371aadcf232eb667c47dbba436a5611088d97ba4c8a9bd0c271f36882b027d`  
		Last Modified: Fri, 23 Jul 2021 11:11:30 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0527440fec380cb5ffab3044cdb10895391dd8c0967dbf50c94f5a6ac54cbe48`  
		Last Modified: Fri, 23 Jul 2021 11:12:23 GMT  
		Size: 81.2 MB (81200505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ead518ac18671d74e03ee9c8d93c71f9ced66c21ba86bcc2c503a8e5c8326b`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f008d376270911f79e7e6c177b16b77b13d0309adcd8dd7266e1bf0b2b4dd9`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9566b0985629bf3ebfee385cb50b88bb50798e5ae4b5c4dbb87298c9baedf66e`  
		Last Modified: Fri, 23 Jul 2021 11:12:09 GMT  
		Size: 2.5 MB (2542546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe2b1704c38fcd44f73cfa4cd5ed3ee7c7c9182e905d3bda2bad7457e7478f2`  
		Last Modified: Fri, 23 Jul 2021 11:12:15 GMT  
		Size: 60.1 MB (60148250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0011d8346df5b8d0b6540960e13a4a200f5fd7cd2283b3d0c7e0e3d61856f2c5`  
		Last Modified: Fri, 23 Jul 2021 11:12:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4115f43d92079ea0e1fd41e8d42467fc73d3b96a655e7eeaf1ceed99049832cf`  
		Last Modified: Fri, 23 Jul 2021 11:12:37 GMT  
		Size: 21.3 MB (21327322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923adc728211126334159e16d7a0931ea37967801e506f3f0eb071d26ced3762`  
		Last Modified: Fri, 23 Jul 2021 11:12:35 GMT  
		Size: 4.9 MB (4919285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1`

```console
$ docker pull redmine@sha256:c9f2b5e97a651b2aa2d4c58ff44bca86aefb51a49e4933d7caf7c0d1dfbbff83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.1` - linux; amd64

```console
$ docker pull redmine@sha256:698a793a34357b15ef34472cf146abcc2a011c240197e9a253eab953b3c06708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.6 MB (206647554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0aa676a8efa66732addd34d54f03c6197d78ebf381246c24c101eac35a9549c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 17:31:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 17:34:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:34:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:34:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:34:07 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:05:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:05:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:05:50 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:05:50 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:05:50 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:05:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:05:51 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 11:05:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 11:05:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:06:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:06:34 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:06:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:06:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:06:35 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:06:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b7373cf9d9195064da3c92860c7157644c595720fffd5bb48615ac96985d5`  
		Last Modified: Thu, 22 Jul 2021 17:43:38 GMT  
		Size: 21.5 MB (21468044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb83e25b0fb68c5c98194adb0ad3740bc7d2242801c213e7d7949281f901679`  
		Last Modified: Thu, 22 Jul 2021 17:43:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61371aadcf232eb667c47dbba436a5611088d97ba4c8a9bd0c271f36882b027d`  
		Last Modified: Fri, 23 Jul 2021 11:11:30 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfd1dde1f32f7f8409959b4663cf89b722a2f427f544c5acf3c4dca5ba89961`  
		Last Modified: Fri, 23 Jul 2021 11:11:43 GMT  
		Size: 94.1 MB (94088300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216270a0114d5886d784b5a4bd95e0270c48d34e26e20ced7ee30251aecc0235`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc0835bd828414f95e3e7358066f88a9b754de0e89b47c431fd9eb5f61f4143`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7337fb63fe3caf0b547c29b505ceb48349b11dc5af872eea66c9b09e2da465`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 2.7 MB (2747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2c810419b90595f5b58de487a8545095e85d1f45da97616a70f30cfc579e86`  
		Last Modified: Fri, 23 Jul 2021 11:11:34 GMT  
		Size: 48.6 MB (48630706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7142a912af0cf678a75e06db24614b42621ba3c5594dd958d31308e8d90c361b`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:d3047b6a3f20c53967162e58629dbf5f9bf7d7df656711a4e1d2344c4d2362b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210649914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:906f660eed56fe2f80404754940f80004e24f07fe1aa72b879f072de8414781d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:39:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 15:01:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:02:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:02:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:02:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:02:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:02:04 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:32:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:33:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:33:37 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:33:37 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:33:38 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:33:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:33:40 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 01:33:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 01:33:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:39:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:39:28 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:39:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:39:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:39:30 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:39:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9237058b7c5120d5c6315b5d17a8c1d783be09a228b83772111ce9436c29d078`  
		Last Modified: Thu, 22 Jul 2021 15:15:34 GMT  
		Size: 10.3 MB (10345807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144b4344f580222d2fbc2f0d80fc139ab1a1ddb9a245b6073c41fdca9a93c23e`  
		Last Modified: Thu, 22 Jul 2021 15:15:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae149ea188f1e064a0256560e0273ae4b331a42ab93326fd9a79753cfb63299d`  
		Last Modified: Thu, 22 Jul 2021 15:18:00 GMT  
		Size: 20.7 MB (20733368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5d2d97d7d53265f79bb7d6b5cfc05f237e3d237d9cf22475536aa4fd57ccde`  
		Last Modified: Thu, 22 Jul 2021 15:17:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822c77937c7bc9bc3d506cf3a12ef2ada0bdbc4c0db3af2efaecc31c4191df4a`  
		Last Modified: Fri, 23 Jul 2021 01:49:24 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c50724a36d3c9a8b9ceae430de242d7f6969dbef3ac25c5fde473a8b062cd3`  
		Last Modified: Fri, 23 Jul 2021 01:50:25 GMT  
		Size: 89.6 MB (89576586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64ad6c53bf00acadba6df300f7a60ca8ae5ddc2336b37cd556bbcc18d26566c`  
		Last Modified: Fri, 23 Jul 2021 01:49:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f057554e99e7143804c2bfa6e4ad7c04cbf19075e611550a34de736734ec41c3`  
		Last Modified: Fri, 23 Jul 2021 01:49:22 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890a1a9f8beba551d854feae5c278566e6556b2bb755a4518aa8e17b21a184b8`  
		Last Modified: Fri, 23 Jul 2021 01:49:25 GMT  
		Size: 2.7 MB (2747690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f512938291c851f1276e8ffe92f72cf4a2d4ad57b115945b68d2df77c79bcf`  
		Last Modified: Fri, 23 Jul 2021 01:49:50 GMT  
		Size: 62.4 MB (62363137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e581faafeae657c0d1e349678afd589d102215ba5a2ef10d020cf819e943ff68`  
		Last Modified: Fri, 23 Jul 2021 01:49:22 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:6eebe2e3817e16be90e0203273f1d110ebb3b628d469036fcb1f67560b13c360
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203830389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b70a3855d41ad008f02e50f66b192b32951aaae36adaa23649329aa2636dfad`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:15:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 02:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 02:46:35 GMT
ENV RUBY_MAJOR=2.6
# Fri, 23 Jul 2021 02:46:35 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 23 Jul 2021 02:46:36 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 23 Jul 2021 02:50:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 02:50:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 02:50:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 02:50:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:50:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 02:50:43 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 21:25:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 21:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 21:26:28 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 21:26:29 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 21:26:29 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 21:26:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 21:26:32 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 21:26:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 21:26:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 21:31:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 21:31:57 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 21:31:57 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 21:31:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 21:31:58 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 21:31:58 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b8c791d70de7f22816846fbb07e0a1d7d419841c7e539a7cf57ef05fd50c5`  
		Last Modified: Fri, 23 Jul 2021 03:05:10 GMT  
		Size: 9.9 MB (9872218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12a7edb0af862efa24dc389d7901cd2a894f2e106a1cef931ba0a6d675e2c0`  
		Last Modified: Fri, 23 Jul 2021 03:05:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0837e4e34dc8fe0ec9567b99bb7b1397a813fca3b43abfbbd75ee231a946a979`  
		Last Modified: Fri, 23 Jul 2021 03:07:54 GMT  
		Size: 20.6 MB (20643760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c76309d8689f06c398ddc0f6b5ec99a408c65c613d73d63fb9f5101ebe3e2a1`  
		Last Modified: Fri, 23 Jul 2021 03:07:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c349a607ae692434577c905a1f4029d996cee89a0c9f214fa866ac935ceddf23`  
		Last Modified: Fri, 23 Jul 2021 21:41:16 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2880a64f27ab57a09b4f72db20fc36a50bf3b6a6f3475f8661e8184e4b8acb99`  
		Last Modified: Fri, 23 Jul 2021 21:42:11 GMT  
		Size: 85.6 MB (85590430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455a681e485f6469d2ea0559f66edfbdf6ea359e79d4a5db42bf76287a0de434`  
		Last Modified: Fri, 23 Jul 2021 21:41:15 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac534a0a817b7f2f9c1f1e31c139ea1f9375a72e0f485b0383bc4fc4d59fd2a`  
		Last Modified: Fri, 23 Jul 2021 21:41:14 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c259d05afcbc2a0eb12900c825ff56dcc70e11e07fdb65c78eab33160c0e5101`  
		Last Modified: Fri, 23 Jul 2021 21:41:18 GMT  
		Size: 2.7 MB (2747686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709e390734515835b5ca9e0fef442f6c0d52edad99d53438eabe4f69ee5ecf1f`  
		Last Modified: Fri, 23 Jul 2021 21:41:43 GMT  
		Size: 62.2 MB (62226086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bb46285ccbd31e69fc92ab1250e30fdd2d5555b1673e408f871e9f9e5c5882`  
		Last Modified: Fri, 23 Jul 2021 21:41:14 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:5cc5f6edf0217b06b83a6d9daf43c2595773bcbcef895bcfb558f310e8e31091
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217532817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0a234953326e03a8a215dd562aa68f5ade3010aa21e045a241631da99b8e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 12:36:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 12:45:29 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 12:45:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 12:45:30 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 12:47:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 12:47:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 12:47:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 12:47:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 12:47:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 12:47:36 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:00:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:01:14 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:01:15 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:01:15 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:01:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:01:16 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 01:01:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 01:01:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:03:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:03:25 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:03:25 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:03:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:03:26 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:03:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a77364b6ec6cfc9422903e0f9d3f5cab5ee0ac4b62cfac6fc7c3d544ad7f57`  
		Last Modified: Thu, 22 Jul 2021 12:55:11 GMT  
		Size: 11.3 MB (11263053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a68321ef048d82e4480bc2de1681a811f18b2e1d04b5aa9dec38030570eaa40`  
		Last Modified: Thu, 22 Jul 2021 12:55:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319f6f39ac757356a2f054631df2eaa6a111934c0e9128d04df9f2296eef143`  
		Last Modified: Thu, 22 Jul 2021 12:57:16 GMT  
		Size: 21.3 MB (21308954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3246f58f273186efdfacba513b296257ca20afe8e09b07635bf20c90f80cc2eb`  
		Last Modified: Thu, 22 Jul 2021 12:57:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11d0bb585455c7f2d643b57d83d2bc79e83d4fa6102af98583c50395fdd42c`  
		Last Modified: Fri, 23 Jul 2021 01:07:19 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c1e2df6c95b23a8889c0654161e692541689cbcffaec4d8da108ae9c92bf22`  
		Last Modified: Fri, 23 Jul 2021 01:07:34 GMT  
		Size: 92.6 MB (92611084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c484a1eebcc4d4b1196c27f7f75a74073d9698f5f68a0b86039801f5dbdebf`  
		Last Modified: Fri, 23 Jul 2021 01:07:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc0b0c15a3bb1ec46ee2421b14a404f1d32163bd66d9aa39c4bd340e4d66136`  
		Last Modified: Fri, 23 Jul 2021 01:07:16 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564dafa91638f855756581e6ca8ec66c1b11882217effc7b7b8106960fbd754`  
		Last Modified: Fri, 23 Jul 2021 01:07:17 GMT  
		Size: 2.7 MB (2747697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c9dcd637a9c0101748c513c5f58b49ab12f28e39f3910882bcb2c163d6dff`  
		Last Modified: Fri, 23 Jul 2021 01:07:24 GMT  
		Size: 63.7 MB (63682990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789464e18852a4489c02f3bd68b8e06398cdb0d633f0e232899c4cdc9be1054`  
		Last Modified: Fri, 23 Jul 2021 01:07:16 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; 386

```console
$ docker pull redmine@sha256:1eba46b22559e6801bb7c7084ac6ce0da373a36cea4be84ffefc07a2bae45219
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213006133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:776784c756ff94ee538d092f5f0fc3fc1d9d00566ee457627d381a49ca08c0c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:38:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:39:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 15:39:00 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 15:53:08 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 15:53:09 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 15:53:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 15:56:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:56:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:56:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:56:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:56:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:56:29 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:13:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:14:41 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:14:42 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:14:42 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:14:44 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:14:45 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 00:14:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 00:14:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 00:16:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 00:16:17 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 00:16:18 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 00:16:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 00:16:18 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 00:16:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d04ca5200ad3b98494cfde36960022dbd29c9afc33d685ac499fae8a05d63`  
		Last Modified: Thu, 22 Jul 2021 16:06:57 GMT  
		Size: 17.2 MB (17227285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d9d06c9e919afbd9358b702cad5bc0f28b8150722ffedb25ece16dc1f19b2`  
		Last Modified: Thu, 22 Jul 2021 16:06:48 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3172650cf56a46da1b8438a86468d4053edf77c17eaad06d10b7c7a4f89d13ff`  
		Last Modified: Thu, 22 Jul 2021 16:09:12 GMT  
		Size: 20.9 MB (20910118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686761ac4b88297af44e82ba027c5c73411fe3e728b11bbdc631ea19cae4207`  
		Last Modified: Thu, 22 Jul 2021 16:09:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd85881cfa469c977c54673a6f7a5069bd5524e91c3dcc68765e8c34126cabe2`  
		Last Modified: Fri, 23 Jul 2021 00:23:41 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceccbef720a55f3b84f4c45e8ebfdec613398d896ceb5e3e5eb289b29c9fc015`  
		Last Modified: Fri, 23 Jul 2021 00:24:18 GMT  
		Size: 95.7 MB (95703189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2780ce2bed1fed359a6ca6b2570df212412bf9869a7e43011fd9b1e2b174944`  
		Last Modified: Fri, 23 Jul 2021 00:23:39 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156819ab7d2b648146a7ca9ccee6d402b080b6d4f0d598d5844ff1dcd229e09`  
		Last Modified: Fri, 23 Jul 2021 00:23:38 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443e7b0b88457341dc4d307344c8daae4f9443080a388a17d7f8594216731fad`  
		Last Modified: Fri, 23 Jul 2021 00:23:41 GMT  
		Size: 2.7 MB (2747695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18766104464d025bd83baa3b2f7422510d67e7969c35a05c71990f5bb50269e`  
		Last Modified: Fri, 23 Jul 2021 00:23:57 GMT  
		Size: 48.6 MB (48616155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dde10ba37dd3ba1c71ba7593bdb3be9f87bb9df2510ec41f832f63e3bd8065`  
		Last Modified: Fri, 23 Jul 2021 00:23:38 GMT  
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
$ docker pull redmine@sha256:c1c3473d2e887bdda0ea9be84088a3c1ce628dc37cdbc227a6d0231d09f55c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216897999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861436ac7fbd4f0e3f580f06a327e8e274dc07c164f45cb6eed2fae48b074874`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:03:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:03:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:03:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:38:29 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 14:38:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 14:38:31 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 14:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:42:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:42:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:42:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:42:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:42:37 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 02:10:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 02:11:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:11:22 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 02:11:23 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 02:11:23 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 02:11:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 02:11:24 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 02:11:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 02:11:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 02:13:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 02:13:22 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 02:13:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 02:13:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:13:23 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 02:13:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d658cd93dd34abb2452544d10308c796ec6310f6d1ca2d2762c8e85402e3e`  
		Last Modified: Thu, 22 Jul 2021 14:48:41 GMT  
		Size: 10.8 MB (10814518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bebc1f15c6904197539abc99a69885fa65493d7fae9f27d2529be2fa05491e`  
		Last Modified: Thu, 22 Jul 2021 14:48:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f561c255d99a491c5b43abff939ba38e74ae544c4075fb8c14e7c01f0a932d`  
		Last Modified: Thu, 22 Jul 2021 14:50:04 GMT  
		Size: 21.6 MB (21620156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556bb48ca77fd1659ce0e0ef9979115f34bd73b84af8bdc963902aa6ee99b83d`  
		Last Modified: Thu, 22 Jul 2021 14:50:02 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eb91b4d29f39917d9f1202634b78d331a8353110334caeaaf943d784e262`  
		Last Modified: Fri, 23 Jul 2021 02:17:45 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ac7d182c9da98ae82c5d32d13a6b4f232f1879de0b45139fccc48fa24f9e0`  
		Last Modified: Fri, 23 Jul 2021 02:17:58 GMT  
		Size: 91.8 MB (91790979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7104972ffbab9d882836504ebc8cee4ecab3ba51688a1fd6aacacee23b570b98`  
		Last Modified: Fri, 23 Jul 2021 02:17:44 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9f10e253324628fca93c339a045a38f301f3270bde8a193a3e432ed326248f`  
		Last Modified: Fri, 23 Jul 2021 02:17:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b20fbb52d2d72923dcd2120b7555607a538f553718db56099ab18697972050c`  
		Last Modified: Fri, 23 Jul 2021 02:17:44 GMT  
		Size: 2.7 MB (2747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f62a0f717f48c967a594517c3e8defe7f51af5cd9dd36e9aa9a0b331e8dd49e`  
		Last Modified: Fri, 23 Jul 2021 02:17:50 GMT  
		Size: 64.2 MB (64159644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb665766fc848837037e31fc14e65ff6e17794c489e5672ba21ccf46c2b34c7`  
		Last Modified: Fri, 23 Jul 2021 02:17:44 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-alpine`

```console
$ docker pull redmine@sha256:ab4e088a86875b1b538344cd8bffecef2ae743209af62856f076991270196c4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull redmine@sha256:9e91d95281f9ff0fb683f71fd65ba73bf88fde088b9aef777ba1b1e628d5090c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:c499bd79bf270637e1b6f6ed279ce13089b93898edf72e944aea444772eb7c30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232889481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69116a0dfe69db4103b1958e640ed39fd178571467c6883ffdf3248425f71fbe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 17:31:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 17:34:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:34:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:34:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:34:07 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:05:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:05:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:05:50 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:05:50 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:05:50 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:05:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:05:51 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 11:05:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 11:05:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:06:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:06:34 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:06:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:06:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:06:35 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:06:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 23 Jul 2021 11:06:49 GMT
ENV PASSENGER_VERSION=6.0.10
# Fri, 23 Jul 2021 11:07:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:07:06 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 23 Jul 2021 11:07:06 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 23 Jul 2021 11:07:07 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b7373cf9d9195064da3c92860c7157644c595720fffd5bb48615ac96985d5`  
		Last Modified: Thu, 22 Jul 2021 17:43:38 GMT  
		Size: 21.5 MB (21468044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb83e25b0fb68c5c98194adb0ad3740bc7d2242801c213e7d7949281f901679`  
		Last Modified: Thu, 22 Jul 2021 17:43:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61371aadcf232eb667c47dbba436a5611088d97ba4c8a9bd0c271f36882b027d`  
		Last Modified: Fri, 23 Jul 2021 11:11:30 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfd1dde1f32f7f8409959b4663cf89b722a2f427f544c5acf3c4dca5ba89961`  
		Last Modified: Fri, 23 Jul 2021 11:11:43 GMT  
		Size: 94.1 MB (94088300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216270a0114d5886d784b5a4bd95e0270c48d34e26e20ced7ee30251aecc0235`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc0835bd828414f95e3e7358066f88a9b754de0e89b47c431fd9eb5f61f4143`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7337fb63fe3caf0b547c29b505ceb48349b11dc5af872eea66c9b09e2da465`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 2.7 MB (2747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2c810419b90595f5b58de487a8545095e85d1f45da97616a70f30cfc579e86`  
		Last Modified: Fri, 23 Jul 2021 11:11:34 GMT  
		Size: 48.6 MB (48630706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7142a912af0cf678a75e06db24614b42621ba3c5594dd958d31308e8d90c361b`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca940f76f0f6a85724cc5803412f923ac7eb39d9d89d4d93b7d5159583b02af`  
		Last Modified: Fri, 23 Jul 2021 11:11:57 GMT  
		Size: 21.3 MB (21322642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08f83ae20505edb1de5a54246e3f767e2cb555ed3d0e98f4e17fa03f894183e`  
		Last Modified: Fri, 23 Jul 2021 11:11:55 GMT  
		Size: 4.9 MB (4919285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.3`

```console
$ docker pull redmine@sha256:c9f2b5e97a651b2aa2d4c58ff44bca86aefb51a49e4933d7caf7c0d1dfbbff83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.1.3` - linux; amd64

```console
$ docker pull redmine@sha256:698a793a34357b15ef34472cf146abcc2a011c240197e9a253eab953b3c06708
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.6 MB (206647554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0aa676a8efa66732addd34d54f03c6197d78ebf381246c24c101eac35a9549c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 17:31:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 17:34:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:34:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:34:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:34:07 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:05:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:05:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:05:50 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:05:50 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:05:50 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:05:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:05:51 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 11:05:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 11:05:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:06:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:06:34 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:06:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:06:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:06:35 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:06:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b7373cf9d9195064da3c92860c7157644c595720fffd5bb48615ac96985d5`  
		Last Modified: Thu, 22 Jul 2021 17:43:38 GMT  
		Size: 21.5 MB (21468044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb83e25b0fb68c5c98194adb0ad3740bc7d2242801c213e7d7949281f901679`  
		Last Modified: Thu, 22 Jul 2021 17:43:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61371aadcf232eb667c47dbba436a5611088d97ba4c8a9bd0c271f36882b027d`  
		Last Modified: Fri, 23 Jul 2021 11:11:30 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfd1dde1f32f7f8409959b4663cf89b722a2f427f544c5acf3c4dca5ba89961`  
		Last Modified: Fri, 23 Jul 2021 11:11:43 GMT  
		Size: 94.1 MB (94088300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216270a0114d5886d784b5a4bd95e0270c48d34e26e20ced7ee30251aecc0235`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc0835bd828414f95e3e7358066f88a9b754de0e89b47c431fd9eb5f61f4143`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7337fb63fe3caf0b547c29b505ceb48349b11dc5af872eea66c9b09e2da465`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 2.7 MB (2747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2c810419b90595f5b58de487a8545095e85d1f45da97616a70f30cfc579e86`  
		Last Modified: Fri, 23 Jul 2021 11:11:34 GMT  
		Size: 48.6 MB (48630706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7142a912af0cf678a75e06db24614b42621ba3c5594dd958d31308e8d90c361b`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; arm variant v5

```console
$ docker pull redmine@sha256:d3047b6a3f20c53967162e58629dbf5f9bf7d7df656711a4e1d2344c4d2362b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210649914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:906f660eed56fe2f80404754940f80004e24f07fe1aa72b879f072de8414781d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:39:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 14:57:30 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 15:01:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:02:00 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:02:01 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:02:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:02:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:02:04 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:32:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:33:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:33:37 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:33:37 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:33:38 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:33:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:33:40 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 01:33:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 01:33:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:39:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:39:28 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:39:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:39:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:39:30 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:39:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9237058b7c5120d5c6315b5d17a8c1d783be09a228b83772111ce9436c29d078`  
		Last Modified: Thu, 22 Jul 2021 15:15:34 GMT  
		Size: 10.3 MB (10345807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144b4344f580222d2fbc2f0d80fc139ab1a1ddb9a245b6073c41fdca9a93c23e`  
		Last Modified: Thu, 22 Jul 2021 15:15:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae149ea188f1e064a0256560e0273ae4b331a42ab93326fd9a79753cfb63299d`  
		Last Modified: Thu, 22 Jul 2021 15:18:00 GMT  
		Size: 20.7 MB (20733368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5d2d97d7d53265f79bb7d6b5cfc05f237e3d237d9cf22475536aa4fd57ccde`  
		Last Modified: Thu, 22 Jul 2021 15:17:55 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822c77937c7bc9bc3d506cf3a12ef2ada0bdbc4c0db3af2efaecc31c4191df4a`  
		Last Modified: Fri, 23 Jul 2021 01:49:24 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c50724a36d3c9a8b9ceae430de242d7f6969dbef3ac25c5fde473a8b062cd3`  
		Last Modified: Fri, 23 Jul 2021 01:50:25 GMT  
		Size: 89.6 MB (89576586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64ad6c53bf00acadba6df300f7a60ca8ae5ddc2336b37cd556bbcc18d26566c`  
		Last Modified: Fri, 23 Jul 2021 01:49:22 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f057554e99e7143804c2bfa6e4ad7c04cbf19075e611550a34de736734ec41c3`  
		Last Modified: Fri, 23 Jul 2021 01:49:22 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890a1a9f8beba551d854feae5c278566e6556b2bb755a4518aa8e17b21a184b8`  
		Last Modified: Fri, 23 Jul 2021 01:49:25 GMT  
		Size: 2.7 MB (2747690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f512938291c851f1276e8ffe92f72cf4a2d4ad57b115945b68d2df77c79bcf`  
		Last Modified: Fri, 23 Jul 2021 01:49:50 GMT  
		Size: 62.4 MB (62363137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e581faafeae657c0d1e349678afd589d102215ba5a2ef10d020cf819e943ff68`  
		Last Modified: Fri, 23 Jul 2021 01:49:22 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; arm variant v7

```console
$ docker pull redmine@sha256:6eebe2e3817e16be90e0203273f1d110ebb3b628d469036fcb1f67560b13c360
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203830389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b70a3855d41ad008f02e50f66b192b32951aaae36adaa23649329aa2636dfad`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:15:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 02:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 02:46:35 GMT
ENV RUBY_MAJOR=2.6
# Fri, 23 Jul 2021 02:46:35 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 23 Jul 2021 02:46:36 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 23 Jul 2021 02:50:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 02:50:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 02:50:40 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 02:50:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:50:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 02:50:43 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 21:25:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 21:26:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 21:26:28 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 21:26:29 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 21:26:29 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 21:26:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 21:26:32 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 21:26:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 21:26:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 21:31:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 21:31:57 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 21:31:57 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 21:31:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 21:31:58 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 21:31:58 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b8c791d70de7f22816846fbb07e0a1d7d419841c7e539a7cf57ef05fd50c5`  
		Last Modified: Fri, 23 Jul 2021 03:05:10 GMT  
		Size: 9.9 MB (9872218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12a7edb0af862efa24dc389d7901cd2a894f2e106a1cef931ba0a6d675e2c0`  
		Last Modified: Fri, 23 Jul 2021 03:05:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0837e4e34dc8fe0ec9567b99bb7b1397a813fca3b43abfbbd75ee231a946a979`  
		Last Modified: Fri, 23 Jul 2021 03:07:54 GMT  
		Size: 20.6 MB (20643760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c76309d8689f06c398ddc0f6b5ec99a408c65c613d73d63fb9f5101ebe3e2a1`  
		Last Modified: Fri, 23 Jul 2021 03:07:49 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c349a607ae692434577c905a1f4029d996cee89a0c9f214fa866ac935ceddf23`  
		Last Modified: Fri, 23 Jul 2021 21:41:16 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2880a64f27ab57a09b4f72db20fc36a50bf3b6a6f3475f8661e8184e4b8acb99`  
		Last Modified: Fri, 23 Jul 2021 21:42:11 GMT  
		Size: 85.6 MB (85590430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455a681e485f6469d2ea0559f66edfbdf6ea359e79d4a5db42bf76287a0de434`  
		Last Modified: Fri, 23 Jul 2021 21:41:15 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ac534a0a817b7f2f9c1f1e31c139ea1f9375a72e0f485b0383bc4fc4d59fd2a`  
		Last Modified: Fri, 23 Jul 2021 21:41:14 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c259d05afcbc2a0eb12900c825ff56dcc70e11e07fdb65c78eab33160c0e5101`  
		Last Modified: Fri, 23 Jul 2021 21:41:18 GMT  
		Size: 2.7 MB (2747686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709e390734515835b5ca9e0fef442f6c0d52edad99d53438eabe4f69ee5ecf1f`  
		Last Modified: Fri, 23 Jul 2021 21:41:43 GMT  
		Size: 62.2 MB (62226086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bb46285ccbd31e69fc92ab1250e30fdd2d5555b1673e408f871e9f9e5c5882`  
		Last Modified: Fri, 23 Jul 2021 21:41:14 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:5cc5f6edf0217b06b83a6d9daf43c2595773bcbcef895bcfb558f310e8e31091
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217532817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8db0a234953326e03a8a215dd562aa68f5ade3010aa21e045a241631da99b8e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 12:36:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 12:45:29 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 12:45:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 12:45:30 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 12:47:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 12:47:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 12:47:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 12:47:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 12:47:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 12:47:36 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:00:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:01:14 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:01:15 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:01:15 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:01:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:01:16 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 01:01:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 01:01:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:03:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:03:25 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:03:25 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:03:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:03:26 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:03:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a77364b6ec6cfc9422903e0f9d3f5cab5ee0ac4b62cfac6fc7c3d544ad7f57`  
		Last Modified: Thu, 22 Jul 2021 12:55:11 GMT  
		Size: 11.3 MB (11263053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a68321ef048d82e4480bc2de1681a811f18b2e1d04b5aa9dec38030570eaa40`  
		Last Modified: Thu, 22 Jul 2021 12:55:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6319f6f39ac757356a2f054631df2eaa6a111934c0e9128d04df9f2296eef143`  
		Last Modified: Thu, 22 Jul 2021 12:57:16 GMT  
		Size: 21.3 MB (21308954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3246f58f273186efdfacba513b296257ca20afe8e09b07635bf20c90f80cc2eb`  
		Last Modified: Thu, 22 Jul 2021 12:57:14 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc11d0bb585455c7f2d643b57d83d2bc79e83d4fa6102af98583c50395fdd42c`  
		Last Modified: Fri, 23 Jul 2021 01:07:19 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c1e2df6c95b23a8889c0654161e692541689cbcffaec4d8da108ae9c92bf22`  
		Last Modified: Fri, 23 Jul 2021 01:07:34 GMT  
		Size: 92.6 MB (92611084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c484a1eebcc4d4b1196c27f7f75a74073d9698f5f68a0b86039801f5dbdebf`  
		Last Modified: Fri, 23 Jul 2021 01:07:16 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc0b0c15a3bb1ec46ee2421b14a404f1d32163bd66d9aa39c4bd340e4d66136`  
		Last Modified: Fri, 23 Jul 2021 01:07:16 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0564dafa91638f855756581e6ca8ec66c1b11882217effc7b7b8106960fbd754`  
		Last Modified: Fri, 23 Jul 2021 01:07:17 GMT  
		Size: 2.7 MB (2747697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99c9dcd637a9c0101748c513c5f58b49ab12f28e39f3910882bcb2c163d6dff`  
		Last Modified: Fri, 23 Jul 2021 01:07:24 GMT  
		Size: 63.7 MB (63682990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6789464e18852a4489c02f3bd68b8e06398cdb0d633f0e232899c4cdc9be1054`  
		Last Modified: Fri, 23 Jul 2021 01:07:16 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.3` - linux; 386

```console
$ docker pull redmine@sha256:1eba46b22559e6801bb7c7084ac6ce0da373a36cea4be84ffefc07a2bae45219
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213006133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:776784c756ff94ee538d092f5f0fc3fc1d9d00566ee457627d381a49ca08c0c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:38:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:39:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 15:39:00 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 15:53:08 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 15:53:09 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 15:53:09 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 15:56:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:56:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:56:27 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:56:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:56:28 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:56:29 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:13:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:14:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:14:41 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:14:42 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:14:42 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:14:44 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:14:45 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 00:14:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 00:14:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 00:16:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 00:16:17 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 00:16:18 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 00:16:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 00:16:18 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 00:16:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d04ca5200ad3b98494cfde36960022dbd29c9afc33d685ac499fae8a05d63`  
		Last Modified: Thu, 22 Jul 2021 16:06:57 GMT  
		Size: 17.2 MB (17227285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d9d06c9e919afbd9358b702cad5bc0f28b8150722ffedb25ece16dc1f19b2`  
		Last Modified: Thu, 22 Jul 2021 16:06:48 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3172650cf56a46da1b8438a86468d4053edf77c17eaad06d10b7c7a4f89d13ff`  
		Last Modified: Thu, 22 Jul 2021 16:09:12 GMT  
		Size: 20.9 MB (20910118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2686761ac4b88297af44e82ba027c5c73411fe3e728b11bbdc631ea19cae4207`  
		Last Modified: Thu, 22 Jul 2021 16:09:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd85881cfa469c977c54673a6f7a5069bd5524e91c3dcc68765e8c34126cabe2`  
		Last Modified: Fri, 23 Jul 2021 00:23:41 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceccbef720a55f3b84f4c45e8ebfdec613398d896ceb5e3e5eb289b29c9fc015`  
		Last Modified: Fri, 23 Jul 2021 00:24:18 GMT  
		Size: 95.7 MB (95703189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2780ce2bed1fed359a6ca6b2570df212412bf9869a7e43011fd9b1e2b174944`  
		Last Modified: Fri, 23 Jul 2021 00:23:39 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f156819ab7d2b648146a7ca9ccee6d402b080b6d4f0d598d5844ff1dcd229e09`  
		Last Modified: Fri, 23 Jul 2021 00:23:38 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:443e7b0b88457341dc4d307344c8daae4f9443080a388a17d7f8594216731fad`  
		Last Modified: Fri, 23 Jul 2021 00:23:41 GMT  
		Size: 2.7 MB (2747695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18766104464d025bd83baa3b2f7422510d67e7969c35a05c71990f5bb50269e`  
		Last Modified: Fri, 23 Jul 2021 00:23:57 GMT  
		Size: 48.6 MB (48616155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dde10ba37dd3ba1c71ba7593bdb3be9f87bb9df2510ec41f832f63e3bd8065`  
		Last Modified: Fri, 23 Jul 2021 00:23:38 GMT  
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
$ docker pull redmine@sha256:c1c3473d2e887bdda0ea9be84088a3c1ce628dc37cdbc227a6d0231d09f55c3f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216897999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:861436ac7fbd4f0e3f580f06a327e8e274dc07c164f45cb6eed2fae48b074874`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:03:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:03:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:03:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:38:29 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 14:38:30 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 14:38:31 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 14:42:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:42:33 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:42:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:42:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:42:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:42:37 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 02:10:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 02:11:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:11:22 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 02:11:23 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 02:11:23 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 02:11:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 02:11:24 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 02:11:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 02:11:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 02:13:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 02:13:22 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 02:13:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 02:13:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:13:23 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 02:13:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d658cd93dd34abb2452544d10308c796ec6310f6d1ca2d2762c8e85402e3e`  
		Last Modified: Thu, 22 Jul 2021 14:48:41 GMT  
		Size: 10.8 MB (10814518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bebc1f15c6904197539abc99a69885fa65493d7fae9f27d2529be2fa05491e`  
		Last Modified: Thu, 22 Jul 2021 14:48:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58f561c255d99a491c5b43abff939ba38e74ae544c4075fb8c14e7c01f0a932d`  
		Last Modified: Thu, 22 Jul 2021 14:50:04 GMT  
		Size: 21.6 MB (21620156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556bb48ca77fd1659ce0e0ef9979115f34bd73b84af8bdc963902aa6ee99b83d`  
		Last Modified: Thu, 22 Jul 2021 14:50:02 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7eb91b4d29f39917d9f1202634b78d331a8353110334caeaaf943d784e262`  
		Last Modified: Fri, 23 Jul 2021 02:17:45 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ac7d182c9da98ae82c5d32d13a6b4f232f1879de0b45139fccc48fa24f9e0`  
		Last Modified: Fri, 23 Jul 2021 02:17:58 GMT  
		Size: 91.8 MB (91790979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7104972ffbab9d882836504ebc8cee4ecab3ba51688a1fd6aacacee23b570b98`  
		Last Modified: Fri, 23 Jul 2021 02:17:44 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9f10e253324628fca93c339a045a38f301f3270bde8a193a3e432ed326248f`  
		Last Modified: Fri, 23 Jul 2021 02:17:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b20fbb52d2d72923dcd2120b7555607a538f553718db56099ab18697972050c`  
		Last Modified: Fri, 23 Jul 2021 02:17:44 GMT  
		Size: 2.7 MB (2747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f62a0f717f48c967a594517c3e8defe7f51af5cd9dd36e9aa9a0b331e8dd49e`  
		Last Modified: Fri, 23 Jul 2021 02:17:50 GMT  
		Size: 64.2 MB (64159644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb665766fc848837037e31fc14e65ff6e17794c489e5672ba21ccf46c2b34c7`  
		Last Modified: Fri, 23 Jul 2021 02:17:44 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.3-alpine`

```console
$ docker pull redmine@sha256:ab4e088a86875b1b538344cd8bffecef2ae743209af62856f076991270196c4f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull redmine@sha256:9e91d95281f9ff0fb683f71fd65ba73bf88fde088b9aef777ba1b1e628d5090c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1.3-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:c499bd79bf270637e1b6f6ed279ce13089b93898edf72e944aea444772eb7c30
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232889481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69116a0dfe69db4103b1958e640ed39fd178571467c6883ffdf3248425f71fbe`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_MAJOR=2.6
# Thu, 22 Jul 2021 17:31:24 GMT
ENV RUBY_VERSION=2.6.8
# Thu, 22 Jul 2021 17:31:25 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Thu, 22 Jul 2021 17:34:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:34:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:34:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:34:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:34:07 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:05:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:05:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:05:50 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:05:50 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:05:50 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:05:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:05:51 GMT
ENV REDMINE_VERSION=4.1.3
# Fri, 23 Jul 2021 11:05:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=b5a11a750fa7eeafdf513b352fa2375987b6ebad4264a929ad4db0421870c154
# Fri, 23 Jul 2021 11:05:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:06:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:06:34 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:06:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:06:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:06:35 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:06:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 23 Jul 2021 11:06:49 GMT
ENV PASSENGER_VERSION=6.0.10
# Fri, 23 Jul 2021 11:07:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:07:06 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 23 Jul 2021 11:07:06 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 23 Jul 2021 11:07:07 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b7373cf9d9195064da3c92860c7157644c595720fffd5bb48615ac96985d5`  
		Last Modified: Thu, 22 Jul 2021 17:43:38 GMT  
		Size: 21.5 MB (21468044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb83e25b0fb68c5c98194adb0ad3740bc7d2242801c213e7d7949281f901679`  
		Last Modified: Thu, 22 Jul 2021 17:43:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61371aadcf232eb667c47dbba436a5611088d97ba4c8a9bd0c271f36882b027d`  
		Last Modified: Fri, 23 Jul 2021 11:11:30 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dfd1dde1f32f7f8409959b4663cf89b722a2f427f544c5acf3c4dca5ba89961`  
		Last Modified: Fri, 23 Jul 2021 11:11:43 GMT  
		Size: 94.1 MB (94088300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216270a0114d5886d784b5a4bd95e0270c48d34e26e20ced7ee30251aecc0235`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc0835bd828414f95e3e7358066f88a9b754de0e89b47c431fd9eb5f61f4143`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb7337fb63fe3caf0b547c29b505ceb48349b11dc5af872eea66c9b09e2da465`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 2.7 MB (2747691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2c810419b90595f5b58de487a8545095e85d1f45da97616a70f30cfc579e86`  
		Last Modified: Fri, 23 Jul 2021 11:11:34 GMT  
		Size: 48.6 MB (48630706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7142a912af0cf678a75e06db24614b42621ba3c5594dd958d31308e8d90c361b`  
		Last Modified: Fri, 23 Jul 2021 11:11:27 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca940f76f0f6a85724cc5803412f923ac7eb39d9d89d4d93b7d5159583b02af`  
		Last Modified: Fri, 23 Jul 2021 11:11:57 GMT  
		Size: 21.3 MB (21322642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08f83ae20505edb1de5a54246e3f767e2cb555ed3d0e98f4e17fa03f894183e`  
		Last Modified: Fri, 23 Jul 2021 11:11:55 GMT  
		Size: 4.9 MB (4919285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2`

```console
$ docker pull redmine@sha256:95435c3e6e2d0815459d7c44520b2743dbb8806cba32184ba0bfdf143d5af0b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.2` - linux; amd64

```console
$ docker pull redmine@sha256:e28ea2b1f675569c4763cf0cd04ff101d384a263d952858b8e7533b7f335f34a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195475927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be97e87738155b1d102c2b0b7286bd39b06e62a5a8184e8fb0e21b7a2e819743`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 17:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:28:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:28:25 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:03:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:04:03 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:04:03 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:04:03 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:04:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 11:04:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:04:49 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:04:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:49 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:04:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e582c090726ff249b7e30253c7f0c11aa2cd14282a8b6cd0e8055c8615e5586`  
		Last Modified: Thu, 22 Jul 2021 17:42:40 GMT  
		Size: 14.5 MB (14509812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f96a83aedee46aef2be1d4f73cc6990dc7e756981b022462100ac16fad345`  
		Last Modified: Thu, 22 Jul 2021 17:42:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9466f2ac94d013cc74523ee4ad44d9720c72baa51d8aecc2afcba41c3754be44`  
		Last Modified: Fri, 23 Jul 2021 11:10:32 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbad6372ccefa1ce14b5eefe2fe718c0cd234b40bf9a70e3d02e131a9dd65d26`  
		Last Modified: Fri, 23 Jul 2021 11:10:45 GMT  
		Size: 94.1 MB (94087869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93724991108aa18238773a3122f3fcd80f69331610c0a7f00656f690ac7692`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19466676666dc7f1a145b5b2534855e6f32c152cd3da118bc5536badc24da33d`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc48a22ec231d5048d556cd637291655083a29acb695b0073039d36315929da`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 3.1 MB (3058677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00b1336ee6986b3f2923502d082ce45ebccea58e21f85ddd12812be6796e1f`  
		Last Modified: Fri, 23 Jul 2021 11:10:33 GMT  
		Size: 44.1 MB (44106755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fe342d55cb9155ec0d7a14a371258946d43b0b4e3df44e3f1bbe9b166a5ef`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v5

```console
$ docker pull redmine@sha256:9ef48dcd233199a54171d5bf678c6fc5245453cdd9827c68ce9b91796501de9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196974351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25105893bd633c389af7ab7f4e947fa0ff2172ac3cd182d70b9bc2d2a45607e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:39:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:48:33 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 14:48:33 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 14:48:34 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 14:52:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:52:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:52:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:52:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:52:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:52:55 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:25:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:26:16 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:26:17 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:26:17 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:26:18 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:26:19 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 01:26:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 01:26:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:32:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:32:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:32:10 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:32:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:32:11 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:32:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9237058b7c5120d5c6315b5d17a8c1d783be09a228b83772111ce9436c29d078`  
		Last Modified: Thu, 22 Jul 2021 15:15:34 GMT  
		Size: 10.3 MB (10345807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144b4344f580222d2fbc2f0d80fc139ab1a1ddb9a245b6073c41fdca9a93c23e`  
		Last Modified: Thu, 22 Jul 2021 15:15:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8ddbd20410764a5a44de2520de7417bddfcc0fdf2f4fa1b1d4e9ac785ce253`  
		Last Modified: Thu, 22 Jul 2021 15:17:00 GMT  
		Size: 13.9 MB (13871315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1fe10899466e387c0fc9cc130a0a900ffeb91af92c09301e387e444836d74f`  
		Last Modified: Thu, 22 Jul 2021 15:16:52 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b419523e1af1c8a3f9891c74f5e29e5697be8bf7bf57f23880ac551c460f07`  
		Last Modified: Fri, 23 Jul 2021 01:48:00 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d44a2001e78eed6fc3a85dbe0059a0bfae376949cda406c9304941ed617a23`  
		Last Modified: Fri, 23 Jul 2021 01:49:01 GMT  
		Size: 89.6 MB (89576912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2901c80e9a45cf66afe7fb2306719b195ec9c983783f4058ef68246bb10b95`  
		Last Modified: Fri, 23 Jul 2021 01:47:58 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0cf9a21c70c0994e217daf5f71efd9d2f8ce8f36e062be7c831492162e99a`  
		Last Modified: Fri, 23 Jul 2021 01:47:57 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5daae06ca7c40f7fa2e94d4be701850020a63374c01cb310471f056eda7498`  
		Last Modified: Fri, 23 Jul 2021 01:48:01 GMT  
		Size: 3.1 MB (3058682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d9118a275db8a49fd1b15511383b91ac8b867604e68e255d097c4a7880a8ff`  
		Last Modified: Fri, 23 Jul 2021 01:48:21 GMT  
		Size: 55.2 MB (55238308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d94f744aa1ad4af6e0d39600d4e4bf9e68e942510443afa0d8ecf37e30835`  
		Last Modified: Fri, 23 Jul 2021 01:47:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:3aca8dadb5407c0d388ac5baf1a99dbeeabc4fe3da1c506883b1c394c7fe7610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9074a5390b69761aca8dcac7078799a4f869792b8311bc2280916419daa31aca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:15:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 02:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 02:25:03 GMT
ENV RUBY_MAJOR=2.7
# Fri, 23 Jul 2021 02:25:04 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 23 Jul 2021 02:25:04 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 23 Jul 2021 02:29:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 02:29:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 02:29:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 02:29:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:29:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 02:29:10 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 21:18:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 21:19:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 21:19:37 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 21:19:37 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 21:19:38 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 21:19:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 21:19:40 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 21:19:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 21:19:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 21:25:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 21:25:05 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 21:25:06 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 21:25:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 21:25:06 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 21:25:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b8c791d70de7f22816846fbb07e0a1d7d419841c7e539a7cf57ef05fd50c5`  
		Last Modified: Fri, 23 Jul 2021 03:05:10 GMT  
		Size: 9.9 MB (9872218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12a7edb0af862efa24dc389d7901cd2a894f2e106a1cef931ba0a6d675e2c0`  
		Last Modified: Fri, 23 Jul 2021 03:05:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b75d257bf75804e51385b730af2aaba386a501ef50517b8379966d4372c8597`  
		Last Modified: Fri, 23 Jul 2021 03:06:48 GMT  
		Size: 13.8 MB (13766962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc7c7e0536ed6ba4a99c1b8960d7c1d7365c8bc52d230b8af44d07d085916f`  
		Last Modified: Fri, 23 Jul 2021 03:06:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9cbdbb67af5c0b986c2fd6f93a2bacf3c795b046bfdf19e8f483dbc780c643`  
		Last Modified: Fri, 23 Jul 2021 21:39:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823bb8e3702405c250a7cc3dadba844fef162cbd0f5b9fb70a107f618dffeddf`  
		Last Modified: Fri, 23 Jul 2021 21:40:51 GMT  
		Size: 85.6 MB (85590187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930c9cc4f262f629914e37abf7b88697bc949d34260a237f8d740ea30ddf5902`  
		Last Modified: Fri, 23 Jul 2021 21:39:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e7aa3a63516ee59c6e77fd1a74b1ce0b303c09b2a97dd0ca3b0af594021030`  
		Last Modified: Fri, 23 Jul 2021 21:39:55 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b8cbe774bbfa06d5d0e463126138a655e455605ce81a4b4799b6495959723`  
		Last Modified: Fri, 23 Jul 2021 21:39:58 GMT  
		Size: 3.1 MB (3058685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231b30773994af4c612b2b73b0a33eef728b235396a59b1c34d64b17c2289dd`  
		Last Modified: Fri, 23 Jul 2021 21:40:19 GMT  
		Size: 55.1 MB (55076883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af42513ad3b3f3a0291481c9f4b6a077a9e62fc8cd14736897d28d5f70687618`  
		Last Modified: Fri, 23 Jul 2021 21:39:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:b7a96326ffb8fc77358a78fac0448fd3c56dd2fb1feb29dd3528e6cac29cd155
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203231883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e4b31ef3849045f66d5846fad154cbaf41e73cd54c0a5afcf7bed7817d16a5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 12:36:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 12:41:08 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 12:41:08 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 12:41:09 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 12:43:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 12:43:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 12:43:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 12:43:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 12:43:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 12:43:05 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:57:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:58:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:58:04 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:58:04 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:58:04 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:58:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:58:05 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 00:58:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 00:58:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:00:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:00:36 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:00:36 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:00:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:00:36 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:00:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a77364b6ec6cfc9422903e0f9d3f5cab5ee0ac4b62cfac6fc7c3d544ad7f57`  
		Last Modified: Thu, 22 Jul 2021 12:55:11 GMT  
		Size: 11.3 MB (11263053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a68321ef048d82e4480bc2de1681a811f18b2e1d04b5aa9dec38030570eaa40`  
		Last Modified: Thu, 22 Jul 2021 12:55:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ec69cd14df7f6066799b20f9268ae3ce6e5e0564c2b560a10804765f4c7cf`  
		Last Modified: Thu, 22 Jul 2021 12:56:22 GMT  
		Size: 14.4 MB (14356675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4a2f06c1cec263f641737334f76372caff218cb8312bc8375c4e69c7289147`  
		Last Modified: Thu, 22 Jul 2021 12:56:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02fa466075ed10ab6e904b032ad10baf66dce45f41bb930b1ea5728647d32c`  
		Last Modified: Fri, 23 Jul 2021 01:06:41 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde3ab2a527d4e47aafb6f9cf0128ee08d754d6bed600addccaa4309e29f6437`  
		Last Modified: Fri, 23 Jul 2021 01:06:56 GMT  
		Size: 92.6 MB (92610625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f378e820ad759f627889603226956c607d864e95e967c969aa7965d93fb45816`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8291e2aab5ca9a9c51cc69c4cab741f3d46369744adec4f04f120329ed36f48d`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314b7425fd6ac642e912d76f7f9dafe5eda902a1abd7ab0ad23662da1bb75d73`  
		Last Modified: Fri, 23 Jul 2021 01:06:39 GMT  
		Size: 3.1 MB (3058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9b783db9ec2f80081bb3fc6226424e234ca9e33e9da8e7e6784a9e8b2a4b9f`  
		Last Modified: Fri, 23 Jul 2021 01:06:44 GMT  
		Size: 56.0 MB (56023809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f20fa5c3f8387a262408432f792b73cb61c7957e5c6ba4edd46d4da28d05a6c`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; 386

```console
$ docker pull redmine@sha256:e0c39c52abc9d57cf5bd97523c15db6fe60284390d12d89bd95e1d8ff7ea69dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202117810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6402098c31c9ce288516e50c34618b6cdce5229aaefc10ad583c89f4e4144289`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:38:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:39:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 15:39:00 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 15:49:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:49:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:49:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:49:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:49:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:49:39 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:10:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:11:45 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:11:45 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:11:46 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:11:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:11:48 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 00:11:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 00:11:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 00:13:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 00:13:26 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 00:13:26 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 00:13:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 00:13:27 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 00:13:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d04ca5200ad3b98494cfde36960022dbd29c9afc33d685ac499fae8a05d63`  
		Last Modified: Thu, 22 Jul 2021 16:06:57 GMT  
		Size: 17.2 MB (17227285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d9d06c9e919afbd9358b702cad5bc0f28b8150722ffedb25ece16dc1f19b2`  
		Last Modified: Thu, 22 Jul 2021 16:06:48 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9e06bdf88f28c2f5d5893c862c6da8a6a73eb098cb2cd8eec57656d9a79b69`  
		Last Modified: Thu, 22 Jul 2021 16:08:14 GMT  
		Size: 14.0 MB (13992268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4f84633b2fe0d1dff5a1fd6ab3a5506af8978d94ded4f5a0f2727ce06805d4`  
		Last Modified: Thu, 22 Jul 2021 16:08:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57ef59b51318d382563cb5fdab4577df04d06c56bd8885926c9a9374a31ed7c`  
		Last Modified: Fri, 23 Jul 2021 00:22:32 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2922ffac0f77cf1fd832a20d48b586a6621e1d75610c055227f6d76e34928b16`  
		Last Modified: Fri, 23 Jul 2021 00:23:09 GMT  
		Size: 95.7 MB (95703233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb8c5967872202784509fa53a811f849c714ef794dd53a40047d0c81585ce4`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c1ffe6294aae5e8df812aee47c20e59fe0f4ec3593946e4ed069116ebb9f1`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f26aa32bafd59c6d9237ded27dc8ab964a91915e3b9a678b76d587899376ec`  
		Last Modified: Fri, 23 Jul 2021 00:22:31 GMT  
		Size: 3.1 MB (3058690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba425f932ee35d618a7e2a024cf68062985ba8dbbedbfd829e6af8cb1d1978b6`  
		Last Modified: Fri, 23 Jul 2021 00:22:45 GMT  
		Size: 44.3 MB (44334640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bca1f4ee34a1ccde3aac51ad07cafbaa3d857e77059427b1f928f48da6a0134`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 1.8 KB (1797 bytes)  
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
$ docker pull redmine@sha256:37201304a98b29096c65aff1082800685f8811d091fecfdbbfbc4b02ce56c712
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202549844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cceccec5920cb372b1e0e6536384018db9d2cf92a8ccf57721c5e55ec24b272`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:03:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:03:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:03:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:23:01 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 14:23:02 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 14:23:03 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 14:26:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:26:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:26:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:26:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:26:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:26:30 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 02:07:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:08:34 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 02:08:34 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 02:08:34 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 02:08:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 02:08:35 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 02:08:36 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 02:08:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 02:10:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 02:10:31 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 02:10:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 02:10:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:10:32 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 02:10:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d658cd93dd34abb2452544d10308c796ec6310f6d1ca2d2762c8e85402e3e`  
		Last Modified: Thu, 22 Jul 2021 14:48:41 GMT  
		Size: 10.8 MB (10814518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bebc1f15c6904197539abc99a69885fa65493d7fae9f27d2529be2fa05491e`  
		Last Modified: Thu, 22 Jul 2021 14:48:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa61230ad4685d16dfcb4b68dd88f40b84ddf598a2031852e9881218e137c19a`  
		Last Modified: Thu, 22 Jul 2021 14:49:27 GMT  
		Size: 14.7 MB (14697201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f9ff30668a8bd8fd8341049bbebd3d1db4e433d0116f70111daa596abf7e7a`  
		Last Modified: Thu, 22 Jul 2021 14:49:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91522d35fa6424129e9d5eb39ac436e70fd9e80337413131aa3401b1496857ff`  
		Last Modified: Fri, 23 Jul 2021 02:17:18 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5900d840b86d971e896fc6c7451e9a176bd80fa994f5090d5dbcf5ef6e48b14`  
		Last Modified: Fri, 23 Jul 2021 02:17:31 GMT  
		Size: 91.8 MB (91790782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede4b68f2bb6676b42e076513a0c075e3da52f75acb4070789e5d12196646541`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add04b7bc101933c98b8043337844f9e18f272fd13d47b87100f4fd9f52710b2`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51111bc126246f79519ed7c546b73f24285cc97694e205b48267a20ba50637f2`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 3.1 MB (3058684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad5d1e67f7c62f6d33343a9632c4aca3d5c808a4a4a18a476fcad4acf39bdb`  
		Last Modified: Fri, 23 Jul 2021 02:17:26 GMT  
		Size: 56.4 MB (56423655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c540e32ed87a6e82bdca054e93ee83775afa16fab29404772b98d2a047156a0c`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-alpine`

```console
$ docker pull redmine@sha256:7de4015773da4d105b5f43705556003eb3071d781612fa6e7f6010981e4e56e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull redmine@sha256:4198d395967db00ec073ed9d714c41b00472e77e49b0dcae51f259d9b78dbc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:43a77f34a70b4e12264df8bff7377b5ae47895166cfd156a903cb28b641fec29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0604330a8f415b11297aee811ea898c9a092e3255eb53a843e412e37469ba9d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 17:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:28:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:28:25 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:03:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:04:03 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:04:03 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:04:03 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:04:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 11:04:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:04:49 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:04:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:49 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:04:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 23 Jul 2021 11:04:59 GMT
ENV PASSENGER_VERSION=6.0.10
# Fri, 23 Jul 2021 11:05:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:05:16 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 23 Jul 2021 11:05:17 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 23 Jul 2021 11:05:17 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e582c090726ff249b7e30253c7f0c11aa2cd14282a8b6cd0e8055c8615e5586`  
		Last Modified: Thu, 22 Jul 2021 17:42:40 GMT  
		Size: 14.5 MB (14509812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f96a83aedee46aef2be1d4f73cc6990dc7e756981b022462100ac16fad345`  
		Last Modified: Thu, 22 Jul 2021 17:42:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9466f2ac94d013cc74523ee4ad44d9720c72baa51d8aecc2afcba41c3754be44`  
		Last Modified: Fri, 23 Jul 2021 11:10:32 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbad6372ccefa1ce14b5eefe2fe718c0cd234b40bf9a70e3d02e131a9dd65d26`  
		Last Modified: Fri, 23 Jul 2021 11:10:45 GMT  
		Size: 94.1 MB (94087869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93724991108aa18238773a3122f3fcd80f69331610c0a7f00656f690ac7692`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19466676666dc7f1a145b5b2534855e6f32c152cd3da118bc5536badc24da33d`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc48a22ec231d5048d556cd637291655083a29acb695b0073039d36315929da`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 3.1 MB (3058677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00b1336ee6986b3f2923502d082ce45ebccea58e21f85ddd12812be6796e1f`  
		Last Modified: Fri, 23 Jul 2021 11:10:33 GMT  
		Size: 44.1 MB (44106755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fe342d55cb9155ec0d7a14a371258946d43b0b4e3df44e3f1bbe9b166a5ef`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8e911f2db9cefa3945c1c8bbcc4e9dc79575560305045da7e987dfa48fa522`  
		Last Modified: Fri, 23 Jul 2021 11:11:07 GMT  
		Size: 21.1 MB (21131293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab210a34ab4fa48ee042162c1b27897332d05666f95bb001a39f2d04a7df605`  
		Last Modified: Fri, 23 Jul 2021 11:11:05 GMT  
		Size: 4.9 MB (4919283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.1`

```console
$ docker pull redmine@sha256:95435c3e6e2d0815459d7c44520b2743dbb8806cba32184ba0bfdf143d5af0b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.2.1` - linux; amd64

```console
$ docker pull redmine@sha256:e28ea2b1f675569c4763cf0cd04ff101d384a263d952858b8e7533b7f335f34a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195475927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be97e87738155b1d102c2b0b7286bd39b06e62a5a8184e8fb0e21b7a2e819743`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 17:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:28:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:28:25 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:03:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:04:03 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:04:03 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:04:03 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:04:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 11:04:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:04:49 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:04:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:49 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:04:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e582c090726ff249b7e30253c7f0c11aa2cd14282a8b6cd0e8055c8615e5586`  
		Last Modified: Thu, 22 Jul 2021 17:42:40 GMT  
		Size: 14.5 MB (14509812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f96a83aedee46aef2be1d4f73cc6990dc7e756981b022462100ac16fad345`  
		Last Modified: Thu, 22 Jul 2021 17:42:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9466f2ac94d013cc74523ee4ad44d9720c72baa51d8aecc2afcba41c3754be44`  
		Last Modified: Fri, 23 Jul 2021 11:10:32 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbad6372ccefa1ce14b5eefe2fe718c0cd234b40bf9a70e3d02e131a9dd65d26`  
		Last Modified: Fri, 23 Jul 2021 11:10:45 GMT  
		Size: 94.1 MB (94087869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93724991108aa18238773a3122f3fcd80f69331610c0a7f00656f690ac7692`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19466676666dc7f1a145b5b2534855e6f32c152cd3da118bc5536badc24da33d`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc48a22ec231d5048d556cd637291655083a29acb695b0073039d36315929da`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 3.1 MB (3058677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00b1336ee6986b3f2923502d082ce45ebccea58e21f85ddd12812be6796e1f`  
		Last Modified: Fri, 23 Jul 2021 11:10:33 GMT  
		Size: 44.1 MB (44106755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fe342d55cb9155ec0d7a14a371258946d43b0b4e3df44e3f1bbe9b166a5ef`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:9ef48dcd233199a54171d5bf678c6fc5245453cdd9827c68ce9b91796501de9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196974351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25105893bd633c389af7ab7f4e947fa0ff2172ac3cd182d70b9bc2d2a45607e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:39:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:48:33 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 14:48:33 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 14:48:34 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 14:52:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:52:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:52:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:52:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:52:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:52:55 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:25:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:26:16 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:26:17 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:26:17 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:26:18 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:26:19 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 01:26:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 01:26:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:32:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:32:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:32:10 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:32:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:32:11 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:32:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9237058b7c5120d5c6315b5d17a8c1d783be09a228b83772111ce9436c29d078`  
		Last Modified: Thu, 22 Jul 2021 15:15:34 GMT  
		Size: 10.3 MB (10345807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144b4344f580222d2fbc2f0d80fc139ab1a1ddb9a245b6073c41fdca9a93c23e`  
		Last Modified: Thu, 22 Jul 2021 15:15:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8ddbd20410764a5a44de2520de7417bddfcc0fdf2f4fa1b1d4e9ac785ce253`  
		Last Modified: Thu, 22 Jul 2021 15:17:00 GMT  
		Size: 13.9 MB (13871315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1fe10899466e387c0fc9cc130a0a900ffeb91af92c09301e387e444836d74f`  
		Last Modified: Thu, 22 Jul 2021 15:16:52 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b419523e1af1c8a3f9891c74f5e29e5697be8bf7bf57f23880ac551c460f07`  
		Last Modified: Fri, 23 Jul 2021 01:48:00 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d44a2001e78eed6fc3a85dbe0059a0bfae376949cda406c9304941ed617a23`  
		Last Modified: Fri, 23 Jul 2021 01:49:01 GMT  
		Size: 89.6 MB (89576912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2901c80e9a45cf66afe7fb2306719b195ec9c983783f4058ef68246bb10b95`  
		Last Modified: Fri, 23 Jul 2021 01:47:58 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0cf9a21c70c0994e217daf5f71efd9d2f8ce8f36e062be7c831492162e99a`  
		Last Modified: Fri, 23 Jul 2021 01:47:57 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5daae06ca7c40f7fa2e94d4be701850020a63374c01cb310471f056eda7498`  
		Last Modified: Fri, 23 Jul 2021 01:48:01 GMT  
		Size: 3.1 MB (3058682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d9118a275db8a49fd1b15511383b91ac8b867604e68e255d097c4a7880a8ff`  
		Last Modified: Fri, 23 Jul 2021 01:48:21 GMT  
		Size: 55.2 MB (55238308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d94f744aa1ad4af6e0d39600d4e4bf9e68e942510443afa0d8ecf37e30835`  
		Last Modified: Fri, 23 Jul 2021 01:47:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:3aca8dadb5407c0d388ac5baf1a99dbeeabc4fe3da1c506883b1c394c7fe7610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9074a5390b69761aca8dcac7078799a4f869792b8311bc2280916419daa31aca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:15:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 02:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 02:25:03 GMT
ENV RUBY_MAJOR=2.7
# Fri, 23 Jul 2021 02:25:04 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 23 Jul 2021 02:25:04 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 23 Jul 2021 02:29:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 02:29:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 02:29:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 02:29:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:29:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 02:29:10 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 21:18:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 21:19:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 21:19:37 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 21:19:37 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 21:19:38 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 21:19:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 21:19:40 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 21:19:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 21:19:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 21:25:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 21:25:05 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 21:25:06 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 21:25:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 21:25:06 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 21:25:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b8c791d70de7f22816846fbb07e0a1d7d419841c7e539a7cf57ef05fd50c5`  
		Last Modified: Fri, 23 Jul 2021 03:05:10 GMT  
		Size: 9.9 MB (9872218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12a7edb0af862efa24dc389d7901cd2a894f2e106a1cef931ba0a6d675e2c0`  
		Last Modified: Fri, 23 Jul 2021 03:05:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b75d257bf75804e51385b730af2aaba386a501ef50517b8379966d4372c8597`  
		Last Modified: Fri, 23 Jul 2021 03:06:48 GMT  
		Size: 13.8 MB (13766962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc7c7e0536ed6ba4a99c1b8960d7c1d7365c8bc52d230b8af44d07d085916f`  
		Last Modified: Fri, 23 Jul 2021 03:06:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9cbdbb67af5c0b986c2fd6f93a2bacf3c795b046bfdf19e8f483dbc780c643`  
		Last Modified: Fri, 23 Jul 2021 21:39:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823bb8e3702405c250a7cc3dadba844fef162cbd0f5b9fb70a107f618dffeddf`  
		Last Modified: Fri, 23 Jul 2021 21:40:51 GMT  
		Size: 85.6 MB (85590187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930c9cc4f262f629914e37abf7b88697bc949d34260a237f8d740ea30ddf5902`  
		Last Modified: Fri, 23 Jul 2021 21:39:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e7aa3a63516ee59c6e77fd1a74b1ce0b303c09b2a97dd0ca3b0af594021030`  
		Last Modified: Fri, 23 Jul 2021 21:39:55 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b8cbe774bbfa06d5d0e463126138a655e455605ce81a4b4799b6495959723`  
		Last Modified: Fri, 23 Jul 2021 21:39:58 GMT  
		Size: 3.1 MB (3058685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231b30773994af4c612b2b73b0a33eef728b235396a59b1c34d64b17c2289dd`  
		Last Modified: Fri, 23 Jul 2021 21:40:19 GMT  
		Size: 55.1 MB (55076883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af42513ad3b3f3a0291481c9f4b6a077a9e62fc8cd14736897d28d5f70687618`  
		Last Modified: Fri, 23 Jul 2021 21:39:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:b7a96326ffb8fc77358a78fac0448fd3c56dd2fb1feb29dd3528e6cac29cd155
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203231883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e4b31ef3849045f66d5846fad154cbaf41e73cd54c0a5afcf7bed7817d16a5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 12:36:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 12:41:08 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 12:41:08 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 12:41:09 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 12:43:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 12:43:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 12:43:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 12:43:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 12:43:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 12:43:05 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:57:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:58:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:58:04 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:58:04 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:58:04 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:58:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:58:05 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 00:58:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 00:58:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:00:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:00:36 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:00:36 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:00:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:00:36 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:00:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a77364b6ec6cfc9422903e0f9d3f5cab5ee0ac4b62cfac6fc7c3d544ad7f57`  
		Last Modified: Thu, 22 Jul 2021 12:55:11 GMT  
		Size: 11.3 MB (11263053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a68321ef048d82e4480bc2de1681a811f18b2e1d04b5aa9dec38030570eaa40`  
		Last Modified: Thu, 22 Jul 2021 12:55:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ec69cd14df7f6066799b20f9268ae3ce6e5e0564c2b560a10804765f4c7cf`  
		Last Modified: Thu, 22 Jul 2021 12:56:22 GMT  
		Size: 14.4 MB (14356675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4a2f06c1cec263f641737334f76372caff218cb8312bc8375c4e69c7289147`  
		Last Modified: Thu, 22 Jul 2021 12:56:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02fa466075ed10ab6e904b032ad10baf66dce45f41bb930b1ea5728647d32c`  
		Last Modified: Fri, 23 Jul 2021 01:06:41 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde3ab2a527d4e47aafb6f9cf0128ee08d754d6bed600addccaa4309e29f6437`  
		Last Modified: Fri, 23 Jul 2021 01:06:56 GMT  
		Size: 92.6 MB (92610625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f378e820ad759f627889603226956c607d864e95e967c969aa7965d93fb45816`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8291e2aab5ca9a9c51cc69c4cab741f3d46369744adec4f04f120329ed36f48d`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314b7425fd6ac642e912d76f7f9dafe5eda902a1abd7ab0ad23662da1bb75d73`  
		Last Modified: Fri, 23 Jul 2021 01:06:39 GMT  
		Size: 3.1 MB (3058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9b783db9ec2f80081bb3fc6226424e234ca9e33e9da8e7e6784a9e8b2a4b9f`  
		Last Modified: Fri, 23 Jul 2021 01:06:44 GMT  
		Size: 56.0 MB (56023809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f20fa5c3f8387a262408432f792b73cb61c7957e5c6ba4edd46d4da28d05a6c`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.1` - linux; 386

```console
$ docker pull redmine@sha256:e0c39c52abc9d57cf5bd97523c15db6fe60284390d12d89bd95e1d8ff7ea69dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202117810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6402098c31c9ce288516e50c34618b6cdce5229aaefc10ad583c89f4e4144289`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:38:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:39:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 15:39:00 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 15:49:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:49:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:49:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:49:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:49:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:49:39 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:10:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:11:45 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:11:45 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:11:46 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:11:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:11:48 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 00:11:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 00:11:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 00:13:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 00:13:26 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 00:13:26 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 00:13:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 00:13:27 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 00:13:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d04ca5200ad3b98494cfde36960022dbd29c9afc33d685ac499fae8a05d63`  
		Last Modified: Thu, 22 Jul 2021 16:06:57 GMT  
		Size: 17.2 MB (17227285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d9d06c9e919afbd9358b702cad5bc0f28b8150722ffedb25ece16dc1f19b2`  
		Last Modified: Thu, 22 Jul 2021 16:06:48 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9e06bdf88f28c2f5d5893c862c6da8a6a73eb098cb2cd8eec57656d9a79b69`  
		Last Modified: Thu, 22 Jul 2021 16:08:14 GMT  
		Size: 14.0 MB (13992268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4f84633b2fe0d1dff5a1fd6ab3a5506af8978d94ded4f5a0f2727ce06805d4`  
		Last Modified: Thu, 22 Jul 2021 16:08:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57ef59b51318d382563cb5fdab4577df04d06c56bd8885926c9a9374a31ed7c`  
		Last Modified: Fri, 23 Jul 2021 00:22:32 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2922ffac0f77cf1fd832a20d48b586a6621e1d75610c055227f6d76e34928b16`  
		Last Modified: Fri, 23 Jul 2021 00:23:09 GMT  
		Size: 95.7 MB (95703233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb8c5967872202784509fa53a811f849c714ef794dd53a40047d0c81585ce4`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c1ffe6294aae5e8df812aee47c20e59fe0f4ec3593946e4ed069116ebb9f1`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f26aa32bafd59c6d9237ded27dc8ab964a91915e3b9a678b76d587899376ec`  
		Last Modified: Fri, 23 Jul 2021 00:22:31 GMT  
		Size: 3.1 MB (3058690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba425f932ee35d618a7e2a024cf68062985ba8dbbedbfd829e6af8cb1d1978b6`  
		Last Modified: Fri, 23 Jul 2021 00:22:45 GMT  
		Size: 44.3 MB (44334640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bca1f4ee34a1ccde3aac51ad07cafbaa3d857e77059427b1f928f48da6a0134`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 1.8 KB (1797 bytes)  
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
$ docker pull redmine@sha256:37201304a98b29096c65aff1082800685f8811d091fecfdbbfbc4b02ce56c712
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202549844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cceccec5920cb372b1e0e6536384018db9d2cf92a8ccf57721c5e55ec24b272`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:03:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:03:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:03:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:23:01 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 14:23:02 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 14:23:03 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 14:26:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:26:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:26:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:26:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:26:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:26:30 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 02:07:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:08:34 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 02:08:34 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 02:08:34 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 02:08:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 02:08:35 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 02:08:36 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 02:08:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 02:10:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 02:10:31 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 02:10:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 02:10:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:10:32 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 02:10:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d658cd93dd34abb2452544d10308c796ec6310f6d1ca2d2762c8e85402e3e`  
		Last Modified: Thu, 22 Jul 2021 14:48:41 GMT  
		Size: 10.8 MB (10814518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bebc1f15c6904197539abc99a69885fa65493d7fae9f27d2529be2fa05491e`  
		Last Modified: Thu, 22 Jul 2021 14:48:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa61230ad4685d16dfcb4b68dd88f40b84ddf598a2031852e9881218e137c19a`  
		Last Modified: Thu, 22 Jul 2021 14:49:27 GMT  
		Size: 14.7 MB (14697201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f9ff30668a8bd8fd8341049bbebd3d1db4e433d0116f70111daa596abf7e7a`  
		Last Modified: Thu, 22 Jul 2021 14:49:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91522d35fa6424129e9d5eb39ac436e70fd9e80337413131aa3401b1496857ff`  
		Last Modified: Fri, 23 Jul 2021 02:17:18 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5900d840b86d971e896fc6c7451e9a176bd80fa994f5090d5dbcf5ef6e48b14`  
		Last Modified: Fri, 23 Jul 2021 02:17:31 GMT  
		Size: 91.8 MB (91790782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede4b68f2bb6676b42e076513a0c075e3da52f75acb4070789e5d12196646541`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add04b7bc101933c98b8043337844f9e18f272fd13d47b87100f4fd9f52710b2`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51111bc126246f79519ed7c546b73f24285cc97694e205b48267a20ba50637f2`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 3.1 MB (3058684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad5d1e67f7c62f6d33343a9632c4aca3d5c808a4a4a18a476fcad4acf39bdb`  
		Last Modified: Fri, 23 Jul 2021 02:17:26 GMT  
		Size: 56.4 MB (56423655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c540e32ed87a6e82bdca054e93ee83775afa16fab29404772b98d2a047156a0c`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.1-alpine`

```console
$ docker pull redmine@sha256:7de4015773da4d105b5f43705556003eb3071d781612fa6e7f6010981e4e56e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull redmine@sha256:4198d395967db00ec073ed9d714c41b00472e77e49b0dcae51f259d9b78dbc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:43a77f34a70b4e12264df8bff7377b5ae47895166cfd156a903cb28b641fec29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0604330a8f415b11297aee811ea898c9a092e3255eb53a843e412e37469ba9d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 17:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:28:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:28:25 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:03:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:04:03 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:04:03 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:04:03 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:04:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 11:04:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:04:49 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:04:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:49 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:04:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 23 Jul 2021 11:04:59 GMT
ENV PASSENGER_VERSION=6.0.10
# Fri, 23 Jul 2021 11:05:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:05:16 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 23 Jul 2021 11:05:17 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 23 Jul 2021 11:05:17 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e582c090726ff249b7e30253c7f0c11aa2cd14282a8b6cd0e8055c8615e5586`  
		Last Modified: Thu, 22 Jul 2021 17:42:40 GMT  
		Size: 14.5 MB (14509812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f96a83aedee46aef2be1d4f73cc6990dc7e756981b022462100ac16fad345`  
		Last Modified: Thu, 22 Jul 2021 17:42:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9466f2ac94d013cc74523ee4ad44d9720c72baa51d8aecc2afcba41c3754be44`  
		Last Modified: Fri, 23 Jul 2021 11:10:32 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbad6372ccefa1ce14b5eefe2fe718c0cd234b40bf9a70e3d02e131a9dd65d26`  
		Last Modified: Fri, 23 Jul 2021 11:10:45 GMT  
		Size: 94.1 MB (94087869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93724991108aa18238773a3122f3fcd80f69331610c0a7f00656f690ac7692`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19466676666dc7f1a145b5b2534855e6f32c152cd3da118bc5536badc24da33d`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc48a22ec231d5048d556cd637291655083a29acb695b0073039d36315929da`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 3.1 MB (3058677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00b1336ee6986b3f2923502d082ce45ebccea58e21f85ddd12812be6796e1f`  
		Last Modified: Fri, 23 Jul 2021 11:10:33 GMT  
		Size: 44.1 MB (44106755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fe342d55cb9155ec0d7a14a371258946d43b0b4e3df44e3f1bbe9b166a5ef`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8e911f2db9cefa3945c1c8bbcc4e9dc79575560305045da7e987dfa48fa522`  
		Last Modified: Fri, 23 Jul 2021 11:11:07 GMT  
		Size: 21.1 MB (21131293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab210a34ab4fa48ee042162c1b27897332d05666f95bb001a39f2d04a7df605`  
		Last Modified: Fri, 23 Jul 2021 11:11:05 GMT  
		Size: 4.9 MB (4919283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:alpine`

```console
$ docker pull redmine@sha256:7de4015773da4d105b5f43705556003eb3071d781612fa6e7f6010981e4e56e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
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
$ docker pull redmine@sha256:95435c3e6e2d0815459d7c44520b2743dbb8806cba32184ba0bfdf143d5af0b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `redmine:latest` - linux; amd64

```console
$ docker pull redmine@sha256:e28ea2b1f675569c4763cf0cd04ff101d384a263d952858b8e7533b7f335f34a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195475927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be97e87738155b1d102c2b0b7286bd39b06e62a5a8184e8fb0e21b7a2e819743`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 17:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:28:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:28:25 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:03:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:04:03 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:04:03 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:04:03 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:04:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 11:04:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:04:49 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:04:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:49 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:04:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e582c090726ff249b7e30253c7f0c11aa2cd14282a8b6cd0e8055c8615e5586`  
		Last Modified: Thu, 22 Jul 2021 17:42:40 GMT  
		Size: 14.5 MB (14509812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f96a83aedee46aef2be1d4f73cc6990dc7e756981b022462100ac16fad345`  
		Last Modified: Thu, 22 Jul 2021 17:42:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9466f2ac94d013cc74523ee4ad44d9720c72baa51d8aecc2afcba41c3754be44`  
		Last Modified: Fri, 23 Jul 2021 11:10:32 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbad6372ccefa1ce14b5eefe2fe718c0cd234b40bf9a70e3d02e131a9dd65d26`  
		Last Modified: Fri, 23 Jul 2021 11:10:45 GMT  
		Size: 94.1 MB (94087869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93724991108aa18238773a3122f3fcd80f69331610c0a7f00656f690ac7692`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19466676666dc7f1a145b5b2534855e6f32c152cd3da118bc5536badc24da33d`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc48a22ec231d5048d556cd637291655083a29acb695b0073039d36315929da`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 3.1 MB (3058677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00b1336ee6986b3f2923502d082ce45ebccea58e21f85ddd12812be6796e1f`  
		Last Modified: Fri, 23 Jul 2021 11:10:33 GMT  
		Size: 44.1 MB (44106755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fe342d55cb9155ec0d7a14a371258946d43b0b4e3df44e3f1bbe9b166a5ef`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:9ef48dcd233199a54171d5bf678c6fc5245453cdd9827c68ce9b91796501de9d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196974351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25105893bd633c389af7ab7f4e947fa0ff2172ac3cd182d70b9bc2d2a45607e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:50:06 GMT
ADD file:885454a996e63d5eb93f1f365a3be77a441f368d7f5a77a7fd1636edf5d0b8cd in / 
# Thu, 22 Jul 2021 00:50:07 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:39:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:39:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:39:29 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:48:33 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 14:48:33 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 14:48:34 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 14:52:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:52:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:52:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:52:53 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:52:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:52:55 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 01:25:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 01:26:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 01:26:16 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 01:26:17 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 01:26:17 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 01:26:18 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 01:26:19 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 01:26:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 01:26:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:32:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:32:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:32:10 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:32:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:32:11 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:32:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:2b96a0a1ddfe4fab89025b13e583392414251af73361434f28af076c3db77100`  
		Last Modified: Thu, 22 Jul 2021 01:02:11 GMT  
		Size: 24.9 MB (24879093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9237058b7c5120d5c6315b5d17a8c1d783be09a228b83772111ce9436c29d078`  
		Last Modified: Thu, 22 Jul 2021 15:15:34 GMT  
		Size: 10.3 MB (10345807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144b4344f580222d2fbc2f0d80fc139ab1a1ddb9a245b6073c41fdca9a93c23e`  
		Last Modified: Thu, 22 Jul 2021 15:15:26 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8ddbd20410764a5a44de2520de7417bddfcc0fdf2f4fa1b1d4e9ac785ce253`  
		Last Modified: Thu, 22 Jul 2021 15:17:00 GMT  
		Size: 13.9 MB (13871315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1fe10899466e387c0fc9cc130a0a900ffeb91af92c09301e387e444836d74f`  
		Last Modified: Thu, 22 Jul 2021 15:16:52 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b419523e1af1c8a3f9891c74f5e29e5697be8bf7bf57f23880ac551c460f07`  
		Last Modified: Fri, 23 Jul 2021 01:48:00 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d44a2001e78eed6fc3a85dbe0059a0bfae376949cda406c9304941ed617a23`  
		Last Modified: Fri, 23 Jul 2021 01:49:01 GMT  
		Size: 89.6 MB (89576912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc2901c80e9a45cf66afe7fb2306719b195ec9c983783f4058ef68246bb10b95`  
		Last Modified: Fri, 23 Jul 2021 01:47:58 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b0cf9a21c70c0994e217daf5f71efd9d2f8ce8f36e062be7c831492162e99a`  
		Last Modified: Fri, 23 Jul 2021 01:47:57 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5daae06ca7c40f7fa2e94d4be701850020a63374c01cb310471f056eda7498`  
		Last Modified: Fri, 23 Jul 2021 01:48:01 GMT  
		Size: 3.1 MB (3058682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d9118a275db8a49fd1b15511383b91ac8b867604e68e255d097c4a7880a8ff`  
		Last Modified: Fri, 23 Jul 2021 01:48:21 GMT  
		Size: 55.2 MB (55238308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d94f744aa1ad4af6e0d39600d4e4bf9e68e942510443afa0d8ecf37e30835`  
		Last Modified: Fri, 23 Jul 2021 01:47:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:3aca8dadb5407c0d388ac5baf1a99dbeeabc4fe3da1c506883b1c394c7fe7610
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115143 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9074a5390b69761aca8dcac7078799a4f869792b8311bc2280916419daa31aca`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:46 GMT
ADD file:8f466611d9ba85407e1768128a6a2a51886b78675a4775badb9d42e57c4a182e in / 
# Thu, 22 Jul 2021 02:03:47 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 02:15:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:15:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 02:15:46 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 02:25:03 GMT
ENV RUBY_MAJOR=2.7
# Fri, 23 Jul 2021 02:25:04 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 23 Jul 2021 02:25:04 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 23 Jul 2021 02:29:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 02:29:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 02:29:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 02:29:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 02:29:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 02:29:10 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 21:18:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 21:19:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 21:19:37 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 21:19:37 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 21:19:38 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 21:19:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 21:19:40 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 21:19:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 21:19:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 21:25:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 21:25:05 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 21:25:06 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 21:25:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 21:25:06 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 21:25:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:607f77084e8a15bf45d56215b058a593cdcf4e0039e5326157954b12663c0d31`  
		Last Modified: Thu, 22 Jul 2021 02:16:17 GMT  
		Size: 22.7 MB (22745974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011b8c791d70de7f22816846fbb07e0a1d7d419841c7e539a7cf57ef05fd50c5`  
		Last Modified: Fri, 23 Jul 2021 03:05:10 GMT  
		Size: 9.9 MB (9872218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb12a7edb0af862efa24dc389d7901cd2a894f2e106a1cef931ba0a6d675e2c0`  
		Last Modified: Fri, 23 Jul 2021 03:05:04 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b75d257bf75804e51385b730af2aaba386a501ef50517b8379966d4372c8597`  
		Last Modified: Fri, 23 Jul 2021 03:06:48 GMT  
		Size: 13.8 MB (13766962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbc7c7e0536ed6ba4a99c1b8960d7c1d7365c8bc52d230b8af44d07d085916f`  
		Last Modified: Fri, 23 Jul 2021 03:06:40 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9cbdbb67af5c0b986c2fd6f93a2bacf3c795b046bfdf19e8f483dbc780c643`  
		Last Modified: Fri, 23 Jul 2021 21:39:57 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823bb8e3702405c250a7cc3dadba844fef162cbd0f5b9fb70a107f618dffeddf`  
		Last Modified: Fri, 23 Jul 2021 21:40:51 GMT  
		Size: 85.6 MB (85590187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930c9cc4f262f629914e37abf7b88697bc949d34260a237f8d740ea30ddf5902`  
		Last Modified: Fri, 23 Jul 2021 21:39:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e7aa3a63516ee59c6e77fd1a74b1ce0b303c09b2a97dd0ca3b0af594021030`  
		Last Modified: Fri, 23 Jul 2021 21:39:55 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224b8cbe774bbfa06d5d0e463126138a655e455605ce81a4b4799b6495959723`  
		Last Modified: Fri, 23 Jul 2021 21:39:58 GMT  
		Size: 3.1 MB (3058685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d231b30773994af4c612b2b73b0a33eef728b235396a59b1c34d64b17c2289dd`  
		Last Modified: Fri, 23 Jul 2021 21:40:19 GMT  
		Size: 55.1 MB (55076883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af42513ad3b3f3a0291481c9f4b6a077a9e62fc8cd14736897d28d5f70687618`  
		Last Modified: Fri, 23 Jul 2021 21:39:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:b7a96326ffb8fc77358a78fac0448fd3c56dd2fb1feb29dd3528e6cac29cd155
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203231883 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15e4b31ef3849045f66d5846fad154cbaf41e73cd54c0a5afcf7bed7817d16a5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:40:14 GMT
ADD file:074ffc2065bab83c9a5c596576656b04d271dd78406aadad160b68e38f38269f in / 
# Thu, 22 Jul 2021 00:40:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 12:36:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 12:36:23 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 12:41:08 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 12:41:08 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 12:41:09 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 12:43:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 12:43:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 12:43:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 12:43:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 12:43:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 12:43:05 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:57:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:58:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:58:04 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:58:04 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:58:04 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:58:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:58:05 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 00:58:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 00:58:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 01:00:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 01:00:36 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 01:00:36 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 01:00:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 01:00:36 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 01:00:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:513c6babab2b9079da61a69300c0e26d1037ca98910376098e9ae87baeb112c0`  
		Last Modified: Thu, 22 Jul 2021 00:45:53 GMT  
		Size: 25.9 MB (25914794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79a77364b6ec6cfc9422903e0f9d3f5cab5ee0ac4b62cfac6fc7c3d544ad7f57`  
		Last Modified: Thu, 22 Jul 2021 12:55:11 GMT  
		Size: 11.3 MB (11263053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a68321ef048d82e4480bc2de1681a811f18b2e1d04b5aa9dec38030570eaa40`  
		Last Modified: Thu, 22 Jul 2021 12:55:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ec69cd14df7f6066799b20f9268ae3ce6e5e0564c2b560a10804765f4c7cf`  
		Last Modified: Thu, 22 Jul 2021 12:56:22 GMT  
		Size: 14.4 MB (14356675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4a2f06c1cec263f641737334f76372caff218cb8312bc8375c4e69c7289147`  
		Last Modified: Thu, 22 Jul 2021 12:56:20 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa02fa466075ed10ab6e904b032ad10baf66dce45f41bb930b1ea5728647d32c`  
		Last Modified: Fri, 23 Jul 2021 01:06:41 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde3ab2a527d4e47aafb6f9cf0128ee08d754d6bed600addccaa4309e29f6437`  
		Last Modified: Fri, 23 Jul 2021 01:06:56 GMT  
		Size: 92.6 MB (92610625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f378e820ad759f627889603226956c607d864e95e967c969aa7965d93fb45816`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8291e2aab5ca9a9c51cc69c4cab741f3d46369744adec4f04f120329ed36f48d`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314b7425fd6ac642e912d76f7f9dafe5eda902a1abd7ab0ad23662da1bb75d73`  
		Last Modified: Fri, 23 Jul 2021 01:06:39 GMT  
		Size: 3.1 MB (3058678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9b783db9ec2f80081bb3fc6226424e234ca9e33e9da8e7e6784a9e8b2a4b9f`  
		Last Modified: Fri, 23 Jul 2021 01:06:44 GMT  
		Size: 56.0 MB (56023809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f20fa5c3f8387a262408432f792b73cb61c7957e5c6ba4edd46d4da28d05a6c`  
		Last Modified: Fri, 23 Jul 2021 01:06:38 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:e0c39c52abc9d57cf5bd97523c15db6fe60284390d12d89bd95e1d8ff7ea69dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202117810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6402098c31c9ce288516e50c34618b6cdce5229aaefc10ad583c89f4e4144289`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:50 GMT
ADD file:cb657a3d01f25bf815677ce223e8802d054f11aeb95f85b160982277916637bd in / 
# Thu, 22 Jul 2021 00:39:51 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 15:38:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 15:39:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 15:39:00 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 15:46:48 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 15:49:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 15:49:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 15:49:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 15:49:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 15:49:38 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 15:49:39 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 00:10:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 00:11:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:11:45 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 00:11:45 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 00:11:46 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 00:11:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 00:11:48 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 00:11:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 00:11:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 00:13:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 00:13:26 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 00:13:26 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 00:13:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 00:13:27 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 00:13:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fa9d06db5f4195bd51665a89e08e2e7db25636ac28ab162fe876ae0a53093fe5`  
		Last Modified: Thu, 22 Jul 2021 00:46:36 GMT  
		Size: 27.8 MB (27797459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071d04ca5200ad3b98494cfde36960022dbd29c9afc33d685ac499fae8a05d63`  
		Last Modified: Thu, 22 Jul 2021 16:06:57 GMT  
		Size: 17.2 MB (17227285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96d9d06c9e919afbd9358b702cad5bc0f28b8150722ffedb25ece16dc1f19b2`  
		Last Modified: Thu, 22 Jul 2021 16:06:48 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9e06bdf88f28c2f5d5893c862c6da8a6a73eb098cb2cd8eec57656d9a79b69`  
		Last Modified: Thu, 22 Jul 2021 16:08:14 GMT  
		Size: 14.0 MB (13992268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4f84633b2fe0d1dff5a1fd6ab3a5506af8978d94ded4f5a0f2727ce06805d4`  
		Last Modified: Thu, 22 Jul 2021 16:08:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57ef59b51318d382563cb5fdab4577df04d06c56bd8885926c9a9374a31ed7c`  
		Last Modified: Fri, 23 Jul 2021 00:22:32 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2922ffac0f77cf1fd832a20d48b586a6621e1d75610c055227f6d76e34928b16`  
		Last Modified: Fri, 23 Jul 2021 00:23:09 GMT  
		Size: 95.7 MB (95703233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeb8c5967872202784509fa53a811f849c714ef794dd53a40047d0c81585ce4`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f2c1ffe6294aae5e8df812aee47c20e59fe0f4ec3593946e4ed069116ebb9f1`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f26aa32bafd59c6d9237ded27dc8ab964a91915e3b9a678b76d587899376ec`  
		Last Modified: Fri, 23 Jul 2021 00:22:31 GMT  
		Size: 3.1 MB (3058690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba425f932ee35d618a7e2a024cf68062985ba8dbbedbfd829e6af8cb1d1978b6`  
		Last Modified: Fri, 23 Jul 2021 00:22:45 GMT  
		Size: 44.3 MB (44334640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bca1f4ee34a1ccde3aac51ad07cafbaa3d857e77059427b1f928f48da6a0134`  
		Last Modified: Fri, 23 Jul 2021 00:22:29 GMT  
		Size: 1.8 KB (1797 bytes)  
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
$ docker pull redmine@sha256:37201304a98b29096c65aff1082800685f8811d091fecfdbbfbc4b02ce56c712
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.5 MB (202549844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cceccec5920cb372b1e0e6536384018db9d2cf92a8ccf57721c5e55ec24b272`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:42:45 GMT
ADD file:1ab999eb6f80d8ce91ce3a173e23fd2710f2779117bba29037eaa82aadcbf6ed in / 
# Thu, 22 Jul 2021 00:42:48 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 14:03:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 14:03:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 14:03:21 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 14:23:01 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 14:23:02 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 14:23:03 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 14:26:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 14:26:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 14:26:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 14:26:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 14:26:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 14:26:30 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 02:07:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 02:08:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:08:34 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 02:08:34 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 02:08:34 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 02:08:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 02:08:35 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 02:08:36 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 02:08:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 02:10:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 02:10:31 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 02:10:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 02:10:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 02:10:32 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 02:10:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a50fdd85ff244c1465e71c51354d055e3df0b90ff5faad28cc22d9ecde9daf3`  
		Last Modified: Thu, 22 Jul 2021 00:48:13 GMT  
		Size: 25.8 MB (25760761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8d658cd93dd34abb2452544d10308c796ec6310f6d1ca2d2762c8e85402e3e`  
		Last Modified: Thu, 22 Jul 2021 14:48:41 GMT  
		Size: 10.8 MB (10814518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09bebc1f15c6904197539abc99a69885fa65493d7fae9f27d2529be2fa05491e`  
		Last Modified: Thu, 22 Jul 2021 14:48:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa61230ad4685d16dfcb4b68dd88f40b84ddf598a2031852e9881218e137c19a`  
		Last Modified: Thu, 22 Jul 2021 14:49:27 GMT  
		Size: 14.7 MB (14697201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f9ff30668a8bd8fd8341049bbebd3d1db4e433d0116f70111daa596abf7e7a`  
		Last Modified: Thu, 22 Jul 2021 14:49:26 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91522d35fa6424129e9d5eb39ac436e70fd9e80337413131aa3401b1496857ff`  
		Last Modified: Fri, 23 Jul 2021 02:17:18 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5900d840b86d971e896fc6c7451e9a176bd80fa994f5090d5dbcf5ef6e48b14`  
		Last Modified: Fri, 23 Jul 2021 02:17:31 GMT  
		Size: 91.8 MB (91790782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede4b68f2bb6676b42e076513a0c075e3da52f75acb4070789e5d12196646541`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add04b7bc101933c98b8043337844f9e18f272fd13d47b87100f4fd9f52710b2`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51111bc126246f79519ed7c546b73f24285cc97694e205b48267a20ba50637f2`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 3.1 MB (3058684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ad5d1e67f7c62f6d33343a9632c4aca3d5c808a4a4a18a476fcad4acf39bdb`  
		Last Modified: Fri, 23 Jul 2021 02:17:26 GMT  
		Size: 56.4 MB (56423655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c540e32ed87a6e82bdca054e93ee83775afa16fab29404772b98d2a047156a0c`  
		Last Modified: Fri, 23 Jul 2021 02:17:17 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:passenger`

```console
$ docker pull redmine@sha256:4198d395967db00ec073ed9d714c41b00472e77e49b0dcae51f259d9b78dbc48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:43a77f34a70b4e12264df8bff7377b5ae47895166cfd156a903cb28b641fec29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0604330a8f415b11297aee811ea898c9a092e3255eb53a843e412e37469ba9d2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:43 GMT
ADD file:45f5dfa135c848a348382413cb8b66a3b1dac3276814fbbe4684b39101d1b148 in / 
# Thu, 22 Jul 2021 00:45:44 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 17:20:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 17:20:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 22 Jul 2021 17:20:06 GMT
ENV LANG=C.UTF-8
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_MAJOR=2.7
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_VERSION=2.7.4
# Thu, 22 Jul 2021 17:25:56 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 22 Jul 2021 17:28:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 22 Jul 2021 17:28:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 22 Jul 2021 17:28:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 22 Jul 2021 17:28:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 22 Jul 2021 17:28:25 GMT
CMD ["irb"]
# Fri, 23 Jul 2021 11:03:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 23 Jul 2021 11:04:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:04:03 GMT
ENV RAILS_ENV=production
# Fri, 23 Jul 2021 11:04:03 GMT
WORKDIR /usr/src/redmine
# Fri, 23 Jul 2021 11:04:03 GMT
ENV HOME=/home/redmine
# Fri, 23 Jul 2021 11:04:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_VERSION=4.2.1
# Fri, 23 Jul 2021 11:04:04 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Fri, 23 Jul 2021 11:04:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 23 Jul 2021 11:04:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:04:49 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 23 Jul 2021 11:04:49 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 23 Jul 2021 11:04:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:49 GMT
EXPOSE 3000
# Fri, 23 Jul 2021 11:04:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 23 Jul 2021 11:04:59 GMT
ENV PASSENGER_VERSION=6.0.10
# Fri, 23 Jul 2021 11:05:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 23 Jul 2021 11:05:16 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 23 Jul 2021 11:05:17 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 23 Jul 2021 11:05:17 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:33847f680f63fb1b343a9fc782e267b5abdbdb50d65d4b9bd2a136291d67cf75`  
		Last Modified: Thu, 22 Jul 2021 00:50:35 GMT  
		Size: 27.1 MB (27145795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603cdcbaa70592c67c84ffc51d232163508c6c3480916880fdb7820e7c9b9c17`  
		Last Modified: Thu, 22 Jul 2021 17:41:27 GMT  
		Size: 12.6 MB (12562773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d872ffd3f2a7e6eabea705393351362003a0c6bdee8956d5a53f73dd0b40be`  
		Last Modified: Thu, 22 Jul 2021 17:41:25 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e582c090726ff249b7e30253c7f0c11aa2cd14282a8b6cd0e8055c8615e5586`  
		Last Modified: Thu, 22 Jul 2021 17:42:40 GMT  
		Size: 14.5 MB (14509812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6f96a83aedee46aef2be1d4f73cc6990dc7e756981b022462100ac16fad345`  
		Last Modified: Thu, 22 Jul 2021 17:42:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9466f2ac94d013cc74523ee4ad44d9720c72baa51d8aecc2afcba41c3754be44`  
		Last Modified: Fri, 23 Jul 2021 11:10:32 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbad6372ccefa1ce14b5eefe2fe718c0cd234b40bf9a70e3d02e131a9dd65d26`  
		Last Modified: Fri, 23 Jul 2021 11:10:45 GMT  
		Size: 94.1 MB (94087869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b93724991108aa18238773a3122f3fcd80f69331610c0a7f00656f690ac7692`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19466676666dc7f1a145b5b2534855e6f32c152cd3da118bc5536badc24da33d`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc48a22ec231d5048d556cd637291655083a29acb695b0073039d36315929da`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 3.1 MB (3058677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe00b1336ee6986b3f2923502d082ce45ebccea58e21f85ddd12812be6796e1f`  
		Last Modified: Fri, 23 Jul 2021 11:10:33 GMT  
		Size: 44.1 MB (44106755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:606fe342d55cb9155ec0d7a14a371258946d43b0b4e3df44e3f1bbe9b166a5ef`  
		Last Modified: Fri, 23 Jul 2021 11:10:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8e911f2db9cefa3945c1c8bbcc4e9dc79575560305045da7e987dfa48fa522`  
		Last Modified: Fri, 23 Jul 2021 11:11:07 GMT  
		Size: 21.1 MB (21131293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab210a34ab4fa48ee042162c1b27897332d05666f95bb001a39f2d04a7df605`  
		Last Modified: Fri, 23 Jul 2021 11:11:05 GMT  
		Size: 4.9 MB (4919283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
