<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `redmine`

-	[`redmine:4`](#redmine4)
-	[`redmine:4-alpine`](#redmine4-alpine)
-	[`redmine:4-passenger`](#redmine4-passenger)
-	[`redmine:4.0`](#redmine40)
-	[`redmine:4.0-alpine`](#redmine40-alpine)
-	[`redmine:4.0-passenger`](#redmine40-passenger)
-	[`redmine:4.0.8`](#redmine408)
-	[`redmine:4.0.8-alpine`](#redmine408-alpine)
-	[`redmine:4.0.8-passenger`](#redmine408-passenger)
-	[`redmine:4.1`](#redmine41)
-	[`redmine:4.1-alpine`](#redmine41-alpine)
-	[`redmine:4.1-passenger`](#redmine41-passenger)
-	[`redmine:4.1.2`](#redmine412)
-	[`redmine:4.1.2-alpine`](#redmine412-alpine)
-	[`redmine:4.1.2-passenger`](#redmine412-passenger)
-	[`redmine:4.2`](#redmine42)
-	[`redmine:4.2-alpine`](#redmine42-alpine)
-	[`redmine:4.2-passenger`](#redmine42-passenger)
-	[`redmine:4.2.0`](#redmine420)
-	[`redmine:4.2.0-alpine`](#redmine420-alpine)
-	[`redmine:4.2.0-passenger`](#redmine420-passenger)
-	[`redmine:alpine`](#redminealpine)
-	[`redmine:latest`](#redminelatest)
-	[`redmine:passenger`](#redminepassenger)

## `redmine:4`

```console
$ docker pull redmine@sha256:d748e2a03c4a6c25772fe3f8349339b0e1963b1ade3c1103fa09c892f3af61fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4` - linux; amd64

```console
$ docker pull redmine@sha256:674aaf0691b263a8306a5da9ca763ea706cf9eb73fa97fe5b80880e17e34793e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.5 MB (211501364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9f9e5072432e6d9ac85838768e7d2481b91de8b79dd3010b2d77d4194e7975`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 18:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:42:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:42:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:42:59 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:55:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:56:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:56:28 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:56:28 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:56:28 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:56:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:56:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:17 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:57:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:57:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:57:17 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:57:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1596cf153142005038983af255e0d09ef62c65e139aa5c973c2d2baaa2044b0`  
		Last Modified: Sat, 10 Apr 2021 19:09:47 GMT  
		Size: 22.9 MB (22887036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed63bc8e0386fa836f8cf065b98fa401987445d1ab32e260f00e34398b353c`  
		Last Modified: Sat, 10 Apr 2021 19:09:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6acca6e42a84df58aeac107bc65a7bd29a5a702ca33992837a43d23689e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:20 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1370bc72633d9b6883d4baa5cfe7320f3310950f72f5753966432b3c5fb39af7`  
		Last Modified: Sun, 11 Apr 2021 07:03:35 GMT  
		Size: 93.9 MB (93906284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db1ff6e623ce6c864b167bcc6a6513b6864b9dc79a4d77823597370866a1c4e`  
		Last Modified: Sun, 11 Apr 2021 07:03:21 GMT  
		Size: 1.4 MB (1370219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aafa942955516a5b82908cc908e9fe16aa0e9d25e7c41513563f4d7dcd98e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de8b29a2583f478869875849b6bdc9aa17b8f1cf07835e579284513b946dba`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e2181bd63ce8a24b2330aa48fb52e8188a931903f495caaaaeb4ef6153e86`  
		Last Modified: Sun, 11 Apr 2021 07:03:18 GMT  
		Size: 3.1 MB (3057055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee7416a1645930503313e41e3183303a737aea90454566b7d83fac74e3707`  
		Last Modified: Sun, 11 Apr 2021 07:03:24 GMT  
		Size: 50.6 MB (50574847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f886f325a0ba2239c4905f09d7d6186c89f3202c59614d1181eeecf550cc69`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:c5a5d3160bd8eaf254b337f502de2c7c6eca5e533afaf87013d16ebdcc40c882
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.7 MB (215708994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94de86d41e3b7f9b9c16ef7a058e074b1b018038726598e9151d8ff64b32769f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:34:59 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 07:35:00 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 07:35:01 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 07:38:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:38:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:38:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:38:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:38:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:38:53 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:37:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 17:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:39:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:39:58 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 17:40:01 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 17:40:02 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 17:40:11 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 17:40:11 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 17:40:12 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 17:40:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 17:44:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:44:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 17:44:51 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 17:44:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:44:54 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 17:44:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da9e41f31dbd59278885fc90a21f78df54ac8e0eeaac6cdfc706d58f3e5cbf9`  
		Last Modified: Sat, 10 Apr 2021 08:12:10 GMT  
		Size: 22.1 MB (22135924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738045962dd0fa8676cf7d722f50e91453ae0e03480b28c95a78b29cbe8c1aca`  
		Last Modified: Sat, 10 Apr 2021 08:12:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce548b7edc54230ecd0be27b260538194321967b7d16ef832e6f86b36ec3269c`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4574075c1b7c50bf542b82a25936d688f4f600298ebf34638e46a49915b6cc30`  
		Last Modified: Sat, 10 Apr 2021 17:59:45 GMT  
		Size: 89.5 MB (89482026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1a552ef67d98bc5894cdb93b2a31d6b45c9ba81f13e609629c00d62d5c8cd5`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 1.3 MB (1326336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8e8040892fd65e2920ca520c1f85934ecaf3cac205140f022d26450ddb4e7`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bf7390b6a87b298e37c8f4401109ac9abaa465b693dd974b717848d0557195`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd685807e7eef49564926e681ac910583fdc0032524d07aa1e3c579701924cea`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 3.1 MB (3057047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d377f01a1044a4d648cfe27174049a37901a12adcf773b420a8cb22670008`  
		Last Modified: Sat, 10 Apr 2021 17:59:26 GMT  
		Size: 64.5 MB (64484917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9309b37c7d17afa9ab0ce43eb207cb4c015cf8080e4ef0026f3605f1d63ea4`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:9b090f6a48322643c7aa5cca725c75dbca849e6b72fb179efd17ca1c878c30a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208872054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce4cd6b1e80353141e77cb6b90438a2b128cfa0dc8b26d3541592dc0d371b4fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:30:27 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 16:30:31 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 16:30:37 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 16:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:34:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:34:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:34:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:34:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:34:51 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:36:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:38:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:38:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:38:22 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:38:23 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:38:24 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:38:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:38:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 04:38:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 04:38:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:42:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:42:29 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:42:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:42:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:42:34 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:42:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544200d357634004457e98f7ac1f43b3a31ebffce5d7e19d2ca99541f0a33131`  
		Last Modified: Sat, 10 Apr 2021 17:19:41 GMT  
		Size: 22.0 MB (22018396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9172351c62ca591dae2a838e01000b6c57489cd47d7af7562e3a495a1caf73b7`  
		Last Modified: Sat, 10 Apr 2021 17:19:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09934e285d86d86fd34b9a3e6d7dec0a3c903bc1d3876022959c6fba45f6ffbd`  
		Last Modified: Sun, 11 Apr 2021 04:57:24 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7fc62da65346ee9c7607a212b41cdbf2c0dc5e365e7c18956017fe19fed731`  
		Last Modified: Sun, 11 Apr 2021 04:57:52 GMT  
		Size: 85.5 MB (85517651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1366c02dd0228cb0f5455a819f46c01c72614c8c2c903f30d8da3f4ba7b3eae0`  
		Last Modified: Sun, 11 Apr 2021 04:57:22 GMT  
		Size: 1.3 MB (1319111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6818a0f2ed85db5a6a199a883fbf6e4eb9f5c1ec90f99cf3b39d2b304b1411`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4544ee1e1bc77a527ff800db97c53158ca440f5fa79330dc3c54988c9ef29`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17ee6b4b9725c04744e6bd790ffa5ec91622e224b5cefe433dd05838c6d7aaf`  
		Last Modified: Sun, 11 Apr 2021 04:57:22 GMT  
		Size: 3.1 MB (3057054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea24d2bc0af67d878125d29f6e1e9bd9c69e601e0796cb3d218c66e6e46bec0`  
		Last Modified: Sun, 11 Apr 2021 04:57:38 GMT  
		Size: 64.3 MB (64343712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cf6d83da71cba257a0d5c791bf2cd1d18b7188c3a7c86a1a04362ccfabf95`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:ed7bf06cf7b08eb7ffdc233007259fabb4475c75c3601ceb0c042fc87080db0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222610474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831ae1d31498a4d3370d0b2a75ac9c10ffddf9837dc3cec001c3239efc9874c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:13:06 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 16:13:06 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 16:13:07 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 16:16:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:16:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:16:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:16:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:16:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:16:56 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:36:04 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:37:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:37:31 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:37:32 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:37:33 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:37:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:37:36 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 04:37:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 04:37:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:41:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:41:39 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:41:40 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:41:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:41:42 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:41:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b735094fd3dfe6c2254ce5bc9c940f71df11fa5f06460d079afd191ebc5c674`  
		Last Modified: Sat, 10 Apr 2021 16:49:23 GMT  
		Size: 22.7 MB (22732804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe803a3eac64f3210850b0bff3533351bd47cfcfe47db8de1dfa928d38082cf8`  
		Last Modified: Sat, 10 Apr 2021 16:49:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe02df6b0d5eaba2d093335c1841a204718b89b5937988b73befc4d70e0e65`  
		Last Modified: Sun, 11 Apr 2021 04:55:42 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6b6f8722801008dc9df47485fb2c8de3e8f64b6ffea6ca55a65a322d489582`  
		Last Modified: Sun, 11 Apr 2021 04:56:08 GMT  
		Size: 92.5 MB (92499331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99372a4bd2cbe51d9628e4fb5763221c86530233759f73d039c898f2a3ef983`  
		Last Modified: Sun, 11 Apr 2021 04:55:43 GMT  
		Size: 1.3 MB (1303583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df37457b9b0458d0364314681801996540e1932316815a2d4c6c7d79e313e51`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f4312e5c8dd083d638060fae2e7c29fbc564c923dcbb0fbde7164acd157ea3`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15912641909cdcaec9376c2b88a72afe5e67c5fc2e67e597f8b3dae13f5723cf`  
		Last Modified: Sun, 11 Apr 2021 04:55:42 GMT  
		Size: 3.1 MB (3057038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf21f8a15c6087c8df6dcd1246a8bcc1fc2cb0558cdd6add076415dab67fb76`  
		Last Modified: Sun, 11 Apr 2021 04:55:55 GMT  
		Size: 65.8 MB (65845943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734c10e558c8e573d6e1113e6234bf8a61362235ff0edf48089f2d749422b434`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; 386

```console
$ docker pull redmine@sha256:a7dfbfbcd168473d1c7b59540044e9be1240a86399758af156e9bc5039d266e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217797824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11f3b67e5b83fae70ed263d4bdc62727a2556e4e6a6500b2f8b8372aa991d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:43:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 02:43:52 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 02:43:52 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 02:48:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:48:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:48:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:48:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:48:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:48:10 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:12:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 16:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:13:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:13:37 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 16:13:37 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 16:13:38 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 16:13:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 16:13:39 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 16:13:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 16:13:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 16:14:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:14:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 16:14:37 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 16:14:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 16:14:38 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 16:14:38 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab4999cad906527dc1dec3fd24fa2f63b4cf3360e33768e9a3afaa30af81f7`  
		Last Modified: Sat, 10 Apr 2021 03:12:12 GMT  
		Size: 22.3 MB (22340618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59394b3c951d09cef112094acc41fbd8608139b79afcccf38fe6ab8fa34363c`  
		Last Modified: Sat, 10 Apr 2021 03:12:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4410c086f240a2556c34f99837c171fc5042ee25324d15eed68d6c823d6f2113`  
		Last Modified: Sat, 10 Apr 2021 16:20:40 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0253065be9c93a1dd65d60739959c872d5e54b24ce0278b1b406dcd9a92fe3`  
		Last Modified: Sat, 10 Apr 2021 16:21:04 GMT  
		Size: 95.5 MB (95537702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8174da1366e0c18236b9ff292261c829c40c6f64f8754aaea0a5054378c2163b`  
		Last Modified: Sat, 10 Apr 2021 16:20:40 GMT  
		Size: 1.3 MB (1338943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a85c94e995fd573909579b7e4bc809efcc8a0cd2fa4c52de0b6934660f8f1b9`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761295a090f25492b48fbb3de84b39bcf24c6ea7d9078df49b8b3e10928eb2`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5674eb34390ddbd43c4c23b1f8c317ab1aa39d015b542ff87e8421a51373b543`  
		Last Modified: Sat, 10 Apr 2021 16:20:39 GMT  
		Size: 3.1 MB (3057038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f18b357fea8d540c87223b845dfe4481d83983e189d41dd1eda244160799c3`  
		Last Modified: Sat, 10 Apr 2021 16:20:47 GMT  
		Size: 50.5 MB (50503021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b11c79faef3e548b798c71ffda1c95254e8f0cda712a838cd6fa199162edc71`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; mips64le

```console
$ docker pull redmine@sha256:d8dfe7820f83a620ce99dd6ff63b0846ca72a25d0e9ea0cba169adfbbbfac925
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222021251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:268ae94296a68b7d47b3d70b15e8d1ddd4720476ed9027f05d0f4cae4f73290f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:06:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:16:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:16:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:16:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:16:12 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:15:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:16:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:16:56 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:16:56 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:16:57 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:16:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 19:16:59 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 19:17:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 19:17:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 19:25:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:25:13 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 19:25:13 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 19:25:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 19:25:14 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 19:25:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a308e0916de51c8816bb907b1f46847b9e4f2a4c13ad8496699a943b1cb1192b`  
		Last Modified: Sat, 10 Apr 2021 15:52:29 GMT  
		Size: 23.1 MB (23101289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4aeaf82f75e03c0de4dc8cfbada529330605924f939a89eea76608b649fc61c`  
		Last Modified: Sat, 10 Apr 2021 15:52:19 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d76e50514a47201bc1e5d1ecd34cb3dd052f552ecc3327f756a2ff28e810fd`  
		Last Modified: Sat, 10 Apr 2021 19:44:24 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9894c487a5a062ca596adb69a0c0d1787a83ea05390fc69a9508850fbd0a2aee`  
		Last Modified: Sat, 10 Apr 2021 19:45:32 GMT  
		Size: 90.9 MB (90869502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b429b96dcf10c532cff19eb56cbb9a41a6e88d65179724f8e8d0a175cb4775`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 1.3 MB (1257309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62845c559925cc0291a80649bdc3e23c43fc80a48a73be6a897e6247d616f7ef`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6114ea006b8a2dfe2a8229a601a2f01991affc3feec2a428b26707c99cc92`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866e595f4eb90b05ffa193035de32d77043c97649769baa388e8ed71df9b4c68`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 3.1 MB (3056466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff3272561a535e8b5ba73ff286d51d976cf39ac87092e2f0fa420e43c3712c`  
		Last Modified: Sat, 10 Apr 2021 19:44:56 GMT  
		Size: 66.3 MB (66298266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5a45d6e6fe63215d266dd648b78c69dc5a5ca1f462be021b884fafacfd1f9a`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; ppc64le

```console
$ docker pull redmine@sha256:613ce7722c4bcd975b4d86b7540bf3add1d5db78ea35459a83abf899bf544501
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239082666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab85f646932584743522c4882cfe4c8d378ae92ff7aea25b2022ea176204f8c6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:57:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:57:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:57:33 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:14:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:14:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:15:05 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:23:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:23:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:23:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:23:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:23:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:23:45 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 05:57:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:05:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:07:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:07:15 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:07:24 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:07:27 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:07:49 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:07:55 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:07:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:08:14 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:13:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:13:32 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:13:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:13:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:13:46 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:13:50 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cbbc810e9494a5dfcf8ee1e195a1a58bd57e76aadf8003b70553ed4eb09b2`  
		Last Modified: Sat, 10 Apr 2021 15:54:53 GMT  
		Size: 12.7 MB (12704371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa4e10ca5b1345262af0a6624b7f9980011d8180575de45104358ed122152a`  
		Last Modified: Sat, 10 Apr 2021 15:54:50 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969b8bec5707756c2c65c42151cedb5ed4aa7cfd90762da603a0c27fc694eb1e`  
		Last Modified: Sat, 10 Apr 2021 15:55:48 GMT  
		Size: 23.4 MB (23414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7799f120e744ecf4af99f5374dd470aed6475ca254813ff9b781f8bd5ee9ba`  
		Last Modified: Sat, 10 Apr 2021 15:55:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17b32b0803cb0c499e8847d76fd9c8188e04f99b0a49d3bb00fb57852da102`  
		Last Modified: Sun, 11 Apr 2021 07:07:58 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04001ba15d9c6379ed6823bd4d279724b7dc9c2c3b1779183e3d5e3cf7ced3e`  
		Last Modified: Sun, 11 Apr 2021 07:08:41 GMT  
		Size: 101.1 MB (101147239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7e01d32f1e67a82e76be158bd1f54e80d8e6d43e082bde15416b0cac68efe`  
		Last Modified: Sun, 11 Apr 2021 07:07:59 GMT  
		Size: 1.3 MB (1290574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579cddd918b5fec468e3a6b5d01ab1113193d9a60fe3f5d11de447084f315b6d`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5181bfb422524a8f6b2eace42ef46cd20f8181d2023edf01874b0d0a5f31bfe`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f706945ab1345126925f34b0a33dcd58dbd84322bd093b64077aa818112f46ee`  
		Last Modified: Sun, 11 Apr 2021 07:07:57 GMT  
		Size: 3.1 MB (3057048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c1a53028ee3ee0723cec0f90306634b171fa7905e55e906839bb7eb8601b4`  
		Last Modified: Sun, 11 Apr 2021 07:08:06 GMT  
		Size: 66.9 MB (66919035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a598556acae8e5996306debd91dadc7da82e6cc011a616f95017b1e043b4ecdb`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; s390x

```console
$ docker pull redmine@sha256:d86d5b58aa7e9dd6dc7547929ce5542856c7580dde88fb5b916c4ae6fc3cee9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222020361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89028240f1dee18298827636e792c7c5a0712b03a6445f2c4b28db0991c314e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:04:20 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 02:04:20 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 02:04:21 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 02:06:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:06:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:06:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:06:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:06:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:06:08 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:31:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 12:32:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:32:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:32:57 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 12:32:58 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 12:32:58 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 12:32:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 12:33:00 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 12:33:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 12:33:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 12:35:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:35:47 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 12:35:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 12:35:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 12:35:48 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 12:35:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3098c63e5609140d293715e979f3576527d20157d2f671592b79736f4d72ddd4`  
		Last Modified: Sat, 10 Apr 2021 02:22:38 GMT  
		Size: 23.1 MB (23066252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3547d43bbb52b78bdbe05cc38cf90175f678f4512422ef47540229443c7a1824`  
		Last Modified: Sat, 10 Apr 2021 02:22:37 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd4d29f072b64c3d7e17a9a81fe61294be125cd7f7c2fee6bddc6b5b61bafe7`  
		Last Modified: Sat, 10 Apr 2021 12:47:53 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4b26acacc50fc4a0c6155d028bde06b918cb698c1eafb066f77c98931b82ca`  
		Last Modified: Sat, 10 Apr 2021 12:48:10 GMT  
		Size: 91.6 MB (91641533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e338871896ec393957d527289b7c3ad84893f5da29ee7152a52c7cc97ccdd05a`  
		Last Modified: Sat, 10 Apr 2021 12:47:53 GMT  
		Size: 1.4 MB (1356207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24b741f8a77912f9f77062871d2a869002331460009e31de96fccbb3604b945`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db5b06d283b2c92a6908585d05e13858d8561b7c61b9c190de9807cd4bf05e4`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e29c0ae231298e90eea6df8a140e4608cff7d379598e181106f9b4de31a517`  
		Last Modified: Sat, 10 Apr 2021 12:47:52 GMT  
		Size: 3.1 MB (3057042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22351124edd3ea56412ba14138a1aafc8eb76b8f7b72842596372b3b8dbf3088`  
		Last Modified: Sat, 10 Apr 2021 12:48:02 GMT  
		Size: 66.3 MB (66327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea92b2f8e559d76b1121c336a586e7884919cb81519ff911a84e78a1e98194`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:29454a31d1cebcdc33cd50b35495532b6756e6608a036133c68263de8089b9a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:9d1c434ac62026273ff39820aad3eb9e532678a54012152712ab1a76311a8139
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.3 MB (164260126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5aa389f0b143c0ea7e350e485f5936594d02e5f31ee239353156b2609330376`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:39:43 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 10:39:45 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:47:42 GMT
ENV RUBY_MAJOR=2.7
# Mon, 05 Apr 2021 19:16:34 GMT
ENV RUBY_VERSION=2.7.3
# Mon, 05 Apr 2021 19:16:34 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Mon, 05 Apr 2021 19:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:20:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:20:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:20:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:21:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:21:02 GMT
CMD ["irb"]
# Mon, 05 Apr 2021 20:44:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Mon, 05 Apr 2021 20:44:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Mon, 05 Apr 2021 20:44:49 GMT
ENV RAILS_ENV=production
# Mon, 05 Apr 2021 20:44:49 GMT
WORKDIR /usr/src/redmine
# Mon, 05 Apr 2021 20:44:49 GMT
ENV HOME=/home/redmine
# Mon, 05 Apr 2021 20:44:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 05 Apr 2021 20:44:51 GMT
ENV REDMINE_VERSION=4.2.0
# Mon, 05 Apr 2021 20:44:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Mon, 05 Apr 2021 20:44:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 05 Apr 2021 20:44:55 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 05 Apr 2021 20:47:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 05 Apr 2021 20:47:14 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 05 Apr 2021 20:47:14 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 05 Apr 2021 20:47:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 05 Apr 2021 20:47:15 GMT
EXPOSE 3000
# Mon, 05 Apr 2021 20:47:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9df2de4dab84e51acacca9e65a3d9f7c9fa2f038bc11c2830bd9a97980823a0`  
		Last Modified: Thu, 01 Apr 2021 11:09:32 GMT  
		Size: 1.2 MB (1218696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc339b259bb6448a756fb9b42044f3450a7dcd6fc3bc0102a3cb6b7594daca19`  
		Last Modified: Thu, 01 Apr 2021 11:09:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bf4c0832c8a73d79344879220b7a99ed4ecccf6eb758384bec64d8719c63b8`  
		Last Modified: Mon, 05 Apr 2021 20:15:04 GMT  
		Size: 23.2 MB (23207724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e0141082ecc3e69444f52c2c25989a96c26e3f1db52ed818a2415be78f134a`  
		Last Modified: Mon, 05 Apr 2021 20:15:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed39d01534357156db6127eb2e8773b4392a8e1f7eeda26f6ee1e2a8e546bab7`  
		Last Modified: Mon, 05 Apr 2021 20:58:52 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a15e47cfeac0ace560ab1a638fc48e9778fd707f93c1e1f0f5ce10485c02ff`  
		Last Modified: Mon, 05 Apr 2021 20:59:04 GMT  
		Size: 69.4 MB (69428125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e444a04c0290dbedcaf3c8c2b51834f611b133a5d3972177b6cf6e8a7a8bd26`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d2998285fcc9b3ccd853c688ece46d699af9032ff15b3ce80d713c179b9ca2`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0bf3df829a8a10618bbfe5772d98aeda38ab59effc18261703062cb5ade296`  
		Last Modified: Mon, 05 Apr 2021 20:58:50 GMT  
		Size: 3.1 MB (3058322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1c7fbf7457fdf8ee116d68493251899d90f8b5d5f7ae60fbcdb6f2580965ec`  
		Last Modified: Mon, 05 Apr 2021 20:58:56 GMT  
		Size: 64.5 MB (64531585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ebb1f89b905c30adc636a07475d0f7e1720a4b3cc15d4ea8e30ab637c91b7e`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:fb65384f72d4cdfdde814d4251c875f18a880266352429b55ebd579d4c173ee0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:c079166ff4bd19c8ad9336912641f489b7354401437cd7acee04999530650477
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236801276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f9c99e9a97ac10f42e489199a62f16eb28ae8368a638cd41ad31ecf1c6e5be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 18:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:42:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:42:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:42:59 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:55:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:56:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:56:28 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:56:28 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:56:28 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:56:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:56:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:17 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:57:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:57:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:57:17 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:57:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sun, 11 Apr 2021 06:57:33 GMT
ENV PASSENGER_VERSION=6.0.8
# Sun, 11 Apr 2021 06:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:50 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sun, 11 Apr 2021 06:57:50 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sun, 11 Apr 2021 06:57:50 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1596cf153142005038983af255e0d09ef62c65e139aa5c973c2d2baaa2044b0`  
		Last Modified: Sat, 10 Apr 2021 19:09:47 GMT  
		Size: 22.9 MB (22887036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed63bc8e0386fa836f8cf065b98fa401987445d1ab32e260f00e34398b353c`  
		Last Modified: Sat, 10 Apr 2021 19:09:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6acca6e42a84df58aeac107bc65a7bd29a5a702ca33992837a43d23689e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:20 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1370bc72633d9b6883d4baa5cfe7320f3310950f72f5753966432b3c5fb39af7`  
		Last Modified: Sun, 11 Apr 2021 07:03:35 GMT  
		Size: 93.9 MB (93906284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db1ff6e623ce6c864b167bcc6a6513b6864b9dc79a4d77823597370866a1c4e`  
		Last Modified: Sun, 11 Apr 2021 07:03:21 GMT  
		Size: 1.4 MB (1370219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aafa942955516a5b82908cc908e9fe16aa0e9d25e7c41513563f4d7dcd98e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de8b29a2583f478869875849b6bdc9aa17b8f1cf07835e579284513b946dba`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e2181bd63ce8a24b2330aa48fb52e8188a931903f495caaaaeb4ef6153e86`  
		Last Modified: Sun, 11 Apr 2021 07:03:18 GMT  
		Size: 3.1 MB (3057055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee7416a1645930503313e41e3183303a737aea90454566b7d83fac74e3707`  
		Last Modified: Sun, 11 Apr 2021 07:03:24 GMT  
		Size: 50.6 MB (50574847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f886f325a0ba2239c4905f09d7d6186c89f3202c59614d1181eeecf550cc69`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4e67ce39214f6c91a2e674f89f56c6396296fe4ae2975f2dc24082bfa2db9f`  
		Last Modified: Sun, 11 Apr 2021 07:03:56 GMT  
		Size: 20.4 MB (20363201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd0141a3a34bc643ef0b1a5907467d3643479f4c5bb357ffb15dbff0a695a22`  
		Last Modified: Sun, 11 Apr 2021 07:03:54 GMT  
		Size: 4.9 MB (4936711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0`

```console
$ docker pull redmine@sha256:bee60ae90f25fe39ab6994198d30dc5c5f868958a6b9c6511f708e788dac2ec7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.0` - linux; amd64

```console
$ docker pull redmine@sha256:2a1bd94200c344c25107cbbe34c7f52b6c8b681976a7f066dc264747aa425e83
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.2 MB (206177855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a1eb018c1188212be6ab93e61470b7b1ef152ed52766c08e56a186cdc60a25`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 07:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 07:00:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:00:22 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 07:00:22 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 07:00:22 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 07:00:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 07:00:23 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 07:00:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 07:00:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 07:02:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:02:12 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 07:02:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 07:02:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 07:02:12 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 07:02:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d7e3f1a32c6de0dd372c7905837938a00bf39ab4fcdf748828c4935073551`  
		Last Modified: Sun, 11 Apr 2021 07:04:17 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66743655a9623d68938cfd2efa15e72fb70ce962094fb3c79e40b4408b4e0d1b`  
		Last Modified: Sun, 11 Apr 2021 07:05:19 GMT  
		Size: 81.0 MB (81020804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2861ed67e9e65e0194f1809af11356a997d4ef594e1771b8db9f30fc27f9cc22`  
		Last Modified: Sun, 11 Apr 2021 07:05:07 GMT  
		Size: 1.4 MB (1356453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd99b3be78435843199962828c2bf524d28bfd5123cbadbe79a88aebcacff54`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46277daa4e0232f5f265213bdf13fe3f6fa33c11303e762754b3f6c5a3d67404`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f2bf905d64fdc0678fa13c72441ce49310b8d7d35b2cbf4a5fef981b63436f`  
		Last Modified: Sun, 11 Apr 2021 07:05:04 GMT  
		Size: 2.5 MB (2541667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bd12f0c8e81c2201227718b39054718d424aa01620d6558b0f6f8097968796`  
		Last Modified: Sun, 11 Apr 2021 07:05:15 GMT  
		Size: 60.1 MB (60085642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e702d6f9980e3173128449df698c15765b1dc2208f84fa6e86ffcbb503fb68`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:61d09125ec31a1ca6420fcb1b46ef088ec26d1d982122fe2462885387f6024fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.9 MB (195857954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0985f50db4caa7b7c67e1c0b3bf8b5451e3400aca45da88852757acecbc1c1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:42:11 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 07:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:45:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:45:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:45:55 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:45:11 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 17:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:53:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:53:51 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 17:53:52 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 17:53:52 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 17:53:57 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 17:53:58 GMT
ENV REDMINE_VERSION=4.0.8
# Sat, 10 Apr 2021 17:53:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sat, 10 Apr 2021 17:54:05 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 17:58:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:58:45 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 17:58:46 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 17:58:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:58:49 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 17:58:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f63c1e0d3af67924d2d3ef5636ed70900748b90fffc5bf4e748a38ef7d125`  
		Last Modified: Sat, 10 Apr 2021 08:12:41 GMT  
		Size: 20.7 MB (20732839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9ef980b82778a927138ed4192338fea82cdb79fe3d25e26ac958cc5dc33d62`  
		Last Modified: Sat, 10 Apr 2021 08:12:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e44c16e94e3b1dbd69e19de696cd7efbdfba7b0dce4839c9cc84d00723baf0`  
		Last Modified: Sat, 10 Apr 2021 18:00:05 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c89f5fc34f9483ba7e47ec017c35bb676b60da7741e6bad709bc7fdefae84ff`  
		Last Modified: Sat, 10 Apr 2021 18:01:14 GMT  
		Size: 76.9 MB (76861581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee37976bcb7dae0210c9778b746e1f691c1596086da7a80e35d5875518742cf`  
		Last Modified: Sat, 10 Apr 2021 18:00:50 GMT  
		Size: 1.3 MB (1315113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee876c751e57427a82e3fc88949c5979019da1bccd76fe8ac5d1a689cd2d93d8`  
		Last Modified: Sat, 10 Apr 2021 18:00:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af19d44e71a574d596d347d5fe6f9cbeba87ba0bcc4bbe1501c8c9a023f5fac3`  
		Last Modified: Sat, 10 Apr 2021 18:00:48 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d0869083c1f98b291e8d414c9fe3a5eaf3b65fc243570dd364e738f60c8329`  
		Last Modified: Sat, 10 Apr 2021 18:00:49 GMT  
		Size: 2.5 MB (2541672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9535d688965d325fc9df3bbad4751621b1c787c9596d76b715bec37735e71b`  
		Last Modified: Sat, 10 Apr 2021 18:01:02 GMT  
		Size: 59.2 MB (59184008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839254017393f3fa7519521037c5ffc30ba3921adec999522ee5f588ba46f08`  
		Last Modified: Sat, 10 Apr 2021 18:00:48 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:8a3a5e24ade51015ef2dc3cd63769f1dea40ca4e35c144f0bd3b276c75418da0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.2 MB (189232714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e45c68fdcd14c809057951978490cdfaffc55b4dc779ca9d8b3bd3e15ee144d5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:49:54 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:49:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:49:57 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:53:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:53:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:53:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:53:49 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:42:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:51:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:51:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:51:46 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:51:51 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:51:52 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:51:58 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:52:00 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 04:52:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 04:52:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:56:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:56:55 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:56:56 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:56:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:56:58 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:56:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae68a3a282a83d0e6da8b00595a45c9fb467b44e46970f00dee3a849e860c81c`  
		Last Modified: Sat, 10 Apr 2021 17:20:12 GMT  
		Size: 20.6 MB (20643582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b299ede54fe617996860ca241d888ae39341d21408e0f7e892ef71dea23ee3`  
		Last Modified: Sat, 10 Apr 2021 17:20:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac4b477683229835feada0995794aaeeee3d978e339a0c29e31b5401fdc5ca`  
		Last Modified: Sun, 11 Apr 2021 04:58:14 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3990681ca7a1c562915fdecf77cdccf54cfdda6eb931027cecdee6c4f85659c7`  
		Last Modified: Sun, 11 Apr 2021 04:59:21 GMT  
		Size: 73.2 MB (73204168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd53e50d67fdc8a6e2a79bd97066ccbce4dd59fc1f60100d558c21944dadaf8`  
		Last Modified: Sun, 11 Apr 2021 04:58:59 GMT  
		Size: 1.3 MB (1305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928bb957c6b08625c811b507ea4a97eb32ac5aa2ac0852c8ae47030ecb485`  
		Last Modified: Sun, 11 Apr 2021 04:58:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4873f8c056cc4bfca6960b68718220581ab216d6b9727bde045389a588f0d0f7`  
		Last Modified: Sun, 11 Apr 2021 04:58:57 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f67089eac0e1b6944494f80ecaff256a775a221dcd47e39690543da90ffb8d`  
		Last Modified: Sun, 11 Apr 2021 04:58:58 GMT  
		Size: 2.5 MB (2541659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb430435f743b101667bef7564a03cc96f556ccd1c6f3dc94e29dbacc84305b`  
		Last Modified: Sun, 11 Apr 2021 04:59:11 GMT  
		Size: 58.9 MB (58921665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40735fa79b3ebc2e47ddfe4becc86813e59d735ec18e73087019cb2635945121`  
		Last Modified: Sun, 11 Apr 2021 04:58:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:5eb881676d38f6af2fe269977b09833145a7b2898db63417670531cb12758fde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.0 MB (201957441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bfce45df8c4a75b15c77d4990f6749994006f014ec692f10cb9c7ce7897fac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:20:43 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:20:49 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:20:50 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:24:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:24:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:24:38 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:41:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:49:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:49:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:49:32 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:49:34 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:49:35 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:49:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:49:40 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 04:49:42 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 04:49:49 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:55:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:55:07 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:55:09 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:55:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:55:12 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:55:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805a70932a287839e4483317925d47a504efbbe434fde5824ef4192898e352e2`  
		Last Modified: Sat, 10 Apr 2021 16:50:01 GMT  
		Size: 21.3 MB (21308477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f9a34f968a2b1af6ba62fe49a0831f817c21182613ab38a0633bf356c0cf23`  
		Last Modified: Sat, 10 Apr 2021 16:49:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ececbf89e390256b43a15f33c53615e9029553b1726dffad48507d7138213a6`  
		Last Modified: Sun, 11 Apr 2021 04:56:21 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cc8027e85bd9d41b2f186cd6ad07efbe7f8da82390b5c4d8de6f78021bc759`  
		Last Modified: Sun, 11 Apr 2021 04:57:16 GMT  
		Size: 79.6 MB (79640373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e692a5b9422d5c10fe5cce66c63ae5bf9a69783134d2a2af1002f3c908d078ad`  
		Last Modified: Sun, 11 Apr 2021 04:56:57 GMT  
		Size: 1.3 MB (1291820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ece293a5e59922b35ae9fddc3da48953f17cbaa854812ae86f4c761465b639c`  
		Last Modified: Sun, 11 Apr 2021 04:56:55 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd66c8fcd8111228dadd5a92532739e995d7f5ed8718eb53f2d6bf3cfaaa2ffa`  
		Last Modified: Sun, 11 Apr 2021 04:56:55 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95678d3d349f52fb12f61ee024aaf7d2f5308fa582c487cc33d5219c004b54cf`  
		Last Modified: Sun, 11 Apr 2021 04:56:58 GMT  
		Size: 2.5 MB (2541675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4337c75954970548b54020a8f86710b389ee763d43ab30dedb3fe1552d7d2bcf`  
		Last Modified: Sun, 11 Apr 2021 04:57:06 GMT  
		Size: 60.0 MB (60003321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c567294b3f7a69dedebbb90bde1cd921b46d461b3f2c76499fd257c990e6ad2d`  
		Last Modified: Sun, 11 Apr 2021 04:56:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; 386

```console
$ docker pull redmine@sha256:96069edc4e4d04e68d45c29178395c155fd991d071d364c16a39063cb6378630
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.4 MB (211425618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0668a7b02f442b188b66272ab162d691f57f04c279d0f37fcc6ca70fcd97c4b4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:52:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:52:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:52:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:52:19 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:14:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 16:17:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:17:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:17:16 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 16:17:16 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 16:17:16 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 16:17:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 16:17:17 GMT
ENV REDMINE_VERSION=4.0.8
# Sat, 10 Apr 2021 16:17:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sat, 10 Apr 2021 16:17:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 16:19:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:19:56 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 16:19:56 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 16:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 16:19:56 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 16:19:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207aa5aba20825c04fb847653d3cf6d5011040c7f7b8147ce0824ebda58d682`  
		Last Modified: Sat, 10 Apr 2021 03:13:02 GMT  
		Size: 20.9 MB (20909318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5e3665a3fdb3774edce1b87e369d385982d95b3f12169b947249c7ecb6566`  
		Last Modified: Sat, 10 Apr 2021 03:12:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c61c4b79a951b1b483b330e6fa809e988bab5ec193531c977e7c39ce6fa6fa`  
		Last Modified: Sat, 10 Apr 2021 16:21:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488d2ea51179d8da50447ec20ceb69ff3cbb1ca84b11ffe0524c48984e5859d2`  
		Last Modified: Sat, 10 Apr 2021 16:22:26 GMT  
		Size: 82.4 MB (82437500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a8f287298504a3aa8010a144f1daf33313922972e3e6cc27b60c6f32598ca3`  
		Last Modified: Sat, 10 Apr 2021 16:22:06 GMT  
		Size: 1.3 MB (1327322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57538301434f4789ac2c33becf9c072f47849d6bb28e483602c979dcbfdf5c`  
		Last Modified: Sat, 10 Apr 2021 16:22:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5989dfc48bca16aa4cc9559c74a5894dce06ccd6f9f0a1d9bee163857e060c`  
		Last Modified: Sat, 10 Apr 2021 16:22:04 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e117ff45b4482fa69c393342a1e6d5e0aa244a1e3e637bb7acc5691b3fb289cc`  
		Last Modified: Sat, 10 Apr 2021 16:22:05 GMT  
		Size: 2.5 MB (2541674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fdabe362e26b82776cc039f91365dafb45cce29a37309b6524fc5415289541`  
		Last Modified: Sat, 10 Apr 2021 16:22:14 GMT  
		Size: 59.2 MB (59189302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc72e552a747a702d1664614f7e3408e56827f3738008af7887f372b311e801`  
		Last Modified: Sat, 10 Apr 2021 16:22:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; mips64le

```console
$ docker pull redmine@sha256:8738baa7a2937d7502e62817bc2530701f825c2a0987e2a88f2ef98f75e2b672
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.2 MB (201176539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7c2189ac46bef43f27812d17e3f3af2026801613c2330b819c344bd68ad56`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:24:25 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 15:24:25 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 15:24:26 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 15:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:32:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:32:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:32:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:32:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:33:00 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:25:30 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:36:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:36:45 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:36:46 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:36:46 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:36:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 19:36:49 GMT
ENV REDMINE_VERSION=4.0.8
# Sat, 10 Apr 2021 19:36:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sat, 10 Apr 2021 19:36:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 19:43:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:43:57 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 19:43:58 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 19:43:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 19:43:59 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 19:43:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6a8b6e14ae4c50de74d8a7225fdb08536fc034f6994e460e0f9d6476b068a3`  
		Last Modified: Sat, 10 Apr 2021 15:53:23 GMT  
		Size: 21.7 MB (21661143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af10c60efa418c61d498b86b823d73662484fc921d24b76362fa7c8a1d716be`  
		Last Modified: Sat, 10 Apr 2021 15:53:14 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a88a9e837e51dc5511791e1410d11311dca9f231f8f6120d1160d240ae957b`  
		Last Modified: Sat, 10 Apr 2021 19:45:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cf8215a8716b3e15c8bd3aad48bdf15c21385de589012a3eb76dc0f2a37908`  
		Last Modified: Sat, 10 Apr 2021 19:48:12 GMT  
		Size: 78.1 MB (78139675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e13e07952c904491e48b6dda1750654d334aa9dd35919df91a5aa6e625fbc74`  
		Last Modified: Sat, 10 Apr 2021 19:47:16 GMT  
		Size: 1.2 MB (1244216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b46e972b003bc2193bbd0639e08d48952993d3a035e9b190b6bbb785eb22a87`  
		Last Modified: Sat, 10 Apr 2021 19:47:12 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a955ff4dd91d61cab4d30e90b580f30be55c5fbcdeb05ea260cf5793f07d83`  
		Last Modified: Sat, 10 Apr 2021 19:47:12 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46931f792b62001c6927e4d3c143e93885ff850343d25b0aa64e86ee31476cb2`  
		Last Modified: Sat, 10 Apr 2021 19:47:16 GMT  
		Size: 2.5 MB (2541151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de1b7a80b6a4eaa3cf8f53bd71f995562bad3c079a37977b9bdc8221cddae9`  
		Last Modified: Sat, 10 Apr 2021 19:47:45 GMT  
		Size: 60.2 MB (60151932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b39d2e83bc8ab6475b6620a745e238da82b66b8a85d1d5f35f30ff64ba68601`  
		Last Modified: Sat, 10 Apr 2021 19:47:12 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:9f1f3e0d7846ad7b474ffc99f3892dd65363565fb53d02289d684c2cb71a4995
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217504698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e59a6b27b14fd14a8dc6ea9a129337ce0b677130cfa55399a427267e86c17bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:57:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:57:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:57:33 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:27:53 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 15:27:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 15:28:01 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 15:35:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:35:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:35:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:35:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:35:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:36:11 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:14:19 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:51:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:51:51 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:52:02 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:52:15 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:52:49 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:53:02 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 06:53:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 06:53:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 07:07:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:07:10 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 07:07:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 07:07:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 07:07:20 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 07:07:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cbbc810e9494a5dfcf8ee1e195a1a58bd57e76aadf8003b70553ed4eb09b2`  
		Last Modified: Sat, 10 Apr 2021 15:54:53 GMT  
		Size: 12.7 MB (12704371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa4e10ca5b1345262af0a6624b7f9980011d8180575de45104358ed122152a`  
		Last Modified: Sat, 10 Apr 2021 15:54:50 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0266f29c4d0be5f1d382e9ff0a02f03fb96494b3d6e0fc30c71ea410f72c0`  
		Last Modified: Sat, 10 Apr 2021 15:56:30 GMT  
		Size: 22.0 MB (21984924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168d7a83cd3ffcd313c7d046285a1eabaaba553d590844df3ee3cbd7648a2c9`  
		Last Modified: Sat, 10 Apr 2021 15:56:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb092c4cd4d038d1b22d42c5079bbf5d4f101cd8e63a587f6104ece43b205bba`  
		Last Modified: Sun, 11 Apr 2021 07:09:01 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c147cc6419922fa988f9638c830159a176b9c956096d08120ce71e236f7911e7`  
		Last Modified: Sun, 11 Apr 2021 07:09:57 GMT  
		Size: 87.7 MB (87746565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6b309da6e581e596c7919fd5b8423b0cd3905601300ab84981071ee10a26e6`  
		Last Modified: Sun, 11 Apr 2021 07:09:39 GMT  
		Size: 1.3 MB (1276387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ece19dff96976adb31b39d5c2c163e80d594dbba168094a110a1d7cdd75dad6`  
		Last Modified: Sun, 11 Apr 2021 07:09:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bc115d8d040dd4b647aab0f01c637065b90cac0e00b03ccedfd73bf7ebce67`  
		Last Modified: Sun, 11 Apr 2021 07:09:36 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79d8a41917f2e428d12487247fba2c52c08cd20e762aa00c622acf3b2243d3c`  
		Last Modified: Sun, 11 Apr 2021 07:09:37 GMT  
		Size: 2.5 MB (2541674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a028db1877457828483431f599c3c02e11413bbe1895790b488c5b7891874e45`  
		Last Modified: Sun, 11 Apr 2021 07:09:46 GMT  
		Size: 60.7 MB (60700588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a16a0038c282eb456758805cfb035e9480cc62e8b43629ebdec3a5b5751fda`  
		Last Modified: Sun, 11 Apr 2021 07:09:36 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; s390x

```console
$ docker pull redmine@sha256:ad9baf8ca388ec8d53aeceee13fdcfde3a5863875dd563b426b2d363f6648823
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201369506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d4f2b8e63dc709509807105e97793dbc83e8ac03b337e5554a0d6693cbf2a9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:17:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:17:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:17:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:17:20 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:36:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 12:42:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:43:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:43:06 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 12:43:07 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 12:43:08 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 12:43:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 12:43:10 GMT
ENV REDMINE_VERSION=4.0.8
# Sat, 10 Apr 2021 12:43:11 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sat, 10 Apr 2021 12:43:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 12:47:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:47:25 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 12:47:26 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 12:47:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 12:47:27 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 12:47:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f085c8813292ca999ce489985962c48c430c2055b5e583be1f6f4e0dfd5353`  
		Last Modified: Sat, 10 Apr 2021 02:22:58 GMT  
		Size: 21.6 MB (21618739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea955664e86a3a2fc2a4765705d82563887aaa4c51dd1b6de0ad1d783561ee90`  
		Last Modified: Sat, 10 Apr 2021 02:22:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caafc17bfb9bef6d20a4d1bee71743fdc15a7b73de616c69b477f48c1140d05`  
		Last Modified: Sat, 10 Apr 2021 12:48:23 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3971b7397a8d2b592596fa5005416be4c47904803edbc7c6003f1639e90680ff`  
		Last Modified: Sat, 10 Apr 2021 12:49:08 GMT  
		Size: 78.8 MB (78776229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024030ae4ad30ae8062177468e6f0fc42e845f4b2f83a044f5e8f74123c90e9c`  
		Last Modified: Sat, 10 Apr 2021 12:48:54 GMT  
		Size: 1.3 MB (1342620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75216f044269d86b8d4ec63782f2b474d58e3d7d960cd14f60b68ee654ad782e`  
		Last Modified: Sat, 10 Apr 2021 12:48:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385328e9e2cb30103ce68dbaffa561af084effdb23444698761c9cf9844f145c`  
		Last Modified: Sat, 10 Apr 2021 12:48:51 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1153191d2cb5ac6078ed551e10ca8ef67371cfb9f4aad2f378b8d6507cb986ec`  
		Last Modified: Sat, 10 Apr 2021 12:48:52 GMT  
		Size: 2.5 MB (2541667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60fc43d39d62022c7a591cc115af38cb818ead6bc760d9dad8e0f53f7a1a0ba`  
		Last Modified: Sat, 10 Apr 2021 12:49:01 GMT  
		Size: 60.5 MB (60517943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806bf7f576d6dac5d3f6d9e8425df03c396f71c5e789b6e7a227d550be60da8e`  
		Last Modified: Sat, 10 Apr 2021 12:48:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-alpine`

```console
$ docker pull redmine@sha256:8a11b8b550012b7c4cbbd59395c4c9e9e555b07236320391b78d6b520467e13a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:90b7600c4aff4f071d854964035266096766456e349bfadf4ee7806046aa93f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.3 MB (153335497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c1028c79f4b7526e4dfa853b0f422b7ed1fb3a5063aaf444f66fc19bd6fffc1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:39:43 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 10:39:45 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:55:16 GMT
ENV RUBY_MAJOR=2.6
# Mon, 05 Apr 2021 19:40:49 GMT
ENV RUBY_VERSION=2.6.7
# Mon, 05 Apr 2021 19:40:49 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Mon, 05 Apr 2021 19:45:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:45:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:45:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:45:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:45:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:45:05 GMT
CMD ["irb"]
# Mon, 05 Apr 2021 20:49:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Mon, 05 Apr 2021 20:55:37 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Mon, 05 Apr 2021 20:55:37 GMT
ENV RAILS_ENV=production
# Mon, 05 Apr 2021 20:55:38 GMT
WORKDIR /usr/src/redmine
# Mon, 05 Apr 2021 20:55:38 GMT
ENV HOME=/home/redmine
# Mon, 05 Apr 2021 20:55:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 05 Apr 2021 20:55:39 GMT
ENV REDMINE_VERSION=4.0.8
# Mon, 05 Apr 2021 20:55:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Mon, 05 Apr 2021 20:55:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 05 Apr 2021 20:55:43 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 05 Apr 2021 20:57:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 05 Apr 2021 20:57:18 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 05 Apr 2021 20:57:18 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 05 Apr 2021 20:57:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 05 Apr 2021 20:57:19 GMT
EXPOSE 3000
# Mon, 05 Apr 2021 20:57:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9df2de4dab84e51acacca9e65a3d9f7c9fa2f038bc11c2830bd9a97980823a0`  
		Last Modified: Thu, 01 Apr 2021 11:09:32 GMT  
		Size: 1.2 MB (1218696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc339b259bb6448a756fb9b42044f3450a7dcd6fc3bc0102a3cb6b7594daca19`  
		Last Modified: Thu, 01 Apr 2021 11:09:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50912dd8ac3c72a63b47d2ea4938ce0d0b540b3d281b6e7afde7431b771f7821`  
		Last Modified: Mon, 05 Apr 2021 20:16:47 GMT  
		Size: 21.8 MB (21839400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d6f19cafc240eb97d8d85ce13604a63ae1302240377da30f1da030a381871f`  
		Last Modified: Mon, 05 Apr 2021 20:16:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e42f435c0bb598a2d54e4d1abb1e2433c64bd72e903564a32209b96271fdbd1`  
		Last Modified: Mon, 05 Apr 2021 21:00:16 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052fd31a2728992bf069a7683e900c63361022a28130f178ecf37313bd21d422`  
		Last Modified: Mon, 05 Apr 2021 21:01:41 GMT  
		Size: 66.1 MB (66075620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80bea3abebec9cc2134e12e98f1ab38c146536b99f32663f151cd41f2cb212`  
		Last Modified: Mon, 05 Apr 2021 21:01:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1beb398278d5829cee76d372b79ca33d82c06e64428bf5b5213651f482973c2d`  
		Last Modified: Mon, 05 Apr 2021 21:01:24 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab61081e09c9755e45525b209fb625aac5ce72b7a4f1a0d38db5bdcbc94bde3f`  
		Last Modified: Mon, 05 Apr 2021 21:01:25 GMT  
		Size: 2.5 MB (2543099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3745ef83cee6de7a9dc13f726fcba8f0a9eb464fde25414699ff12415bc34b2d`  
		Last Modified: Mon, 05 Apr 2021 21:01:31 GMT  
		Size: 58.8 MB (58843006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baed54af0e0b00be44b1b6aa25e915b79468d85bf7f7f2a0e0cffa1979684aa2`  
		Last Modified: Mon, 05 Apr 2021 21:01:24 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-passenger`

```console
$ docker pull redmine@sha256:41e4bafd59e8ca296c50879d573f0cbd20fea6a22bfe167e05776117a8c4504f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:daafacdf3abafd2e54870eceb6140e779419d89a1f2379530b9687bbaf6c68c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231467473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2883b123c919a0ae57fadef7afcdadaf2d6dd2767de9b607bbbe1a383cc506ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 07:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 07:00:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:00:22 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 07:00:22 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 07:00:22 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 07:00:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 07:00:23 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 07:00:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 07:00:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 07:02:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:02:12 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 07:02:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 07:02:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 07:02:12 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 07:02:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sun, 11 Apr 2021 07:02:28 GMT
ENV PASSENGER_VERSION=6.0.8
# Sun, 11 Apr 2021 07:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:02:46 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sun, 11 Apr 2021 07:02:46 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sun, 11 Apr 2021 07:02:46 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d7e3f1a32c6de0dd372c7905837938a00bf39ab4fcdf748828c4935073551`  
		Last Modified: Sun, 11 Apr 2021 07:04:17 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66743655a9623d68938cfd2efa15e72fb70ce962094fb3c79e40b4408b4e0d1b`  
		Last Modified: Sun, 11 Apr 2021 07:05:19 GMT  
		Size: 81.0 MB (81020804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2861ed67e9e65e0194f1809af11356a997d4ef594e1771b8db9f30fc27f9cc22`  
		Last Modified: Sun, 11 Apr 2021 07:05:07 GMT  
		Size: 1.4 MB (1356453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd99b3be78435843199962828c2bf524d28bfd5123cbadbe79a88aebcacff54`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46277daa4e0232f5f265213bdf13fe3f6fa33c11303e762754b3f6c5a3d67404`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f2bf905d64fdc0678fa13c72441ce49310b8d7d35b2cbf4a5fef981b63436f`  
		Last Modified: Sun, 11 Apr 2021 07:05:04 GMT  
		Size: 2.5 MB (2541667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bd12f0c8e81c2201227718b39054718d424aa01620d6558b0f6f8097968796`  
		Last Modified: Sun, 11 Apr 2021 07:05:15 GMT  
		Size: 60.1 MB (60085642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e702d6f9980e3173128449df698c15765b1dc2208f84fa6e86ffcbb503fb68`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d96e78e20fe93a6e3de8b1f405bfac07a1fb431e911c2261eb33673b6341a1`  
		Last Modified: Sun, 11 Apr 2021 07:05:33 GMT  
		Size: 20.4 MB (20352904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f2124ce9e6dbe37feeb5ae18cac7fbbc7dbf0ec4536b9d7ef6f50187b493a4`  
		Last Modified: Sun, 11 Apr 2021 07:05:31 GMT  
		Size: 4.9 MB (4936714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.8`

```console
$ docker pull redmine@sha256:bee60ae90f25fe39ab6994198d30dc5c5f868958a6b9c6511f708e788dac2ec7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.0.8` - linux; amd64

```console
$ docker pull redmine@sha256:2a1bd94200c344c25107cbbe34c7f52b6c8b681976a7f066dc264747aa425e83
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.2 MB (206177855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a1eb018c1188212be6ab93e61470b7b1ef152ed52766c08e56a186cdc60a25`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 07:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 07:00:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:00:22 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 07:00:22 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 07:00:22 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 07:00:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 07:00:23 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 07:00:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 07:00:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 07:02:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:02:12 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 07:02:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 07:02:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 07:02:12 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 07:02:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d7e3f1a32c6de0dd372c7905837938a00bf39ab4fcdf748828c4935073551`  
		Last Modified: Sun, 11 Apr 2021 07:04:17 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66743655a9623d68938cfd2efa15e72fb70ce962094fb3c79e40b4408b4e0d1b`  
		Last Modified: Sun, 11 Apr 2021 07:05:19 GMT  
		Size: 81.0 MB (81020804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2861ed67e9e65e0194f1809af11356a997d4ef594e1771b8db9f30fc27f9cc22`  
		Last Modified: Sun, 11 Apr 2021 07:05:07 GMT  
		Size: 1.4 MB (1356453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd99b3be78435843199962828c2bf524d28bfd5123cbadbe79a88aebcacff54`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46277daa4e0232f5f265213bdf13fe3f6fa33c11303e762754b3f6c5a3d67404`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f2bf905d64fdc0678fa13c72441ce49310b8d7d35b2cbf4a5fef981b63436f`  
		Last Modified: Sun, 11 Apr 2021 07:05:04 GMT  
		Size: 2.5 MB (2541667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bd12f0c8e81c2201227718b39054718d424aa01620d6558b0f6f8097968796`  
		Last Modified: Sun, 11 Apr 2021 07:05:15 GMT  
		Size: 60.1 MB (60085642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e702d6f9980e3173128449df698c15765b1dc2208f84fa6e86ffcbb503fb68`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.8` - linux; arm variant v5

```console
$ docker pull redmine@sha256:61d09125ec31a1ca6420fcb1b46ef088ec26d1d982122fe2462885387f6024fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.9 MB (195857954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e0985f50db4caa7b7c67e1c0b3bf8b5451e3400aca45da88852757acecbc1c1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:42:11 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 07:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:45:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:45:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:45:55 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:45:11 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 17:53:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:53:50 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:53:51 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 17:53:52 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 17:53:52 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 17:53:57 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 17:53:58 GMT
ENV REDMINE_VERSION=4.0.8
# Sat, 10 Apr 2021 17:53:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sat, 10 Apr 2021 17:54:05 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 17:58:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:58:45 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 17:58:46 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 17:58:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:58:49 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 17:58:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f63c1e0d3af67924d2d3ef5636ed70900748b90fffc5bf4e748a38ef7d125`  
		Last Modified: Sat, 10 Apr 2021 08:12:41 GMT  
		Size: 20.7 MB (20732839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9ef980b82778a927138ed4192338fea82cdb79fe3d25e26ac958cc5dc33d62`  
		Last Modified: Sat, 10 Apr 2021 08:12:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e44c16e94e3b1dbd69e19de696cd7efbdfba7b0dce4839c9cc84d00723baf0`  
		Last Modified: Sat, 10 Apr 2021 18:00:05 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c89f5fc34f9483ba7e47ec017c35bb676b60da7741e6bad709bc7fdefae84ff`  
		Last Modified: Sat, 10 Apr 2021 18:01:14 GMT  
		Size: 76.9 MB (76861581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee37976bcb7dae0210c9778b746e1f691c1596086da7a80e35d5875518742cf`  
		Last Modified: Sat, 10 Apr 2021 18:00:50 GMT  
		Size: 1.3 MB (1315113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee876c751e57427a82e3fc88949c5979019da1bccd76fe8ac5d1a689cd2d93d8`  
		Last Modified: Sat, 10 Apr 2021 18:00:48 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af19d44e71a574d596d347d5fe6f9cbeba87ba0bcc4bbe1501c8c9a023f5fac3`  
		Last Modified: Sat, 10 Apr 2021 18:00:48 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d0869083c1f98b291e8d414c9fe3a5eaf3b65fc243570dd364e738f60c8329`  
		Last Modified: Sat, 10 Apr 2021 18:00:49 GMT  
		Size: 2.5 MB (2541672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9535d688965d325fc9df3bbad4751621b1c787c9596d76b715bec37735e71b`  
		Last Modified: Sat, 10 Apr 2021 18:01:02 GMT  
		Size: 59.2 MB (59184008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839254017393f3fa7519521037c5ffc30ba3921adec999522ee5f588ba46f08`  
		Last Modified: Sat, 10 Apr 2021 18:00:48 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.8` - linux; arm variant v7

```console
$ docker pull redmine@sha256:8a3a5e24ade51015ef2dc3cd63769f1dea40ca4e35c144f0bd3b276c75418da0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.2 MB (189232714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e45c68fdcd14c809057951978490cdfaffc55b4dc779ca9d8b3bd3e15ee144d5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:49:54 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:49:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:49:57 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:53:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:53:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:53:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:53:49 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:42:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:51:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:51:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:51:46 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:51:51 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:51:52 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:51:58 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:52:00 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 04:52:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 04:52:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:56:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:56:55 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:56:56 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:56:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:56:58 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:56:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae68a3a282a83d0e6da8b00595a45c9fb467b44e46970f00dee3a849e860c81c`  
		Last Modified: Sat, 10 Apr 2021 17:20:12 GMT  
		Size: 20.6 MB (20643582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b299ede54fe617996860ca241d888ae39341d21408e0f7e892ef71dea23ee3`  
		Last Modified: Sat, 10 Apr 2021 17:20:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac4b477683229835feada0995794aaeeee3d978e339a0c29e31b5401fdc5ca`  
		Last Modified: Sun, 11 Apr 2021 04:58:14 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3990681ca7a1c562915fdecf77cdccf54cfdda6eb931027cecdee6c4f85659c7`  
		Last Modified: Sun, 11 Apr 2021 04:59:21 GMT  
		Size: 73.2 MB (73204168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd53e50d67fdc8a6e2a79bd97066ccbce4dd59fc1f60100d558c21944dadaf8`  
		Last Modified: Sun, 11 Apr 2021 04:58:59 GMT  
		Size: 1.3 MB (1305509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958928bb957c6b08625c811b507ea4a97eb32ac5aa2ac0852c8ae47030ecb485`  
		Last Modified: Sun, 11 Apr 2021 04:58:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4873f8c056cc4bfca6960b68718220581ab216d6b9727bde045389a588f0d0f7`  
		Last Modified: Sun, 11 Apr 2021 04:58:57 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f67089eac0e1b6944494f80ecaff256a775a221dcd47e39690543da90ffb8d`  
		Last Modified: Sun, 11 Apr 2021 04:58:58 GMT  
		Size: 2.5 MB (2541659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb430435f743b101667bef7564a03cc96f556ccd1c6f3dc94e29dbacc84305b`  
		Last Modified: Sun, 11 Apr 2021 04:59:11 GMT  
		Size: 58.9 MB (58921665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40735fa79b3ebc2e47ddfe4becc86813e59d735ec18e73087019cb2635945121`  
		Last Modified: Sun, 11 Apr 2021 04:58:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.8` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:5eb881676d38f6af2fe269977b09833145a7b2898db63417670531cb12758fde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.0 MB (201957441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98bfce45df8c4a75b15c77d4990f6749994006f014ec692f10cb9c7ce7897fac`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:20:43 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:20:49 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:20:50 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:24:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:24:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:24:38 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:41:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:49:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:49:31 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:49:32 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:49:34 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:49:35 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:49:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:49:40 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 04:49:42 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 04:49:49 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:55:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:55:07 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:55:09 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:55:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:55:12 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:55:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805a70932a287839e4483317925d47a504efbbe434fde5824ef4192898e352e2`  
		Last Modified: Sat, 10 Apr 2021 16:50:01 GMT  
		Size: 21.3 MB (21308477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f9a34f968a2b1af6ba62fe49a0831f817c21182613ab38a0633bf356c0cf23`  
		Last Modified: Sat, 10 Apr 2021 16:49:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ececbf89e390256b43a15f33c53615e9029553b1726dffad48507d7138213a6`  
		Last Modified: Sun, 11 Apr 2021 04:56:21 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5cc8027e85bd9d41b2f186cd6ad07efbe7f8da82390b5c4d8de6f78021bc759`  
		Last Modified: Sun, 11 Apr 2021 04:57:16 GMT  
		Size: 79.6 MB (79640373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e692a5b9422d5c10fe5cce66c63ae5bf9a69783134d2a2af1002f3c908d078ad`  
		Last Modified: Sun, 11 Apr 2021 04:56:57 GMT  
		Size: 1.3 MB (1291820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ece293a5e59922b35ae9fddc3da48953f17cbaa854812ae86f4c761465b639c`  
		Last Modified: Sun, 11 Apr 2021 04:56:55 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd66c8fcd8111228dadd5a92532739e995d7f5ed8718eb53f2d6bf3cfaaa2ffa`  
		Last Modified: Sun, 11 Apr 2021 04:56:55 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95678d3d349f52fb12f61ee024aaf7d2f5308fa582c487cc33d5219c004b54cf`  
		Last Modified: Sun, 11 Apr 2021 04:56:58 GMT  
		Size: 2.5 MB (2541675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4337c75954970548b54020a8f86710b389ee763d43ab30dedb3fe1552d7d2bcf`  
		Last Modified: Sun, 11 Apr 2021 04:57:06 GMT  
		Size: 60.0 MB (60003321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c567294b3f7a69dedebbb90bde1cd921b46d461b3f2c76499fd257c990e6ad2d`  
		Last Modified: Sun, 11 Apr 2021 04:56:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.8` - linux; 386

```console
$ docker pull redmine@sha256:96069edc4e4d04e68d45c29178395c155fd991d071d364c16a39063cb6378630
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.4 MB (211425618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0668a7b02f442b188b66272ab162d691f57f04c279d0f37fcc6ca70fcd97c4b4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:52:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:52:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:52:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:52:19 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:14:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 16:17:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:17:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:17:16 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 16:17:16 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 16:17:16 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 16:17:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 16:17:17 GMT
ENV REDMINE_VERSION=4.0.8
# Sat, 10 Apr 2021 16:17:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sat, 10 Apr 2021 16:17:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 16:19:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:19:56 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 16:19:56 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 16:19:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 16:19:56 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 16:19:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207aa5aba20825c04fb847653d3cf6d5011040c7f7b8147ce0824ebda58d682`  
		Last Modified: Sat, 10 Apr 2021 03:13:02 GMT  
		Size: 20.9 MB (20909318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5e3665a3fdb3774edce1b87e369d385982d95b3f12169b947249c7ecb6566`  
		Last Modified: Sat, 10 Apr 2021 03:12:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c61c4b79a951b1b483b330e6fa809e988bab5ec193531c977e7c39ce6fa6fa`  
		Last Modified: Sat, 10 Apr 2021 16:21:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488d2ea51179d8da50447ec20ceb69ff3cbb1ca84b11ffe0524c48984e5859d2`  
		Last Modified: Sat, 10 Apr 2021 16:22:26 GMT  
		Size: 82.4 MB (82437500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a8f287298504a3aa8010a144f1daf33313922972e3e6cc27b60c6f32598ca3`  
		Last Modified: Sat, 10 Apr 2021 16:22:06 GMT  
		Size: 1.3 MB (1327322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db57538301434f4789ac2c33becf9c072f47849d6bb28e483602c979dcbfdf5c`  
		Last Modified: Sat, 10 Apr 2021 16:22:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5989dfc48bca16aa4cc9559c74a5894dce06ccd6f9f0a1d9bee163857e060c`  
		Last Modified: Sat, 10 Apr 2021 16:22:04 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e117ff45b4482fa69c393342a1e6d5e0aa244a1e3e637bb7acc5691b3fb289cc`  
		Last Modified: Sat, 10 Apr 2021 16:22:05 GMT  
		Size: 2.5 MB (2541674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8fdabe362e26b82776cc039f91365dafb45cce29a37309b6524fc5415289541`  
		Last Modified: Sat, 10 Apr 2021 16:22:14 GMT  
		Size: 59.2 MB (59189302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc72e552a747a702d1664614f7e3408e56827f3738008af7887f372b311e801`  
		Last Modified: Sat, 10 Apr 2021 16:22:04 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.8` - linux; mips64le

```console
$ docker pull redmine@sha256:8738baa7a2937d7502e62817bc2530701f825c2a0987e2a88f2ef98f75e2b672
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.2 MB (201176539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47f7c2189ac46bef43f27812d17e3f3af2026801613c2330b819c344bd68ad56`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:24:25 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 15:24:25 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 15:24:26 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 15:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:32:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:32:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:32:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:32:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:33:00 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:25:30 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:36:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:36:45 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:36:45 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:36:46 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:36:46 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:36:48 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 19:36:49 GMT
ENV REDMINE_VERSION=4.0.8
# Sat, 10 Apr 2021 19:36:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sat, 10 Apr 2021 19:36:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 19:43:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:43:57 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 19:43:58 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 19:43:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 19:43:59 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 19:43:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6a8b6e14ae4c50de74d8a7225fdb08536fc034f6994e460e0f9d6476b068a3`  
		Last Modified: Sat, 10 Apr 2021 15:53:23 GMT  
		Size: 21.7 MB (21661143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af10c60efa418c61d498b86b823d73662484fc921d24b76362fa7c8a1d716be`  
		Last Modified: Sat, 10 Apr 2021 15:53:14 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a88a9e837e51dc5511791e1410d11311dca9f231f8f6120d1160d240ae957b`  
		Last Modified: Sat, 10 Apr 2021 19:45:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cf8215a8716b3e15c8bd3aad48bdf15c21385de589012a3eb76dc0f2a37908`  
		Last Modified: Sat, 10 Apr 2021 19:48:12 GMT  
		Size: 78.1 MB (78139675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e13e07952c904491e48b6dda1750654d334aa9dd35919df91a5aa6e625fbc74`  
		Last Modified: Sat, 10 Apr 2021 19:47:16 GMT  
		Size: 1.2 MB (1244216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b46e972b003bc2193bbd0639e08d48952993d3a035e9b190b6bbb785eb22a87`  
		Last Modified: Sat, 10 Apr 2021 19:47:12 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a955ff4dd91d61cab4d30e90b580f30be55c5fbcdeb05ea260cf5793f07d83`  
		Last Modified: Sat, 10 Apr 2021 19:47:12 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46931f792b62001c6927e4d3c143e93885ff850343d25b0aa64e86ee31476cb2`  
		Last Modified: Sat, 10 Apr 2021 19:47:16 GMT  
		Size: 2.5 MB (2541151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32de1b7a80b6a4eaa3cf8f53bd71f995562bad3c079a37977b9bdc8221cddae9`  
		Last Modified: Sat, 10 Apr 2021 19:47:45 GMT  
		Size: 60.2 MB (60151932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b39d2e83bc8ab6475b6620a745e238da82b66b8a85d1d5f35f30ff64ba68601`  
		Last Modified: Sat, 10 Apr 2021 19:47:12 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.8` - linux; ppc64le

```console
$ docker pull redmine@sha256:9f1f3e0d7846ad7b474ffc99f3892dd65363565fb53d02289d684c2cb71a4995
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217504698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e59a6b27b14fd14a8dc6ea9a129337ce0b677130cfa55399a427267e86c17bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:57:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:57:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:57:33 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:27:53 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 15:27:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 15:28:01 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 15:35:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:35:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:35:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:35:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:35:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:36:11 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:14:19 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:51:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:51:51 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:52:02 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:52:15 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:52:49 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:53:02 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 06:53:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 06:53:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 07:07:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:07:10 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 07:07:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 07:07:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 07:07:20 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 07:07:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cbbc810e9494a5dfcf8ee1e195a1a58bd57e76aadf8003b70553ed4eb09b2`  
		Last Modified: Sat, 10 Apr 2021 15:54:53 GMT  
		Size: 12.7 MB (12704371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa4e10ca5b1345262af0a6624b7f9980011d8180575de45104358ed122152a`  
		Last Modified: Sat, 10 Apr 2021 15:54:50 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0266f29c4d0be5f1d382e9ff0a02f03fb96494b3d6e0fc30c71ea410f72c0`  
		Last Modified: Sat, 10 Apr 2021 15:56:30 GMT  
		Size: 22.0 MB (21984924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168d7a83cd3ffcd313c7d046285a1eabaaba553d590844df3ee3cbd7648a2c9`  
		Last Modified: Sat, 10 Apr 2021 15:56:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb092c4cd4d038d1b22d42c5079bbf5d4f101cd8e63a587f6104ece43b205bba`  
		Last Modified: Sun, 11 Apr 2021 07:09:01 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c147cc6419922fa988f9638c830159a176b9c956096d08120ce71e236f7911e7`  
		Last Modified: Sun, 11 Apr 2021 07:09:57 GMT  
		Size: 87.7 MB (87746565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6b309da6e581e596c7919fd5b8423b0cd3905601300ab84981071ee10a26e6`  
		Last Modified: Sun, 11 Apr 2021 07:09:39 GMT  
		Size: 1.3 MB (1276387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ece19dff96976adb31b39d5c2c163e80d594dbba168094a110a1d7cdd75dad6`  
		Last Modified: Sun, 11 Apr 2021 07:09:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77bc115d8d040dd4b647aab0f01c637065b90cac0e00b03ccedfd73bf7ebce67`  
		Last Modified: Sun, 11 Apr 2021 07:09:36 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79d8a41917f2e428d12487247fba2c52c08cd20e762aa00c622acf3b2243d3c`  
		Last Modified: Sun, 11 Apr 2021 07:09:37 GMT  
		Size: 2.5 MB (2541674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a028db1877457828483431f599c3c02e11413bbe1895790b488c5b7891874e45`  
		Last Modified: Sun, 11 Apr 2021 07:09:46 GMT  
		Size: 60.7 MB (60700588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a16a0038c282eb456758805cfb035e9480cc62e8b43629ebdec3a5b5751fda`  
		Last Modified: Sun, 11 Apr 2021 07:09:36 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.8` - linux; s390x

```console
$ docker pull redmine@sha256:ad9baf8ca388ec8d53aeceee13fdcfde3a5863875dd563b426b2d363f6648823
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.4 MB (201369506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d4f2b8e63dc709509807105e97793dbc83e8ac03b337e5554a0d6693cbf2a9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:17:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:17:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:17:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:17:20 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:36:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 12:42:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:43:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:43:06 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 12:43:07 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 12:43:08 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 12:43:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 12:43:10 GMT
ENV REDMINE_VERSION=4.0.8
# Sat, 10 Apr 2021 12:43:11 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sat, 10 Apr 2021 12:43:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 12:47:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:47:25 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 12:47:26 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 12:47:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 12:47:27 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 12:47:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f085c8813292ca999ce489985962c48c430c2055b5e583be1f6f4e0dfd5353`  
		Last Modified: Sat, 10 Apr 2021 02:22:58 GMT  
		Size: 21.6 MB (21618739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea955664e86a3a2fc2a4765705d82563887aaa4c51dd1b6de0ad1d783561ee90`  
		Last Modified: Sat, 10 Apr 2021 02:22:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caafc17bfb9bef6d20a4d1bee71743fdc15a7b73de616c69b477f48c1140d05`  
		Last Modified: Sat, 10 Apr 2021 12:48:23 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3971b7397a8d2b592596fa5005416be4c47904803edbc7c6003f1639e90680ff`  
		Last Modified: Sat, 10 Apr 2021 12:49:08 GMT  
		Size: 78.8 MB (78776229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:024030ae4ad30ae8062177468e6f0fc42e845f4b2f83a044f5e8f74123c90e9c`  
		Last Modified: Sat, 10 Apr 2021 12:48:54 GMT  
		Size: 1.3 MB (1342620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75216f044269d86b8d4ec63782f2b474d58e3d7d960cd14f60b68ee654ad782e`  
		Last Modified: Sat, 10 Apr 2021 12:48:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385328e9e2cb30103ce68dbaffa561af084effdb23444698761c9cf9844f145c`  
		Last Modified: Sat, 10 Apr 2021 12:48:51 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1153191d2cb5ac6078ed551e10ca8ef67371cfb9f4aad2f378b8d6507cb986ec`  
		Last Modified: Sat, 10 Apr 2021 12:48:52 GMT  
		Size: 2.5 MB (2541667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e60fc43d39d62022c7a591cc115af38cb818ead6bc760d9dad8e0f53f7a1a0ba`  
		Last Modified: Sat, 10 Apr 2021 12:49:01 GMT  
		Size: 60.5 MB (60517943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806bf7f576d6dac5d3f6d9e8425df03c396f71c5e789b6e7a227d550be60da8e`  
		Last Modified: Sat, 10 Apr 2021 12:48:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.8-alpine`

```console
$ docker pull redmine@sha256:8a11b8b550012b7c4cbbd59395c4c9e9e555b07236320391b78d6b520467e13a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0.8-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:90b7600c4aff4f071d854964035266096766456e349bfadf4ee7806046aa93f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.3 MB (153335497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c1028c79f4b7526e4dfa853b0f422b7ed1fb3a5063aaf444f66fc19bd6fffc1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:39:43 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 10:39:45 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:55:16 GMT
ENV RUBY_MAJOR=2.6
# Mon, 05 Apr 2021 19:40:49 GMT
ENV RUBY_VERSION=2.6.7
# Mon, 05 Apr 2021 19:40:49 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Mon, 05 Apr 2021 19:45:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:45:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:45:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:45:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:45:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:45:05 GMT
CMD ["irb"]
# Mon, 05 Apr 2021 20:49:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Mon, 05 Apr 2021 20:55:37 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Mon, 05 Apr 2021 20:55:37 GMT
ENV RAILS_ENV=production
# Mon, 05 Apr 2021 20:55:38 GMT
WORKDIR /usr/src/redmine
# Mon, 05 Apr 2021 20:55:38 GMT
ENV HOME=/home/redmine
# Mon, 05 Apr 2021 20:55:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 05 Apr 2021 20:55:39 GMT
ENV REDMINE_VERSION=4.0.8
# Mon, 05 Apr 2021 20:55:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Mon, 05 Apr 2021 20:55:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 05 Apr 2021 20:55:43 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 05 Apr 2021 20:57:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 05 Apr 2021 20:57:18 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 05 Apr 2021 20:57:18 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 05 Apr 2021 20:57:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 05 Apr 2021 20:57:19 GMT
EXPOSE 3000
# Mon, 05 Apr 2021 20:57:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9df2de4dab84e51acacca9e65a3d9f7c9fa2f038bc11c2830bd9a97980823a0`  
		Last Modified: Thu, 01 Apr 2021 11:09:32 GMT  
		Size: 1.2 MB (1218696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc339b259bb6448a756fb9b42044f3450a7dcd6fc3bc0102a3cb6b7594daca19`  
		Last Modified: Thu, 01 Apr 2021 11:09:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50912dd8ac3c72a63b47d2ea4938ce0d0b540b3d281b6e7afde7431b771f7821`  
		Last Modified: Mon, 05 Apr 2021 20:16:47 GMT  
		Size: 21.8 MB (21839400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d6f19cafc240eb97d8d85ce13604a63ae1302240377da30f1da030a381871f`  
		Last Modified: Mon, 05 Apr 2021 20:16:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e42f435c0bb598a2d54e4d1abb1e2433c64bd72e903564a32209b96271fdbd1`  
		Last Modified: Mon, 05 Apr 2021 21:00:16 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052fd31a2728992bf069a7683e900c63361022a28130f178ecf37313bd21d422`  
		Last Modified: Mon, 05 Apr 2021 21:01:41 GMT  
		Size: 66.1 MB (66075620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc80bea3abebec9cc2134e12e98f1ab38c146536b99f32663f151cd41f2cb212`  
		Last Modified: Mon, 05 Apr 2021 21:01:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1beb398278d5829cee76d372b79ca33d82c06e64428bf5b5213651f482973c2d`  
		Last Modified: Mon, 05 Apr 2021 21:01:24 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab61081e09c9755e45525b209fb625aac5ce72b7a4f1a0d38db5bdcbc94bde3f`  
		Last Modified: Mon, 05 Apr 2021 21:01:25 GMT  
		Size: 2.5 MB (2543099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3745ef83cee6de7a9dc13f726fcba8f0a9eb464fde25414699ff12415bc34b2d`  
		Last Modified: Mon, 05 Apr 2021 21:01:31 GMT  
		Size: 58.8 MB (58843006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baed54af0e0b00be44b1b6aa25e915b79468d85bf7f7f2a0e0cffa1979684aa2`  
		Last Modified: Mon, 05 Apr 2021 21:01:24 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.8-passenger`

```console
$ docker pull redmine@sha256:41e4bafd59e8ca296c50879d573f0cbd20fea6a22bfe167e05776117a8c4504f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0.8-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:daafacdf3abafd2e54870eceb6140e779419d89a1f2379530b9687bbaf6c68c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.5 MB (231467473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2883b123c919a0ae57fadef7afcdadaf2d6dd2767de9b607bbbe1a383cc506ef`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 07:00:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 07:00:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:00:22 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 07:00:22 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 07:00:22 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 07:00:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 07:00:23 GMT
ENV REDMINE_VERSION=4.0.8
# Sun, 11 Apr 2021 07:00:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=c06ebd75ab87b23d766b37a9e49c9e456756ed91f85b33a584a66f47f888038a
# Sun, 11 Apr 2021 07:00:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 07:02:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:02:12 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 07:02:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 07:02:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 07:02:12 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 07:02:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sun, 11 Apr 2021 07:02:28 GMT
ENV PASSENGER_VERSION=6.0.8
# Sun, 11 Apr 2021 07:02:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 07:02:46 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sun, 11 Apr 2021 07:02:46 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sun, 11 Apr 2021 07:02:46 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d7e3f1a32c6de0dd372c7905837938a00bf39ab4fcdf748828c4935073551`  
		Last Modified: Sun, 11 Apr 2021 07:04:17 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66743655a9623d68938cfd2efa15e72fb70ce962094fb3c79e40b4408b4e0d1b`  
		Last Modified: Sun, 11 Apr 2021 07:05:19 GMT  
		Size: 81.0 MB (81020804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2861ed67e9e65e0194f1809af11356a997d4ef594e1771b8db9f30fc27f9cc22`  
		Last Modified: Sun, 11 Apr 2021 07:05:07 GMT  
		Size: 1.4 MB (1356453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd99b3be78435843199962828c2bf524d28bfd5123cbadbe79a88aebcacff54`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46277daa4e0232f5f265213bdf13fe3f6fa33c11303e762754b3f6c5a3d67404`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f2bf905d64fdc0678fa13c72441ce49310b8d7d35b2cbf4a5fef981b63436f`  
		Last Modified: Sun, 11 Apr 2021 07:05:04 GMT  
		Size: 2.5 MB (2541667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bd12f0c8e81c2201227718b39054718d424aa01620d6558b0f6f8097968796`  
		Last Modified: Sun, 11 Apr 2021 07:05:15 GMT  
		Size: 60.1 MB (60085642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e702d6f9980e3173128449df698c15765b1dc2208f84fa6e86ffcbb503fb68`  
		Last Modified: Sun, 11 Apr 2021 07:05:03 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d96e78e20fe93a6e3de8b1f405bfac07a1fb431e911c2261eb33673b6341a1`  
		Last Modified: Sun, 11 Apr 2021 07:05:33 GMT  
		Size: 20.4 MB (20352904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f2124ce9e6dbe37feeb5ae18cac7fbbc7dbf0ec4536b9d7ef6f50187b493a4`  
		Last Modified: Sun, 11 Apr 2021 07:05:31 GMT  
		Size: 4.9 MB (4936714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1`

```console
$ docker pull redmine@sha256:a2aaeed0b28c5c882208737b4ec67f60d4f5fabcf3efd1b58514eb4db1264d6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.1` - linux; amd64

```console
$ docker pull redmine@sha256:73b4e5f9d99b69c68315653592358a66b81c66852017e87e67a9800041bfae4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207749072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3914314da3f40e5625114119dc5ca04b0ad63b7ebc2b802b90458395d55c77d1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:58:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:58:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:58:30 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:58:31 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:58:31 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:58:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:58:32 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 06:58:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 06:58:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:59:15 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:59:15 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:59:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:59:16 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d7e3f1a32c6de0dd372c7905837938a00bf39ab4fcdf748828c4935073551`  
		Last Modified: Sun, 11 Apr 2021 07:04:17 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91811187fec224eb7aeb2b7421651780efae9c381ebae414471ae50ebfcb83b5`  
		Last Modified: Sun, 11 Apr 2021 07:04:32 GMT  
		Size: 93.9 MB (93905525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd1b2cef837a6657b68dccce68d0e76e6ff56de1be4decfcefd28f6ea76f8`  
		Last Modified: Sun, 11 Apr 2021 07:04:18 GMT  
		Size: 1.4 MB (1370194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e4d930e298fbd202fb41566d57fbb4f6913db69bbe579cff4b4b24c2aa7885`  
		Last Modified: Sun, 11 Apr 2021 07:04:14 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f4134d45fb63638e13a531c6517542ac9eb020e63e0395fd9eaab33babbd80`  
		Last Modified: Sun, 11 Apr 2021 07:04:15 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1b0504ae04ffb70028de5776b99956146f1f45bf2fcb9d3395d44353534570`  
		Last Modified: Sun, 11 Apr 2021 07:04:15 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c5f984afe6efa58f788bf6647e78a9c6c994a9e1fe77d2e67ebbc962f4ac67`  
		Last Modified: Sun, 11 Apr 2021 07:04:20 GMT  
		Size: 48.6 MB (48553591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fdb5ebb7f091b28cd15560d42f97e1c01205814a996362262a4e3f7adfa594`  
		Last Modified: Sun, 11 Apr 2021 07:04:14 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:9d39b6efe49ecafe51a8295c9eac7877bfc2a8583d1d1660090817110abf8d5d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.7 MB (211749881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b78d26b2835b9867fe6190bdb56af323aa72b47480c758a5def9264976756c0b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:42:11 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 07:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:45:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:45:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:45:55 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:45:11 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 17:46:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:47:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:47:11 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 17:47:12 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 17:47:14 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 17:47:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 17:47:18 GMT
ENV REDMINE_VERSION=4.1.2
# Sat, 10 Apr 2021 17:47:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sat, 10 Apr 2021 17:47:28 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 17:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:51:58 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 17:51:58 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 17:51:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:52:01 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 17:52:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f63c1e0d3af67924d2d3ef5636ed70900748b90fffc5bf4e748a38ef7d125`  
		Last Modified: Sat, 10 Apr 2021 08:12:41 GMT  
		Size: 20.7 MB (20732839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9ef980b82778a927138ed4192338fea82cdb79fe3d25e26ac958cc5dc33d62`  
		Last Modified: Sat, 10 Apr 2021 08:12:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e44c16e94e3b1dbd69e19de696cd7efbdfba7b0dce4839c9cc84d00723baf0`  
		Last Modified: Sat, 10 Apr 2021 18:00:05 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c364343bf05f51cfc9fb0fc1ebb9b393feb9a844050ab35525441396786564e9`  
		Last Modified: Sat, 10 Apr 2021 18:00:32 GMT  
		Size: 89.5 MB (89482003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72bcc2163fcadbba15f5f696f8638c0a328034ac0fb434aa1cde74078352311`  
		Last Modified: Sat, 10 Apr 2021 18:00:04 GMT  
		Size: 1.3 MB (1326369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdfeb45b03eb35039bec2708ffbe20b4efbdaca637d4e6f09b4664fdc28ae11`  
		Last Modified: Sat, 10 Apr 2021 17:59:58 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28fdd64a0c6324f4d02fcbcb929e6e923df8a7fe3522833e2030f9f2b81cc6a`  
		Last Modified: Sat, 10 Apr 2021 17:59:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1281944129892177e991e0386c2a13bebc69e26a89b002a5415f01946af13e`  
		Last Modified: Sat, 10 Apr 2021 18:00:03 GMT  
		Size: 2.7 MB (2746468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141e3385933ae3e45aba16698625d4dd261713e2a08d071a13dce3ce61f449bd`  
		Last Modified: Sat, 10 Apr 2021 18:00:11 GMT  
		Size: 62.2 MB (62239462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d451cc648e0b3b0a5d0953e165c6e0d9fd9ac16616fcd27461f29da3d392072`  
		Last Modified: Sat, 10 Apr 2021 17:59:58 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:d2e491c93e38ffd903e920c726bf1bf0be80b1929f253baf20446a474b64ac82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204939589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9adf06ac048e59dd6fa0c65c84125aad90e2f3d7f1cb552926b10e81699e8ee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:49:54 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:49:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:49:57 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:53:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:53:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:53:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:53:49 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:42:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:44:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:44:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:44:31 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:44:33 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:44:35 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:44:46 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:44:47 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 04:44:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 04:45:03 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:49:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:49:18 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:49:21 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:49:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:49:26 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:49:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae68a3a282a83d0e6da8b00595a45c9fb467b44e46970f00dee3a849e860c81c`  
		Last Modified: Sat, 10 Apr 2021 17:20:12 GMT  
		Size: 20.6 MB (20643582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b299ede54fe617996860ca241d888ae39341d21408e0f7e892ef71dea23ee3`  
		Last Modified: Sat, 10 Apr 2021 17:20:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac4b477683229835feada0995794aaeeee3d978e339a0c29e31b5401fdc5ca`  
		Last Modified: Sun, 11 Apr 2021 04:58:14 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726549e18ac568b5a5c79a13defed057c324fb8b4a65adbb972ad269fad363f5`  
		Last Modified: Sun, 11 Apr 2021 04:58:41 GMT  
		Size: 85.5 MB (85517558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df11c32488aee47b6d6c1e9ea9e70794922b1db236aa8e4fe9c76db0678b599`  
		Last Modified: Sun, 11 Apr 2021 04:58:15 GMT  
		Size: 1.3 MB (1319121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b996809afa5a4c9b8e6a005d8a742c02723bce46655166ea475f69ca267aa4a6`  
		Last Modified: Sun, 11 Apr 2021 04:58:12 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9d3dc4346f1745faa7a8659ab80a0575adfec38d60788a5362a01ec04cac9`  
		Last Modified: Sun, 11 Apr 2021 04:58:12 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2d37d8e890a1e0f0dfbe3ee082850355c7641a75fcb2775e5dc02eed2455ca`  
		Last Modified: Sun, 11 Apr 2021 04:58:14 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c78a4ea1f090c2ff1ea86a7df4e7bc951e9e3b27f6f7f02a5387928d455c7b0`  
		Last Modified: Sun, 11 Apr 2021 04:58:27 GMT  
		Size: 62.1 MB (62096724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c91efe8c3422b13944bdd40975515ec1d49091e2f2860ad620e37a337f2f200`  
		Last Modified: Sun, 11 Apr 2021 04:58:12 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:18c4f922bd01c0aab4cc3c9b9223874d3987b223a14b3cd1a9ea39544e982830
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.6 MB (218575756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a75df60cd124e2c87978a11257e1671ca9ac6fac6ada3c99a5e6f15241ad9fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:20:43 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:20:49 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:20:50 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:24:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:24:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:24:38 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:41:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:43:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:43:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:43:23 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:43:24 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:43:25 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:43:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:43:29 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 04:43:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 04:43:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:47:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:47:43 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:47:44 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:47:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:47:46 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:47:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805a70932a287839e4483317925d47a504efbbe434fde5824ef4192898e352e2`  
		Last Modified: Sat, 10 Apr 2021 16:50:01 GMT  
		Size: 21.3 MB (21308477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f9a34f968a2b1af6ba62fe49a0831f817c21182613ab38a0633bf356c0cf23`  
		Last Modified: Sat, 10 Apr 2021 16:49:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ececbf89e390256b43a15f33c53615e9029553b1726dffad48507d7138213a6`  
		Last Modified: Sun, 11 Apr 2021 04:56:21 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71498e4ed4574973a4e56ed0a7696d25bd1df25877cb746ed456da966002be4a`  
		Last Modified: Sun, 11 Apr 2021 04:56:47 GMT  
		Size: 92.5 MB (92499108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f0fce1627f11adec38a99117fcc119b3bdc16cafa53e8273be611337315421`  
		Last Modified: Sun, 11 Apr 2021 04:56:20 GMT  
		Size: 1.3 MB (1303596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8972b0c8bfa9e2dc9a6748239442b83877f1b638151ac1ce544d22d80e4bdcbf`  
		Last Modified: Sun, 11 Apr 2021 04:56:19 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebf12e723219b1e66b6967c638959d285fe6cb0f0b1f86548f7fe38144f541e`  
		Last Modified: Sun, 11 Apr 2021 04:56:19 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3273e141e97001a620f06ae5358a28e312161c1466e67f872fffe745504a672`  
		Last Modified: Sun, 11 Apr 2021 04:56:20 GMT  
		Size: 2.7 MB (2746470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5636f511f434a05195f1e7304c84793ab6e92bb54b46a014a8bba79d42b2dd1`  
		Last Modified: Sun, 11 Apr 2021 04:56:32 GMT  
		Size: 63.5 MB (63546328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4910aba89eaea66fea43f1790bbc19f41fa2d5ea1fdf4aea0975c7a8166472ca`  
		Last Modified: Sun, 11 Apr 2021 04:56:19 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; 386

```console
$ docker pull redmine@sha256:3ca8e90ff8fd84b456d3ee696b5669a5e12d12a30e0d8e32eb31b82603958963
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.1 MB (214085652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a339d78d7775d25ab786a901148bc0de46d39707f7596e58b1b116b1d37ae9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:52:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:52:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:52:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:52:19 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:14:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 16:15:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:15:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:15:26 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 16:15:26 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 16:15:26 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 16:15:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 16:15:27 GMT
ENV REDMINE_VERSION=4.1.2
# Sat, 10 Apr 2021 16:15:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sat, 10 Apr 2021 16:15:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 16:16:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:16:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 16:16:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 16:16:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 16:16:22 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 16:16:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207aa5aba20825c04fb847653d3cf6d5011040c7f7b8147ce0824ebda58d682`  
		Last Modified: Sat, 10 Apr 2021 03:13:02 GMT  
		Size: 20.9 MB (20909318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5e3665a3fdb3774edce1b87e369d385982d95b3f12169b947249c7ecb6566`  
		Last Modified: Sat, 10 Apr 2021 03:12:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c61c4b79a951b1b483b330e6fa809e988bab5ec193531c977e7c39ce6fa6fa`  
		Last Modified: Sat, 10 Apr 2021 16:21:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39b7b76936d5c34abe598348d3ff7844673a22a66e90ffb341a0345648c2cc0`  
		Last Modified: Sat, 10 Apr 2021 16:21:51 GMT  
		Size: 95.5 MB (95537804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd5d9d8bf772fb47342ae47d89caab4a0a7638098486c015ca61ace283d6b16`  
		Last Modified: Sat, 10 Apr 2021 16:21:29 GMT  
		Size: 1.3 MB (1338992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc5e97b4c509bc284a442600fff741cdc26deaac97cdc308a76d7d6498cfad2`  
		Last Modified: Sat, 10 Apr 2021 16:21:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5882f058018caa7612770dfba577df1c11b9f47407bf2ea385a935591fc4a1`  
		Last Modified: Sat, 10 Apr 2021 16:21:26 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cf9728414f34b8792226232c03354af16e8b4fe26d839ecb0d4cc6f3d2f876`  
		Last Modified: Sat, 10 Apr 2021 16:21:27 GMT  
		Size: 2.7 MB (2746474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f138f123c78a8f354dbc3fdbc15012355f45b8bfb55d354a31b1833fd8c92b69`  
		Last Modified: Sat, 10 Apr 2021 16:21:35 GMT  
		Size: 48.5 MB (48532561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ad0b33ad619f09da82257ad17d2b9e2083984150156d6eec1511618454fb18`  
		Last Modified: Sat, 10 Apr 2021 16:21:26 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; mips64le

```console
$ docker pull redmine@sha256:2d95e09ed274d477710bb382eb708be23a8b0bc2f93a2bc0f60a9621e8574ec5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.0 MB (217970340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e10bc218df278c47c17250eb029f49e78434e71cd8baee464cf13ac79ba7af`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:24:25 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 15:24:25 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 15:24:26 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 15:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:32:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:32:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:32:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:32:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:33:00 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:25:30 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:26:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:27:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:27:06 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:27:06 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:27:07 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:27:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 19:27:09 GMT
ENV REDMINE_VERSION=4.1.2
# Sat, 10 Apr 2021 19:27:10 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sat, 10 Apr 2021 19:27:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 19:34:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:34:57 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 19:34:57 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 19:34:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 19:34:58 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 19:34:58 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6a8b6e14ae4c50de74d8a7225fdb08536fc034f6994e460e0f9d6476b068a3`  
		Last Modified: Sat, 10 Apr 2021 15:53:23 GMT  
		Size: 21.7 MB (21661143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af10c60efa418c61d498b86b823d73662484fc921d24b76362fa7c8a1d716be`  
		Last Modified: Sat, 10 Apr 2021 15:53:14 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a88a9e837e51dc5511791e1410d11311dca9f231f8f6120d1160d240ae957b`  
		Last Modified: Sat, 10 Apr 2021 19:45:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c17b2c7b97875f3d574c371e85bb708548ca22912b457bb2893bbdd2db01a1`  
		Last Modified: Sat, 10 Apr 2021 19:47:01 GMT  
		Size: 90.9 MB (90869345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4210b9a15fe4a0d69b6aa09062d3d98f6ee7e158b814ff2accad2c2bfbed9e1`  
		Last Modified: Sat, 10 Apr 2021 19:45:55 GMT  
		Size: 1.3 MB (1257338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966a945bc1e901c71578fc72c5a0c495cdd7349963f2f936dd1ae04a131730f`  
		Last Modified: Sat, 10 Apr 2021 19:45:51 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73b50353a2e9a5231189eabf8e1db8f4e5f166a288a0e7cc7a4115c6c1ad899`  
		Last Modified: Sat, 10 Apr 2021 19:45:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff3975bb195e9eb22f11f4bdcf1cdff37de88ea859bffe24f9aa90ac9356262`  
		Last Modified: Sat, 10 Apr 2021 19:45:55 GMT  
		Size: 2.7 MB (2746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7195af12fc8fbf4bdda9d8f9da6b0911cf9f433796e685c3211745b2c5cdc89`  
		Last Modified: Sat, 10 Apr 2021 19:46:24 GMT  
		Size: 64.0 MB (63998075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186bb702b5a0f33c9a91dae0fc6814a2006487c4836f29f7efef99baf74468ab`  
		Last Modified: Sat, 10 Apr 2021 19:45:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:6c76a5d20a78f467d71f08f968ae24df93ecb3d58ee05fd5cd2ba94f18816e18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235054662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3088be9b91671c8974242524940e6ee40407049a4874a9f214008350da16a050`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:57:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:57:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:57:33 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:27:53 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 15:27:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 15:28:01 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 15:35:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:35:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:35:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:35:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:35:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:36:11 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:14:19 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:19:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:21:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:21:27 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:21:36 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:21:43 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:21:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:22:00 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 06:22:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 06:22:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:32:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:32:30 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:32:35 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:32:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:32:51 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:33:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cbbc810e9494a5dfcf8ee1e195a1a58bd57e76aadf8003b70553ed4eb09b2`  
		Last Modified: Sat, 10 Apr 2021 15:54:53 GMT  
		Size: 12.7 MB (12704371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa4e10ca5b1345262af0a6624b7f9980011d8180575de45104358ed122152a`  
		Last Modified: Sat, 10 Apr 2021 15:54:50 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0266f29c4d0be5f1d382e9ff0a02f03fb96494b3d6e0fc30c71ea410f72c0`  
		Last Modified: Sat, 10 Apr 2021 15:56:30 GMT  
		Size: 22.0 MB (21984924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168d7a83cd3ffcd313c7d046285a1eabaaba553d590844df3ee3cbd7648a2c9`  
		Last Modified: Sat, 10 Apr 2021 15:56:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb092c4cd4d038d1b22d42c5079bbf5d4f101cd8e63a587f6104ece43b205bba`  
		Last Modified: Sun, 11 Apr 2021 07:09:01 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f12304d3dcc47db34ee708817b811d31570a31001392f43d84fdc49735bad41`  
		Last Modified: Sun, 11 Apr 2021 07:09:22 GMT  
		Size: 101.1 MB (101147377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a78d2dd0e3c70ab8fe443a7505d25cdbd06d3cda767fa19353921bffb371d6`  
		Last Modified: Sun, 11 Apr 2021 07:09:01 GMT  
		Size: 1.3 MB (1290201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295518dcb2413b65a3172dcf1bca4d49db0891601d6db95a7982d8adec74e165`  
		Last Modified: Sun, 11 Apr 2021 07:08:58 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1823988bb8c7ef289a8dacf10c78949baa3a9c7401f3dc6afade99f38b42536`  
		Last Modified: Sun, 11 Apr 2021 07:08:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01aa024f002084b333a3493b2bc578da8289604297cbe1df443b4abb67bd7b53`  
		Last Modified: Sun, 11 Apr 2021 07:09:02 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faab34bc23aec1942e034d255f10a626c72883af81994e668f1d452eadd9b2b`  
		Last Modified: Sun, 11 Apr 2021 07:09:08 GMT  
		Size: 64.6 MB (64631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b48255e37a75e256fc97590fb40d0b1ad4063f8f64c51685ccc313ea617ccde`  
		Last Modified: Sun, 11 Apr 2021 07:08:58 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; s390x

```console
$ docker pull redmine@sha256:2f9f5cc700be6e5ab18da7f2c2f3f2ffdcba1ca7339a5b3da2d08d88dd57e053
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.9 MB (217947505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d015df05851fa893b6acd99daa5ab2be50bd88038d29baf18fd37f34caa64b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:17:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:17:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:17:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:17:20 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:36:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 12:37:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:37:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:37:50 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 12:37:50 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 12:37:51 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 12:37:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 12:37:53 GMT
ENV REDMINE_VERSION=4.1.2
# Sat, 10 Apr 2021 12:37:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sat, 10 Apr 2021 12:38:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 12:41:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:41:11 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 12:41:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 12:41:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 12:41:13 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 12:41:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f085c8813292ca999ce489985962c48c430c2055b5e583be1f6f4e0dfd5353`  
		Last Modified: Sat, 10 Apr 2021 02:22:58 GMT  
		Size: 21.6 MB (21618739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea955664e86a3a2fc2a4765705d82563887aaa4c51dd1b6de0ad1d783561ee90`  
		Last Modified: Sat, 10 Apr 2021 02:22:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caafc17bfb9bef6d20a4d1bee71743fdc15a7b73de616c69b477f48c1140d05`  
		Last Modified: Sat, 10 Apr 2021 12:48:23 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb44bf96a7cc7a79ac3dbfb605a8d3d52cb6fa794a3c7296025c86ba7cebc2f`  
		Last Modified: Sat, 10 Apr 2021 12:48:44 GMT  
		Size: 91.6 MB (91641479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c42f97e68d7d7fd2cc782a2db857f93eb5a9e78320f055148186f0a43baee4`  
		Last Modified: Sat, 10 Apr 2021 12:48:23 GMT  
		Size: 1.4 MB (1356223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd2c3968631783c0fe843a21c949ba489adeb7f5b7bbd75f777a75cdeecb58f`  
		Last Modified: Sat, 10 Apr 2021 12:48:20 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9f2f73f47cf544a87597ca5ad0a305c2c4266e3e3683dae204007b3fb12772`  
		Last Modified: Sat, 10 Apr 2021 12:48:20 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2806f9483e016a67523f6eee31289633fbe84f9cd524d0ae0c49dde7e9a14026`  
		Last Modified: Sat, 10 Apr 2021 12:48:21 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7006d57df9cc2d1fc54b1c7f8a5471b0651e0d57ee65afb818c96fe641cbdb18`  
		Last Modified: Sat, 10 Apr 2021 12:48:30 GMT  
		Size: 64.0 MB (64012284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec716c36ae015130e3029a293c13d3415f5d67a3db6ce54aaed5d065cadd9c8`  
		Last Modified: Sat, 10 Apr 2021 12:48:20 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-alpine`

```console
$ docker pull redmine@sha256:611aa4f048742b42b0ec136480d7d349745e11e21cc3e083386eb4f5a83b1593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:942626e1902f02984a7c34e0575f05a91115999baf366e50f1168823e8f6502e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.4 MB (160360471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0da569709263f60d3ce3a9949215cf0cdcf5c06b985965718e1670ca90e3d59`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:39:43 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 10:39:45 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:55:16 GMT
ENV RUBY_MAJOR=2.6
# Mon, 05 Apr 2021 19:40:49 GMT
ENV RUBY_VERSION=2.6.7
# Mon, 05 Apr 2021 19:40:49 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Mon, 05 Apr 2021 19:45:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:45:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:45:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:45:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:45:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:45:05 GMT
CMD ["irb"]
# Mon, 05 Apr 2021 20:49:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Mon, 05 Apr 2021 20:49:35 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Mon, 05 Apr 2021 20:49:36 GMT
ENV RAILS_ENV=production
# Mon, 05 Apr 2021 20:49:36 GMT
WORKDIR /usr/src/redmine
# Mon, 05 Apr 2021 20:49:36 GMT
ENV HOME=/home/redmine
# Mon, 05 Apr 2021 20:49:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 05 Apr 2021 20:49:37 GMT
ENV REDMINE_VERSION=4.1.2
# Mon, 05 Apr 2021 20:49:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Mon, 05 Apr 2021 20:49:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 05 Apr 2021 20:49:42 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 05 Apr 2021 20:51:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 05 Apr 2021 20:51:52 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 05 Apr 2021 20:51:52 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 05 Apr 2021 20:51:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 05 Apr 2021 20:51:53 GMT
EXPOSE 3000
# Mon, 05 Apr 2021 20:51:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9df2de4dab84e51acacca9e65a3d9f7c9fa2f038bc11c2830bd9a97980823a0`  
		Last Modified: Thu, 01 Apr 2021 11:09:32 GMT  
		Size: 1.2 MB (1218696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc339b259bb6448a756fb9b42044f3450a7dcd6fc3bc0102a3cb6b7594daca19`  
		Last Modified: Thu, 01 Apr 2021 11:09:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50912dd8ac3c72a63b47d2ea4938ce0d0b540b3d281b6e7afde7431b771f7821`  
		Last Modified: Mon, 05 Apr 2021 20:16:47 GMT  
		Size: 21.8 MB (21839400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d6f19cafc240eb97d8d85ce13604a63ae1302240377da30f1da030a381871f`  
		Last Modified: Mon, 05 Apr 2021 20:16:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e42f435c0bb598a2d54e4d1abb1e2433c64bd72e903564a32209b96271fdbd1`  
		Last Modified: Mon, 05 Apr 2021 21:00:16 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807f00acf7b7c5e8aee2ebd283ec689329fd8882f724c7487fde09c870479caf`  
		Last Modified: Mon, 05 Apr 2021 21:00:28 GMT  
		Size: 69.4 MB (69427790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a5dbd53ba82a487b476ea2de64374cf1bed41f6e9aaa4b59a38345742f461b`  
		Last Modified: Mon, 05 Apr 2021 21:00:13 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661de499c7c828b9b6b1d597665c5e5da87cf13bd178220749b74464fe581370`  
		Last Modified: Mon, 05 Apr 2021 21:00:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b76f5cb8dec4f7ecdef7e00dea0815935fd8b6aa4fd5e61e6278ed68395d967`  
		Last Modified: Mon, 05 Apr 2021 21:00:14 GMT  
		Size: 2.7 MB (2747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3b58afbc2fe052aa4c652844b4895d833f3892930f9c802371e852ce6dae7`  
		Last Modified: Mon, 05 Apr 2021 21:00:20 GMT  
		Size: 62.3 MB (62311243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363376f05964d713321595d18d81b04052f045ae52731f57f3e47221d31ccd63`  
		Last Modified: Mon, 05 Apr 2021 21:00:13 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-passenger`

```console
$ docker pull redmine@sha256:12ccecfef6e028ee9af5b731450dc1be0adeaa64c02016bad6c2b545f412afd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:3d9669bbdf838b2e49d39be054c35cb658d5eae1678054e32822232e2514b83a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233033841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:497a402dbd3e08d3df61c4b607b10a35c23aef576acbd1db46717763638bd11e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:58:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:58:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:58:30 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:58:31 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:58:31 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:58:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:58:32 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 06:58:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 06:58:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:59:15 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:59:15 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:59:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:59:16 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sun, 11 Apr 2021 06:59:23 GMT
ENV PASSENGER_VERSION=6.0.8
# Sun, 11 Apr 2021 06:59:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:59:39 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sun, 11 Apr 2021 06:59:39 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sun, 11 Apr 2021 06:59:40 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d7e3f1a32c6de0dd372c7905837938a00bf39ab4fcdf748828c4935073551`  
		Last Modified: Sun, 11 Apr 2021 07:04:17 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91811187fec224eb7aeb2b7421651780efae9c381ebae414471ae50ebfcb83b5`  
		Last Modified: Sun, 11 Apr 2021 07:04:32 GMT  
		Size: 93.9 MB (93905525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd1b2cef837a6657b68dccce68d0e76e6ff56de1be4decfcefd28f6ea76f8`  
		Last Modified: Sun, 11 Apr 2021 07:04:18 GMT  
		Size: 1.4 MB (1370194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e4d930e298fbd202fb41566d57fbb4f6913db69bbe579cff4b4b24c2aa7885`  
		Last Modified: Sun, 11 Apr 2021 07:04:14 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f4134d45fb63638e13a531c6517542ac9eb020e63e0395fd9eaab33babbd80`  
		Last Modified: Sun, 11 Apr 2021 07:04:15 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1b0504ae04ffb70028de5776b99956146f1f45bf2fcb9d3395d44353534570`  
		Last Modified: Sun, 11 Apr 2021 07:04:15 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c5f984afe6efa58f788bf6647e78a9c6c994a9e1fe77d2e67ebbc962f4ac67`  
		Last Modified: Sun, 11 Apr 2021 07:04:20 GMT  
		Size: 48.6 MB (48553591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fdb5ebb7f091b28cd15560d42f97e1c01205814a996362262a4e3f7adfa594`  
		Last Modified: Sun, 11 Apr 2021 07:04:14 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4deecf8c6025be666466ff27044551f02a08bc3b8b894e5c5b99cfbd762ef26f`  
		Last Modified: Sun, 11 Apr 2021 07:04:51 GMT  
		Size: 20.3 MB (20348050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bc824c4ed6dae8575775bf2cb8215300aff74957d9a92dfdf222b50958bcdf`  
		Last Modified: Sun, 11 Apr 2021 07:04:49 GMT  
		Size: 4.9 MB (4936719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.2`

```console
$ docker pull redmine@sha256:a2aaeed0b28c5c882208737b4ec67f60d4f5fabcf3efd1b58514eb4db1264d6d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.1.2` - linux; amd64

```console
$ docker pull redmine@sha256:73b4e5f9d99b69c68315653592358a66b81c66852017e87e67a9800041bfae4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207749072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3914314da3f40e5625114119dc5ca04b0ad63b7ebc2b802b90458395d55c77d1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:58:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:58:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:58:30 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:58:31 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:58:31 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:58:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:58:32 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 06:58:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 06:58:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:59:15 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:59:15 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:59:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:59:16 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d7e3f1a32c6de0dd372c7905837938a00bf39ab4fcdf748828c4935073551`  
		Last Modified: Sun, 11 Apr 2021 07:04:17 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91811187fec224eb7aeb2b7421651780efae9c381ebae414471ae50ebfcb83b5`  
		Last Modified: Sun, 11 Apr 2021 07:04:32 GMT  
		Size: 93.9 MB (93905525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd1b2cef837a6657b68dccce68d0e76e6ff56de1be4decfcefd28f6ea76f8`  
		Last Modified: Sun, 11 Apr 2021 07:04:18 GMT  
		Size: 1.4 MB (1370194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e4d930e298fbd202fb41566d57fbb4f6913db69bbe579cff4b4b24c2aa7885`  
		Last Modified: Sun, 11 Apr 2021 07:04:14 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f4134d45fb63638e13a531c6517542ac9eb020e63e0395fd9eaab33babbd80`  
		Last Modified: Sun, 11 Apr 2021 07:04:15 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1b0504ae04ffb70028de5776b99956146f1f45bf2fcb9d3395d44353534570`  
		Last Modified: Sun, 11 Apr 2021 07:04:15 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c5f984afe6efa58f788bf6647e78a9c6c994a9e1fe77d2e67ebbc962f4ac67`  
		Last Modified: Sun, 11 Apr 2021 07:04:20 GMT  
		Size: 48.6 MB (48553591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fdb5ebb7f091b28cd15560d42f97e1c01205814a996362262a4e3f7adfa594`  
		Last Modified: Sun, 11 Apr 2021 07:04:14 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.2` - linux; arm variant v5

```console
$ docker pull redmine@sha256:9d39b6efe49ecafe51a8295c9eac7877bfc2a8583d1d1660090817110abf8d5d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.7 MB (211749881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b78d26b2835b9867fe6190bdb56af323aa72b47480c758a5def9264976756c0b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:42:11 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 07:42:12 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 07:45:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:45:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:51 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:45:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:45:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:45:55 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:45:11 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 17:46:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:47:10 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:47:11 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 17:47:12 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 17:47:14 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 17:47:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 17:47:18 GMT
ENV REDMINE_VERSION=4.1.2
# Sat, 10 Apr 2021 17:47:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sat, 10 Apr 2021 17:47:28 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 17:51:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:51:58 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 17:51:58 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 17:51:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:52:01 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 17:52:02 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f63c1e0d3af67924d2d3ef5636ed70900748b90fffc5bf4e748a38ef7d125`  
		Last Modified: Sat, 10 Apr 2021 08:12:41 GMT  
		Size: 20.7 MB (20732839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9ef980b82778a927138ed4192338fea82cdb79fe3d25e26ac958cc5dc33d62`  
		Last Modified: Sat, 10 Apr 2021 08:12:36 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e44c16e94e3b1dbd69e19de696cd7efbdfba7b0dce4839c9cc84d00723baf0`  
		Last Modified: Sat, 10 Apr 2021 18:00:05 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c364343bf05f51cfc9fb0fc1ebb9b393feb9a844050ab35525441396786564e9`  
		Last Modified: Sat, 10 Apr 2021 18:00:32 GMT  
		Size: 89.5 MB (89482003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72bcc2163fcadbba15f5f696f8638c0a328034ac0fb434aa1cde74078352311`  
		Last Modified: Sat, 10 Apr 2021 18:00:04 GMT  
		Size: 1.3 MB (1326369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdfeb45b03eb35039bec2708ffbe20b4efbdaca637d4e6f09b4664fdc28ae11`  
		Last Modified: Sat, 10 Apr 2021 17:59:58 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28fdd64a0c6324f4d02fcbcb929e6e923df8a7fe3522833e2030f9f2b81cc6a`  
		Last Modified: Sat, 10 Apr 2021 17:59:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1281944129892177e991e0386c2a13bebc69e26a89b002a5415f01946af13e`  
		Last Modified: Sat, 10 Apr 2021 18:00:03 GMT  
		Size: 2.7 MB (2746468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:141e3385933ae3e45aba16698625d4dd261713e2a08d071a13dce3ce61f449bd`  
		Last Modified: Sat, 10 Apr 2021 18:00:11 GMT  
		Size: 62.2 MB (62239462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d451cc648e0b3b0a5d0953e165c6e0d9fd9ac16616fcd27461f29da3d392072`  
		Last Modified: Sat, 10 Apr 2021 17:59:58 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:d2e491c93e38ffd903e920c726bf1bf0be80b1929f253baf20446a474b64ac82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204939589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9adf06ac048e59dd6fa0c65c84125aad90e2f3d7f1cb552926b10e81699e8ee`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:49:54 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:49:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:49:57 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:53:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:53:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:53:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:53:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:53:49 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:42:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:44:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:44:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:44:31 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:44:33 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:44:35 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:44:46 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:44:47 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 04:44:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 04:45:03 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:49:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:49:18 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:49:21 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:49:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:49:26 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:49:28 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae68a3a282a83d0e6da8b00595a45c9fb467b44e46970f00dee3a849e860c81c`  
		Last Modified: Sat, 10 Apr 2021 17:20:12 GMT  
		Size: 20.6 MB (20643582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b299ede54fe617996860ca241d888ae39341d21408e0f7e892ef71dea23ee3`  
		Last Modified: Sat, 10 Apr 2021 17:20:08 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afac4b477683229835feada0995794aaeeee3d978e339a0c29e31b5401fdc5ca`  
		Last Modified: Sun, 11 Apr 2021 04:58:14 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726549e18ac568b5a5c79a13defed057c324fb8b4a65adbb972ad269fad363f5`  
		Last Modified: Sun, 11 Apr 2021 04:58:41 GMT  
		Size: 85.5 MB (85517558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df11c32488aee47b6d6c1e9ea9e70794922b1db236aa8e4fe9c76db0678b599`  
		Last Modified: Sun, 11 Apr 2021 04:58:15 GMT  
		Size: 1.3 MB (1319121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b996809afa5a4c9b8e6a005d8a742c02723bce46655166ea475f69ca267aa4a6`  
		Last Modified: Sun, 11 Apr 2021 04:58:12 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c9d3dc4346f1745faa7a8659ab80a0575adfec38d60788a5362a01ec04cac9`  
		Last Modified: Sun, 11 Apr 2021 04:58:12 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec2d37d8e890a1e0f0dfbe3ee082850355c7641a75fcb2775e5dc02eed2455ca`  
		Last Modified: Sun, 11 Apr 2021 04:58:14 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c78a4ea1f090c2ff1ea86a7df4e7bc951e9e3b27f6f7f02a5387928d455c7b0`  
		Last Modified: Sun, 11 Apr 2021 04:58:27 GMT  
		Size: 62.1 MB (62096724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c91efe8c3422b13944bdd40975515ec1d49091e2f2860ad620e37a337f2f200`  
		Last Modified: Sun, 11 Apr 2021 04:58:12 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:18c4f922bd01c0aab4cc3c9b9223874d3987b223a14b3cd1a9ea39544e982830
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.6 MB (218575756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a75df60cd124e2c87978a11257e1671ca9ac6fac6ada3c99a5e6f15241ad9fc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:20:43 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 16:20:49 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 16:20:50 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 16:24:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:24:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:24:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:24:37 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:24:38 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:41:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:43:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:43:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:43:23 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:43:24 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:43:25 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:43:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:43:29 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 04:43:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 04:43:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:47:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:47:43 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:47:44 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:47:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:47:46 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:47:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805a70932a287839e4483317925d47a504efbbe434fde5824ef4192898e352e2`  
		Last Modified: Sat, 10 Apr 2021 16:50:01 GMT  
		Size: 21.3 MB (21308477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f9a34f968a2b1af6ba62fe49a0831f817c21182613ab38a0633bf356c0cf23`  
		Last Modified: Sat, 10 Apr 2021 16:49:57 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ececbf89e390256b43a15f33c53615e9029553b1726dffad48507d7138213a6`  
		Last Modified: Sun, 11 Apr 2021 04:56:21 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71498e4ed4574973a4e56ed0a7696d25bd1df25877cb746ed456da966002be4a`  
		Last Modified: Sun, 11 Apr 2021 04:56:47 GMT  
		Size: 92.5 MB (92499108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f0fce1627f11adec38a99117fcc119b3bdc16cafa53e8273be611337315421`  
		Last Modified: Sun, 11 Apr 2021 04:56:20 GMT  
		Size: 1.3 MB (1303596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8972b0c8bfa9e2dc9a6748239442b83877f1b638151ac1ce544d22d80e4bdcbf`  
		Last Modified: Sun, 11 Apr 2021 04:56:19 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebf12e723219b1e66b6967c638959d285fe6cb0f0b1f86548f7fe38144f541e`  
		Last Modified: Sun, 11 Apr 2021 04:56:19 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3273e141e97001a620f06ae5358a28e312161c1466e67f872fffe745504a672`  
		Last Modified: Sun, 11 Apr 2021 04:56:20 GMT  
		Size: 2.7 MB (2746470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5636f511f434a05195f1e7304c84793ab6e92bb54b46a014a8bba79d42b2dd1`  
		Last Modified: Sun, 11 Apr 2021 04:56:32 GMT  
		Size: 63.5 MB (63546328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4910aba89eaea66fea43f1790bbc19f41fa2d5ea1fdf4aea0975c7a8166472ca`  
		Last Modified: Sun, 11 Apr 2021 04:56:19 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.2` - linux; 386

```console
$ docker pull redmine@sha256:3ca8e90ff8fd84b456d3ee696b5669a5e12d12a30e0d8e32eb31b82603958963
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.1 MB (214085652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80a339d78d7775d25ab786a901148bc0de46d39707f7596e58b1b116b1d37ae9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:48:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:52:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:52:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:52:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:52:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:52:19 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:14:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 16:15:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:15:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:15:26 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 16:15:26 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 16:15:26 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 16:15:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 16:15:27 GMT
ENV REDMINE_VERSION=4.1.2
# Sat, 10 Apr 2021 16:15:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sat, 10 Apr 2021 16:15:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 16:16:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:16:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 16:16:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 16:16:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 16:16:22 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 16:16:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4207aa5aba20825c04fb847653d3cf6d5011040c7f7b8147ce0824ebda58d682`  
		Last Modified: Sat, 10 Apr 2021 03:13:02 GMT  
		Size: 20.9 MB (20909318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a5e3665a3fdb3774edce1b87e369d385982d95b3f12169b947249c7ecb6566`  
		Last Modified: Sat, 10 Apr 2021 03:12:57 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c61c4b79a951b1b483b330e6fa809e988bab5ec193531c977e7c39ce6fa6fa`  
		Last Modified: Sat, 10 Apr 2021 16:21:29 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39b7b76936d5c34abe598348d3ff7844673a22a66e90ffb341a0345648c2cc0`  
		Last Modified: Sat, 10 Apr 2021 16:21:51 GMT  
		Size: 95.5 MB (95537804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cd5d9d8bf772fb47342ae47d89caab4a0a7638098486c015ca61ace283d6b16`  
		Last Modified: Sat, 10 Apr 2021 16:21:29 GMT  
		Size: 1.3 MB (1338992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc5e97b4c509bc284a442600fff741cdc26deaac97cdc308a76d7d6498cfad2`  
		Last Modified: Sat, 10 Apr 2021 16:21:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d5882f058018caa7612770dfba577df1c11b9f47407bf2ea385a935591fc4a1`  
		Last Modified: Sat, 10 Apr 2021 16:21:26 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21cf9728414f34b8792226232c03354af16e8b4fe26d839ecb0d4cc6f3d2f876`  
		Last Modified: Sat, 10 Apr 2021 16:21:27 GMT  
		Size: 2.7 MB (2746474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f138f123c78a8f354dbc3fdbc15012355f45b8bfb55d354a31b1833fd8c92b69`  
		Last Modified: Sat, 10 Apr 2021 16:21:35 GMT  
		Size: 48.5 MB (48532561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ad0b33ad619f09da82257ad17d2b9e2083984150156d6eec1511618454fb18`  
		Last Modified: Sat, 10 Apr 2021 16:21:26 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.2` - linux; mips64le

```console
$ docker pull redmine@sha256:2d95e09ed274d477710bb382eb708be23a8b0bc2f93a2bc0f60a9621e8574ec5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.0 MB (217970340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6e10bc218df278c47c17250eb029f49e78434e71cd8baee464cf13ac79ba7af`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:24:25 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 15:24:25 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 15:24:26 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 15:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:32:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:32:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:32:57 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:32:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:33:00 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:25:30 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:26:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:27:06 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:27:06 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:27:06 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:27:07 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:27:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 19:27:09 GMT
ENV REDMINE_VERSION=4.1.2
# Sat, 10 Apr 2021 19:27:10 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sat, 10 Apr 2021 19:27:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 19:34:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:34:57 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 19:34:57 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 19:34:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 19:34:58 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 19:34:58 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a6a8b6e14ae4c50de74d8a7225fdb08536fc034f6994e460e0f9d6476b068a3`  
		Last Modified: Sat, 10 Apr 2021 15:53:23 GMT  
		Size: 21.7 MB (21661143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af10c60efa418c61d498b86b823d73662484fc921d24b76362fa7c8a1d716be`  
		Last Modified: Sat, 10 Apr 2021 15:53:14 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a88a9e837e51dc5511791e1410d11311dca9f231f8f6120d1160d240ae957b`  
		Last Modified: Sat, 10 Apr 2021 19:45:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c17b2c7b97875f3d574c371e85bb708548ca22912b457bb2893bbdd2db01a1`  
		Last Modified: Sat, 10 Apr 2021 19:47:01 GMT  
		Size: 90.9 MB (90869345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4210b9a15fe4a0d69b6aa09062d3d98f6ee7e158b814ff2accad2c2bfbed9e1`  
		Last Modified: Sat, 10 Apr 2021 19:45:55 GMT  
		Size: 1.3 MB (1257338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c966a945bc1e901c71578fc72c5a0c495cdd7349963f2f936dd1ae04a131730f`  
		Last Modified: Sat, 10 Apr 2021 19:45:51 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73b50353a2e9a5231189eabf8e1db8f4e5f166a288a0e7cc7a4115c6c1ad899`  
		Last Modified: Sat, 10 Apr 2021 19:45:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff3975bb195e9eb22f11f4bdcf1cdff37de88ea859bffe24f9aa90ac9356262`  
		Last Modified: Sat, 10 Apr 2021 19:45:55 GMT  
		Size: 2.7 MB (2746015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7195af12fc8fbf4bdda9d8f9da6b0911cf9f433796e685c3211745b2c5cdc89`  
		Last Modified: Sat, 10 Apr 2021 19:46:24 GMT  
		Size: 64.0 MB (63998075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186bb702b5a0f33c9a91dae0fc6814a2006487c4836f29f7efef99baf74468ab`  
		Last Modified: Sat, 10 Apr 2021 19:45:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.2` - linux; ppc64le

```console
$ docker pull redmine@sha256:6c76a5d20a78f467d71f08f968ae24df93ecb3d58ee05fd5cd2ba94f18816e18
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.1 MB (235054662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3088be9b91671c8974242524940e6ee40407049a4874a9f214008350da16a050`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:57:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:57:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:57:33 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:27:53 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 15:27:56 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 15:28:01 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 15:35:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:35:32 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:35:37 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:35:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:35:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:36:11 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:14:19 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:19:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:21:16 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:21:27 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:21:36 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:21:43 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:21:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:22:00 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 06:22:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 06:22:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:32:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:32:30 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:32:35 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:32:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:32:51 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:33:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cbbc810e9494a5dfcf8ee1e195a1a58bd57e76aadf8003b70553ed4eb09b2`  
		Last Modified: Sat, 10 Apr 2021 15:54:53 GMT  
		Size: 12.7 MB (12704371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa4e10ca5b1345262af0a6624b7f9980011d8180575de45104358ed122152a`  
		Last Modified: Sat, 10 Apr 2021 15:54:50 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0266f29c4d0be5f1d382e9ff0a02f03fb96494b3d6e0fc30c71ea410f72c0`  
		Last Modified: Sat, 10 Apr 2021 15:56:30 GMT  
		Size: 22.0 MB (21984924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5168d7a83cd3ffcd313c7d046285a1eabaaba553d590844df3ee3cbd7648a2c9`  
		Last Modified: Sat, 10 Apr 2021 15:56:28 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb092c4cd4d038d1b22d42c5079bbf5d4f101cd8e63a587f6104ece43b205bba`  
		Last Modified: Sun, 11 Apr 2021 07:09:01 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f12304d3dcc47db34ee708817b811d31570a31001392f43d84fdc49735bad41`  
		Last Modified: Sun, 11 Apr 2021 07:09:22 GMT  
		Size: 101.1 MB (101147377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a78d2dd0e3c70ab8fe443a7505d25cdbd06d3cda767fa19353921bffb371d6`  
		Last Modified: Sun, 11 Apr 2021 07:09:01 GMT  
		Size: 1.3 MB (1290201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295518dcb2413b65a3172dcf1bca4d49db0891601d6db95a7982d8adec74e165`  
		Last Modified: Sun, 11 Apr 2021 07:08:58 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1823988bb8c7ef289a8dacf10c78949baa3a9c7401f3dc6afade99f38b42536`  
		Last Modified: Sun, 11 Apr 2021 07:08:58 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01aa024f002084b333a3493b2bc578da8289604297cbe1df443b4abb67bd7b53`  
		Last Modified: Sun, 11 Apr 2021 07:09:02 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faab34bc23aec1942e034d255f10a626c72883af81994e668f1d452eadd9b2b`  
		Last Modified: Sun, 11 Apr 2021 07:09:08 GMT  
		Size: 64.6 MB (64631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b48255e37a75e256fc97590fb40d0b1ad4063f8f64c51685ccc313ea617ccde`  
		Last Modified: Sun, 11 Apr 2021 07:08:58 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.2` - linux; s390x

```console
$ docker pull redmine@sha256:2f9f5cc700be6e5ab18da7f2c2f3f2ffdcba1ca7339a5b3da2d08d88dd57e053
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.9 MB (217947505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2d015df05851fa893b6acd99daa5ab2be50bd88038d29baf18fd37f34caa64b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 02:15:38 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 02:17:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:17:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:17:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:17:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:17:20 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:36:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 12:37:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:37:49 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:37:50 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 12:37:50 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 12:37:51 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 12:37:53 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 12:37:53 GMT
ENV REDMINE_VERSION=4.1.2
# Sat, 10 Apr 2021 12:37:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sat, 10 Apr 2021 12:38:00 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 12:41:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:41:11 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 12:41:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 12:41:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 12:41:13 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 12:41:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f085c8813292ca999ce489985962c48c430c2055b5e583be1f6f4e0dfd5353`  
		Last Modified: Sat, 10 Apr 2021 02:22:58 GMT  
		Size: 21.6 MB (21618739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea955664e86a3a2fc2a4765705d82563887aaa4c51dd1b6de0ad1d783561ee90`  
		Last Modified: Sat, 10 Apr 2021 02:22:56 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5caafc17bfb9bef6d20a4d1bee71743fdc15a7b73de616c69b477f48c1140d05`  
		Last Modified: Sat, 10 Apr 2021 12:48:23 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb44bf96a7cc7a79ac3dbfb605a8d3d52cb6fa794a3c7296025c86ba7cebc2f`  
		Last Modified: Sat, 10 Apr 2021 12:48:44 GMT  
		Size: 91.6 MB (91641479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c42f97e68d7d7fd2cc782a2db857f93eb5a9e78320f055148186f0a43baee4`  
		Last Modified: Sat, 10 Apr 2021 12:48:23 GMT  
		Size: 1.4 MB (1356223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fd2c3968631783c0fe843a21c949ba489adeb7f5b7bbd75f777a75cdeecb58f`  
		Last Modified: Sat, 10 Apr 2021 12:48:20 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d9f2f73f47cf544a87597ca5ad0a305c2c4266e3e3683dae204007b3fb12772`  
		Last Modified: Sat, 10 Apr 2021 12:48:20 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2806f9483e016a67523f6eee31289633fbe84f9cd524d0ae0c49dde7e9a14026`  
		Last Modified: Sat, 10 Apr 2021 12:48:21 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7006d57df9cc2d1fc54b1c7f8a5471b0651e0d57ee65afb818c96fe641cbdb18`  
		Last Modified: Sat, 10 Apr 2021 12:48:30 GMT  
		Size: 64.0 MB (64012284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec716c36ae015130e3029a293c13d3415f5d67a3db6ce54aaed5d065cadd9c8`  
		Last Modified: Sat, 10 Apr 2021 12:48:20 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.2-alpine`

```console
$ docker pull redmine@sha256:611aa4f048742b42b0ec136480d7d349745e11e21cc3e083386eb4f5a83b1593
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1.2-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:942626e1902f02984a7c34e0575f05a91115999baf366e50f1168823e8f6502e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.4 MB (160360471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0da569709263f60d3ce3a9949215cf0cdcf5c06b985965718e1670ca90e3d59`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:39:43 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 10:39:45 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:55:16 GMT
ENV RUBY_MAJOR=2.6
# Mon, 05 Apr 2021 19:40:49 GMT
ENV RUBY_VERSION=2.6.7
# Mon, 05 Apr 2021 19:40:49 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Mon, 05 Apr 2021 19:45:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:45:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:45:04 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:45:04 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:45:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:45:05 GMT
CMD ["irb"]
# Mon, 05 Apr 2021 20:49:27 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Mon, 05 Apr 2021 20:49:35 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Mon, 05 Apr 2021 20:49:36 GMT
ENV RAILS_ENV=production
# Mon, 05 Apr 2021 20:49:36 GMT
WORKDIR /usr/src/redmine
# Mon, 05 Apr 2021 20:49:36 GMT
ENV HOME=/home/redmine
# Mon, 05 Apr 2021 20:49:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 05 Apr 2021 20:49:37 GMT
ENV REDMINE_VERSION=4.1.2
# Mon, 05 Apr 2021 20:49:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Mon, 05 Apr 2021 20:49:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 05 Apr 2021 20:49:42 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 05 Apr 2021 20:51:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 05 Apr 2021 20:51:52 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 05 Apr 2021 20:51:52 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 05 Apr 2021 20:51:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 05 Apr 2021 20:51:53 GMT
EXPOSE 3000
# Mon, 05 Apr 2021 20:51:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9df2de4dab84e51acacca9e65a3d9f7c9fa2f038bc11c2830bd9a97980823a0`  
		Last Modified: Thu, 01 Apr 2021 11:09:32 GMT  
		Size: 1.2 MB (1218696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc339b259bb6448a756fb9b42044f3450a7dcd6fc3bc0102a3cb6b7594daca19`  
		Last Modified: Thu, 01 Apr 2021 11:09:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50912dd8ac3c72a63b47d2ea4938ce0d0b540b3d281b6e7afde7431b771f7821`  
		Last Modified: Mon, 05 Apr 2021 20:16:47 GMT  
		Size: 21.8 MB (21839400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d6f19cafc240eb97d8d85ce13604a63ae1302240377da30f1da030a381871f`  
		Last Modified: Mon, 05 Apr 2021 20:16:44 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e42f435c0bb598a2d54e4d1abb1e2433c64bd72e903564a32209b96271fdbd1`  
		Last Modified: Mon, 05 Apr 2021 21:00:16 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807f00acf7b7c5e8aee2ebd283ec689329fd8882f724c7487fde09c870479caf`  
		Last Modified: Mon, 05 Apr 2021 21:00:28 GMT  
		Size: 69.4 MB (69427790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a5dbd53ba82a487b476ea2de64374cf1bed41f6e9aaa4b59a38345742f461b`  
		Last Modified: Mon, 05 Apr 2021 21:00:13 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661de499c7c828b9b6b1d597665c5e5da87cf13bd178220749b74464fe581370`  
		Last Modified: Mon, 05 Apr 2021 21:00:13 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b76f5cb8dec4f7ecdef7e00dea0815935fd8b6aa4fd5e61e6278ed68395d967`  
		Last Modified: Mon, 05 Apr 2021 21:00:14 GMT  
		Size: 2.7 MB (2747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf3b58afbc2fe052aa4c652844b4895d833f3892930f9c802371e852ce6dae7`  
		Last Modified: Mon, 05 Apr 2021 21:00:20 GMT  
		Size: 62.3 MB (62311243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363376f05964d713321595d18d81b04052f045ae52731f57f3e47221d31ccd63`  
		Last Modified: Mon, 05 Apr 2021 21:00:13 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.2-passenger`

```console
$ docker pull redmine@sha256:12ccecfef6e028ee9af5b731450dc1be0adeaa64c02016bad6c2b545f412afd0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1.2-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:3d9669bbdf838b2e49d39be054c35cb658d5eae1678054e32822232e2514b83a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.0 MB (233033841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:497a402dbd3e08d3df61c4b607b10a35c23aef576acbd1db46717763638bd11e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_MAJOR=2.6
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_VERSION=2.6.7
# Sat, 10 Apr 2021 18:46:06 GMT
ENV RUBY_DOWNLOAD_SHA256=f43ead5626202d5432d2050eeab606e547f0554299cc1e5cf573d45670e59611
# Sat, 10 Apr 2021 18:49:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:49:02 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:49:03 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:49:04 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:57:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:58:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:58:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:58:30 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:58:31 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:58:31 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:58:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:58:32 GMT
ENV REDMINE_VERSION=4.1.2
# Sun, 11 Apr 2021 06:58:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=7e22397351c53fe8fe4444c01c4e0640d9cefb17b9ac765b846df27627cd228e
# Sun, 11 Apr 2021 06:58:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:59:15 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:59:15 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:59:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:59:16 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sun, 11 Apr 2021 06:59:23 GMT
ENV PASSENGER_VERSION=6.0.8
# Sun, 11 Apr 2021 06:59:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:59:39 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sun, 11 Apr 2021 06:59:39 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sun, 11 Apr 2021 06:59:40 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:451af66bced958304be82120827542b55bd2229f2e83c5a058a441fa74254828`  
		Last Modified: Sat, 10 Apr 2021 19:10:36 GMT  
		Size: 21.5 MB (21467370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3264de8e4173291cbec86320f1fe2733ffcdc3ff53cfa7c0d3238e334b79dea`  
		Last Modified: Sat, 10 Apr 2021 19:10:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449d7e3f1a32c6de0dd372c7905837938a00bf39ab4fcdf748828c4935073551`  
		Last Modified: Sun, 11 Apr 2021 07:04:17 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91811187fec224eb7aeb2b7421651780efae9c381ebae414471ae50ebfcb83b5`  
		Last Modified: Sun, 11 Apr 2021 07:04:32 GMT  
		Size: 93.9 MB (93905525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466bd1b2cef837a6657b68dccce68d0e76e6ff56de1be4decfcefd28f6ea76f8`  
		Last Modified: Sun, 11 Apr 2021 07:04:18 GMT  
		Size: 1.4 MB (1370194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e4d930e298fbd202fb41566d57fbb4f6913db69bbe579cff4b4b24c2aa7885`  
		Last Modified: Sun, 11 Apr 2021 07:04:14 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f4134d45fb63638e13a531c6517542ac9eb020e63e0395fd9eaab33babbd80`  
		Last Modified: Sun, 11 Apr 2021 07:04:15 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1b0504ae04ffb70028de5776b99956146f1f45bf2fcb9d3395d44353534570`  
		Last Modified: Sun, 11 Apr 2021 07:04:15 GMT  
		Size: 2.7 MB (2746473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c5f984afe6efa58f788bf6647e78a9c6c994a9e1fe77d2e67ebbc962f4ac67`  
		Last Modified: Sun, 11 Apr 2021 07:04:20 GMT  
		Size: 48.6 MB (48553591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85fdb5ebb7f091b28cd15560d42f97e1c01205814a996362262a4e3f7adfa594`  
		Last Modified: Sun, 11 Apr 2021 07:04:14 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4deecf8c6025be666466ff27044551f02a08bc3b8b894e5c5b99cfbd762ef26f`  
		Last Modified: Sun, 11 Apr 2021 07:04:51 GMT  
		Size: 20.3 MB (20348050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35bc824c4ed6dae8575775bf2cb8215300aff74957d9a92dfdf222b50958bcdf`  
		Last Modified: Sun, 11 Apr 2021 07:04:49 GMT  
		Size: 4.9 MB (4936719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2`

```console
$ docker pull redmine@sha256:d748e2a03c4a6c25772fe3f8349339b0e1963b1ade3c1103fa09c892f3af61fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.2` - linux; amd64

```console
$ docker pull redmine@sha256:674aaf0691b263a8306a5da9ca763ea706cf9eb73fa97fe5b80880e17e34793e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.5 MB (211501364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9f9e5072432e6d9ac85838768e7d2481b91de8b79dd3010b2d77d4194e7975`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 18:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:42:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:42:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:42:59 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:55:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:56:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:56:28 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:56:28 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:56:28 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:56:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:56:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:17 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:57:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:57:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:57:17 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:57:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1596cf153142005038983af255e0d09ef62c65e139aa5c973c2d2baaa2044b0`  
		Last Modified: Sat, 10 Apr 2021 19:09:47 GMT  
		Size: 22.9 MB (22887036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed63bc8e0386fa836f8cf065b98fa401987445d1ab32e260f00e34398b353c`  
		Last Modified: Sat, 10 Apr 2021 19:09:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6acca6e42a84df58aeac107bc65a7bd29a5a702ca33992837a43d23689e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:20 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1370bc72633d9b6883d4baa5cfe7320f3310950f72f5753966432b3c5fb39af7`  
		Last Modified: Sun, 11 Apr 2021 07:03:35 GMT  
		Size: 93.9 MB (93906284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db1ff6e623ce6c864b167bcc6a6513b6864b9dc79a4d77823597370866a1c4e`  
		Last Modified: Sun, 11 Apr 2021 07:03:21 GMT  
		Size: 1.4 MB (1370219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aafa942955516a5b82908cc908e9fe16aa0e9d25e7c41513563f4d7dcd98e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de8b29a2583f478869875849b6bdc9aa17b8f1cf07835e579284513b946dba`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e2181bd63ce8a24b2330aa48fb52e8188a931903f495caaaaeb4ef6153e86`  
		Last Modified: Sun, 11 Apr 2021 07:03:18 GMT  
		Size: 3.1 MB (3057055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee7416a1645930503313e41e3183303a737aea90454566b7d83fac74e3707`  
		Last Modified: Sun, 11 Apr 2021 07:03:24 GMT  
		Size: 50.6 MB (50574847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f886f325a0ba2239c4905f09d7d6186c89f3202c59614d1181eeecf550cc69`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v5

```console
$ docker pull redmine@sha256:c5a5d3160bd8eaf254b337f502de2c7c6eca5e533afaf87013d16ebdcc40c882
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.7 MB (215708994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94de86d41e3b7f9b9c16ef7a058e074b1b018038726598e9151d8ff64b32769f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:34:59 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 07:35:00 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 07:35:01 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 07:38:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:38:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:38:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:38:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:38:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:38:53 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:37:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 17:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:39:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:39:58 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 17:40:01 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 17:40:02 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 17:40:11 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 17:40:11 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 17:40:12 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 17:40:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 17:44:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:44:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 17:44:51 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 17:44:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:44:54 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 17:44:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da9e41f31dbd59278885fc90a21f78df54ac8e0eeaac6cdfc706d58f3e5cbf9`  
		Last Modified: Sat, 10 Apr 2021 08:12:10 GMT  
		Size: 22.1 MB (22135924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738045962dd0fa8676cf7d722f50e91453ae0e03480b28c95a78b29cbe8c1aca`  
		Last Modified: Sat, 10 Apr 2021 08:12:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce548b7edc54230ecd0be27b260538194321967b7d16ef832e6f86b36ec3269c`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4574075c1b7c50bf542b82a25936d688f4f600298ebf34638e46a49915b6cc30`  
		Last Modified: Sat, 10 Apr 2021 17:59:45 GMT  
		Size: 89.5 MB (89482026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1a552ef67d98bc5894cdb93b2a31d6b45c9ba81f13e609629c00d62d5c8cd5`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 1.3 MB (1326336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8e8040892fd65e2920ca520c1f85934ecaf3cac205140f022d26450ddb4e7`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bf7390b6a87b298e37c8f4401109ac9abaa465b693dd974b717848d0557195`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd685807e7eef49564926e681ac910583fdc0032524d07aa1e3c579701924cea`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 3.1 MB (3057047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d377f01a1044a4d648cfe27174049a37901a12adcf773b420a8cb22670008`  
		Last Modified: Sat, 10 Apr 2021 17:59:26 GMT  
		Size: 64.5 MB (64484917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9309b37c7d17afa9ab0ce43eb207cb4c015cf8080e4ef0026f3605f1d63ea4`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:9b090f6a48322643c7aa5cca725c75dbca849e6b72fb179efd17ca1c878c30a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208872054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce4cd6b1e80353141e77cb6b90438a2b128cfa0dc8b26d3541592dc0d371b4fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:30:27 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 16:30:31 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 16:30:37 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 16:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:34:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:34:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:34:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:34:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:34:51 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:36:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:38:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:38:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:38:22 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:38:23 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:38:24 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:38:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:38:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 04:38:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 04:38:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:42:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:42:29 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:42:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:42:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:42:34 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:42:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544200d357634004457e98f7ac1f43b3a31ebffce5d7e19d2ca99541f0a33131`  
		Last Modified: Sat, 10 Apr 2021 17:19:41 GMT  
		Size: 22.0 MB (22018396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9172351c62ca591dae2a838e01000b6c57489cd47d7af7562e3a495a1caf73b7`  
		Last Modified: Sat, 10 Apr 2021 17:19:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09934e285d86d86fd34b9a3e6d7dec0a3c903bc1d3876022959c6fba45f6ffbd`  
		Last Modified: Sun, 11 Apr 2021 04:57:24 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7fc62da65346ee9c7607a212b41cdbf2c0dc5e365e7c18956017fe19fed731`  
		Last Modified: Sun, 11 Apr 2021 04:57:52 GMT  
		Size: 85.5 MB (85517651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1366c02dd0228cb0f5455a819f46c01c72614c8c2c903f30d8da3f4ba7b3eae0`  
		Last Modified: Sun, 11 Apr 2021 04:57:22 GMT  
		Size: 1.3 MB (1319111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6818a0f2ed85db5a6a199a883fbf6e4eb9f5c1ec90f99cf3b39d2b304b1411`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4544ee1e1bc77a527ff800db97c53158ca440f5fa79330dc3c54988c9ef29`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17ee6b4b9725c04744e6bd790ffa5ec91622e224b5cefe433dd05838c6d7aaf`  
		Last Modified: Sun, 11 Apr 2021 04:57:22 GMT  
		Size: 3.1 MB (3057054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea24d2bc0af67d878125d29f6e1e9bd9c69e601e0796cb3d218c66e6e46bec0`  
		Last Modified: Sun, 11 Apr 2021 04:57:38 GMT  
		Size: 64.3 MB (64343712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cf6d83da71cba257a0d5c791bf2cd1d18b7188c3a7c86a1a04362ccfabf95`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:ed7bf06cf7b08eb7ffdc233007259fabb4475c75c3601ceb0c042fc87080db0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222610474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831ae1d31498a4d3370d0b2a75ac9c10ffddf9837dc3cec001c3239efc9874c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:13:06 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 16:13:06 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 16:13:07 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 16:16:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:16:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:16:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:16:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:16:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:16:56 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:36:04 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:37:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:37:31 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:37:32 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:37:33 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:37:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:37:36 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 04:37:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 04:37:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:41:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:41:39 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:41:40 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:41:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:41:42 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:41:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b735094fd3dfe6c2254ce5bc9c940f71df11fa5f06460d079afd191ebc5c674`  
		Last Modified: Sat, 10 Apr 2021 16:49:23 GMT  
		Size: 22.7 MB (22732804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe803a3eac64f3210850b0bff3533351bd47cfcfe47db8de1dfa928d38082cf8`  
		Last Modified: Sat, 10 Apr 2021 16:49:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe02df6b0d5eaba2d093335c1841a204718b89b5937988b73befc4d70e0e65`  
		Last Modified: Sun, 11 Apr 2021 04:55:42 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6b6f8722801008dc9df47485fb2c8de3e8f64b6ffea6ca55a65a322d489582`  
		Last Modified: Sun, 11 Apr 2021 04:56:08 GMT  
		Size: 92.5 MB (92499331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99372a4bd2cbe51d9628e4fb5763221c86530233759f73d039c898f2a3ef983`  
		Last Modified: Sun, 11 Apr 2021 04:55:43 GMT  
		Size: 1.3 MB (1303583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df37457b9b0458d0364314681801996540e1932316815a2d4c6c7d79e313e51`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f4312e5c8dd083d638060fae2e7c29fbc564c923dcbb0fbde7164acd157ea3`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15912641909cdcaec9376c2b88a72afe5e67c5fc2e67e597f8b3dae13f5723cf`  
		Last Modified: Sun, 11 Apr 2021 04:55:42 GMT  
		Size: 3.1 MB (3057038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf21f8a15c6087c8df6dcd1246a8bcc1fc2cb0558cdd6add076415dab67fb76`  
		Last Modified: Sun, 11 Apr 2021 04:55:55 GMT  
		Size: 65.8 MB (65845943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734c10e558c8e573d6e1113e6234bf8a61362235ff0edf48089f2d749422b434`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; 386

```console
$ docker pull redmine@sha256:a7dfbfbcd168473d1c7b59540044e9be1240a86399758af156e9bc5039d266e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217797824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11f3b67e5b83fae70ed263d4bdc62727a2556e4e6a6500b2f8b8372aa991d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:43:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 02:43:52 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 02:43:52 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 02:48:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:48:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:48:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:48:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:48:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:48:10 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:12:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 16:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:13:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:13:37 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 16:13:37 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 16:13:38 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 16:13:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 16:13:39 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 16:13:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 16:13:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 16:14:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:14:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 16:14:37 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 16:14:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 16:14:38 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 16:14:38 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab4999cad906527dc1dec3fd24fa2f63b4cf3360e33768e9a3afaa30af81f7`  
		Last Modified: Sat, 10 Apr 2021 03:12:12 GMT  
		Size: 22.3 MB (22340618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59394b3c951d09cef112094acc41fbd8608139b79afcccf38fe6ab8fa34363c`  
		Last Modified: Sat, 10 Apr 2021 03:12:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4410c086f240a2556c34f99837c171fc5042ee25324d15eed68d6c823d6f2113`  
		Last Modified: Sat, 10 Apr 2021 16:20:40 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0253065be9c93a1dd65d60739959c872d5e54b24ce0278b1b406dcd9a92fe3`  
		Last Modified: Sat, 10 Apr 2021 16:21:04 GMT  
		Size: 95.5 MB (95537702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8174da1366e0c18236b9ff292261c829c40c6f64f8754aaea0a5054378c2163b`  
		Last Modified: Sat, 10 Apr 2021 16:20:40 GMT  
		Size: 1.3 MB (1338943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a85c94e995fd573909579b7e4bc809efcc8a0cd2fa4c52de0b6934660f8f1b9`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761295a090f25492b48fbb3de84b39bcf24c6ea7d9078df49b8b3e10928eb2`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5674eb34390ddbd43c4c23b1f8c317ab1aa39d015b542ff87e8421a51373b543`  
		Last Modified: Sat, 10 Apr 2021 16:20:39 GMT  
		Size: 3.1 MB (3057038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f18b357fea8d540c87223b845dfe4481d83983e189d41dd1eda244160799c3`  
		Last Modified: Sat, 10 Apr 2021 16:20:47 GMT  
		Size: 50.5 MB (50503021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b11c79faef3e548b798c71ffda1c95254e8f0cda712a838cd6fa199162edc71`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; mips64le

```console
$ docker pull redmine@sha256:d8dfe7820f83a620ce99dd6ff63b0846ca72a25d0e9ea0cba169adfbbbfac925
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222021251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:268ae94296a68b7d47b3d70b15e8d1ddd4720476ed9027f05d0f4cae4f73290f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:06:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:16:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:16:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:16:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:16:12 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:15:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:16:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:16:56 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:16:56 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:16:57 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:16:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 19:16:59 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 19:17:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 19:17:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 19:25:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:25:13 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 19:25:13 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 19:25:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 19:25:14 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 19:25:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a308e0916de51c8816bb907b1f46847b9e4f2a4c13ad8496699a943b1cb1192b`  
		Last Modified: Sat, 10 Apr 2021 15:52:29 GMT  
		Size: 23.1 MB (23101289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4aeaf82f75e03c0de4dc8cfbada529330605924f939a89eea76608b649fc61c`  
		Last Modified: Sat, 10 Apr 2021 15:52:19 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d76e50514a47201bc1e5d1ecd34cb3dd052f552ecc3327f756a2ff28e810fd`  
		Last Modified: Sat, 10 Apr 2021 19:44:24 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9894c487a5a062ca596adb69a0c0d1787a83ea05390fc69a9508850fbd0a2aee`  
		Last Modified: Sat, 10 Apr 2021 19:45:32 GMT  
		Size: 90.9 MB (90869502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b429b96dcf10c532cff19eb56cbb9a41a6e88d65179724f8e8d0a175cb4775`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 1.3 MB (1257309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62845c559925cc0291a80649bdc3e23c43fc80a48a73be6a897e6247d616f7ef`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6114ea006b8a2dfe2a8229a601a2f01991affc3feec2a428b26707c99cc92`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866e595f4eb90b05ffa193035de32d77043c97649769baa388e8ed71df9b4c68`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 3.1 MB (3056466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff3272561a535e8b5ba73ff286d51d976cf39ac87092e2f0fa420e43c3712c`  
		Last Modified: Sat, 10 Apr 2021 19:44:56 GMT  
		Size: 66.3 MB (66298266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5a45d6e6fe63215d266dd648b78c69dc5a5ca1f462be021b884fafacfd1f9a`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; ppc64le

```console
$ docker pull redmine@sha256:613ce7722c4bcd975b4d86b7540bf3add1d5db78ea35459a83abf899bf544501
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239082666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab85f646932584743522c4882cfe4c8d378ae92ff7aea25b2022ea176204f8c6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:57:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:57:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:57:33 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:14:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:14:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:15:05 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:23:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:23:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:23:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:23:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:23:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:23:45 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 05:57:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:05:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:07:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:07:15 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:07:24 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:07:27 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:07:49 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:07:55 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:07:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:08:14 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:13:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:13:32 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:13:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:13:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:13:46 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:13:50 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cbbc810e9494a5dfcf8ee1e195a1a58bd57e76aadf8003b70553ed4eb09b2`  
		Last Modified: Sat, 10 Apr 2021 15:54:53 GMT  
		Size: 12.7 MB (12704371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa4e10ca5b1345262af0a6624b7f9980011d8180575de45104358ed122152a`  
		Last Modified: Sat, 10 Apr 2021 15:54:50 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969b8bec5707756c2c65c42151cedb5ed4aa7cfd90762da603a0c27fc694eb1e`  
		Last Modified: Sat, 10 Apr 2021 15:55:48 GMT  
		Size: 23.4 MB (23414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7799f120e744ecf4af99f5374dd470aed6475ca254813ff9b781f8bd5ee9ba`  
		Last Modified: Sat, 10 Apr 2021 15:55:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17b32b0803cb0c499e8847d76fd9c8188e04f99b0a49d3bb00fb57852da102`  
		Last Modified: Sun, 11 Apr 2021 07:07:58 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04001ba15d9c6379ed6823bd4d279724b7dc9c2c3b1779183e3d5e3cf7ced3e`  
		Last Modified: Sun, 11 Apr 2021 07:08:41 GMT  
		Size: 101.1 MB (101147239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7e01d32f1e67a82e76be158bd1f54e80d8e6d43e082bde15416b0cac68efe`  
		Last Modified: Sun, 11 Apr 2021 07:07:59 GMT  
		Size: 1.3 MB (1290574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579cddd918b5fec468e3a6b5d01ab1113193d9a60fe3f5d11de447084f315b6d`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5181bfb422524a8f6b2eace42ef46cd20f8181d2023edf01874b0d0a5f31bfe`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f706945ab1345126925f34b0a33dcd58dbd84322bd093b64077aa818112f46ee`  
		Last Modified: Sun, 11 Apr 2021 07:07:57 GMT  
		Size: 3.1 MB (3057048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c1a53028ee3ee0723cec0f90306634b171fa7905e55e906839bb7eb8601b4`  
		Last Modified: Sun, 11 Apr 2021 07:08:06 GMT  
		Size: 66.9 MB (66919035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a598556acae8e5996306debd91dadc7da82e6cc011a616f95017b1e043b4ecdb`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; s390x

```console
$ docker pull redmine@sha256:d86d5b58aa7e9dd6dc7547929ce5542856c7580dde88fb5b916c4ae6fc3cee9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222020361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89028240f1dee18298827636e792c7c5a0712b03a6445f2c4b28db0991c314e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:04:20 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 02:04:20 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 02:04:21 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 02:06:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:06:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:06:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:06:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:06:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:06:08 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:31:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 12:32:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:32:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:32:57 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 12:32:58 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 12:32:58 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 12:32:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 12:33:00 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 12:33:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 12:33:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 12:35:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:35:47 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 12:35:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 12:35:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 12:35:48 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 12:35:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3098c63e5609140d293715e979f3576527d20157d2f671592b79736f4d72ddd4`  
		Last Modified: Sat, 10 Apr 2021 02:22:38 GMT  
		Size: 23.1 MB (23066252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3547d43bbb52b78bdbe05cc38cf90175f678f4512422ef47540229443c7a1824`  
		Last Modified: Sat, 10 Apr 2021 02:22:37 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd4d29f072b64c3d7e17a9a81fe61294be125cd7f7c2fee6bddc6b5b61bafe7`  
		Last Modified: Sat, 10 Apr 2021 12:47:53 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4b26acacc50fc4a0c6155d028bde06b918cb698c1eafb066f77c98931b82ca`  
		Last Modified: Sat, 10 Apr 2021 12:48:10 GMT  
		Size: 91.6 MB (91641533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e338871896ec393957d527289b7c3ad84893f5da29ee7152a52c7cc97ccdd05a`  
		Last Modified: Sat, 10 Apr 2021 12:47:53 GMT  
		Size: 1.4 MB (1356207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24b741f8a77912f9f77062871d2a869002331460009e31de96fccbb3604b945`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db5b06d283b2c92a6908585d05e13858d8561b7c61b9c190de9807cd4bf05e4`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e29c0ae231298e90eea6df8a140e4608cff7d379598e181106f9b4de31a517`  
		Last Modified: Sat, 10 Apr 2021 12:47:52 GMT  
		Size: 3.1 MB (3057042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22351124edd3ea56412ba14138a1aafc8eb76b8f7b72842596372b3b8dbf3088`  
		Last Modified: Sat, 10 Apr 2021 12:48:02 GMT  
		Size: 66.3 MB (66327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea92b2f8e559d76b1121c336a586e7884919cb81519ff911a84e78a1e98194`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-alpine`

```console
$ docker pull redmine@sha256:29454a31d1cebcdc33cd50b35495532b6756e6608a036133c68263de8089b9a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.2-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:9d1c434ac62026273ff39820aad3eb9e532678a54012152712ab1a76311a8139
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.3 MB (164260126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5aa389f0b143c0ea7e350e485f5936594d02e5f31ee239353156b2609330376`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:39:43 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 10:39:45 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:47:42 GMT
ENV RUBY_MAJOR=2.7
# Mon, 05 Apr 2021 19:16:34 GMT
ENV RUBY_VERSION=2.7.3
# Mon, 05 Apr 2021 19:16:34 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Mon, 05 Apr 2021 19:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:20:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:20:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:20:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:21:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:21:02 GMT
CMD ["irb"]
# Mon, 05 Apr 2021 20:44:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Mon, 05 Apr 2021 20:44:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Mon, 05 Apr 2021 20:44:49 GMT
ENV RAILS_ENV=production
# Mon, 05 Apr 2021 20:44:49 GMT
WORKDIR /usr/src/redmine
# Mon, 05 Apr 2021 20:44:49 GMT
ENV HOME=/home/redmine
# Mon, 05 Apr 2021 20:44:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 05 Apr 2021 20:44:51 GMT
ENV REDMINE_VERSION=4.2.0
# Mon, 05 Apr 2021 20:44:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Mon, 05 Apr 2021 20:44:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 05 Apr 2021 20:44:55 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 05 Apr 2021 20:47:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 05 Apr 2021 20:47:14 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 05 Apr 2021 20:47:14 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 05 Apr 2021 20:47:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 05 Apr 2021 20:47:15 GMT
EXPOSE 3000
# Mon, 05 Apr 2021 20:47:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9df2de4dab84e51acacca9e65a3d9f7c9fa2f038bc11c2830bd9a97980823a0`  
		Last Modified: Thu, 01 Apr 2021 11:09:32 GMT  
		Size: 1.2 MB (1218696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc339b259bb6448a756fb9b42044f3450a7dcd6fc3bc0102a3cb6b7594daca19`  
		Last Modified: Thu, 01 Apr 2021 11:09:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bf4c0832c8a73d79344879220b7a99ed4ecccf6eb758384bec64d8719c63b8`  
		Last Modified: Mon, 05 Apr 2021 20:15:04 GMT  
		Size: 23.2 MB (23207724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e0141082ecc3e69444f52c2c25989a96c26e3f1db52ed818a2415be78f134a`  
		Last Modified: Mon, 05 Apr 2021 20:15:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed39d01534357156db6127eb2e8773b4392a8e1f7eeda26f6ee1e2a8e546bab7`  
		Last Modified: Mon, 05 Apr 2021 20:58:52 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a15e47cfeac0ace560ab1a638fc48e9778fd707f93c1e1f0f5ce10485c02ff`  
		Last Modified: Mon, 05 Apr 2021 20:59:04 GMT  
		Size: 69.4 MB (69428125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e444a04c0290dbedcaf3c8c2b51834f611b133a5d3972177b6cf6e8a7a8bd26`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d2998285fcc9b3ccd853c688ece46d699af9032ff15b3ce80d713c179b9ca2`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0bf3df829a8a10618bbfe5772d98aeda38ab59effc18261703062cb5ade296`  
		Last Modified: Mon, 05 Apr 2021 20:58:50 GMT  
		Size: 3.1 MB (3058322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1c7fbf7457fdf8ee116d68493251899d90f8b5d5f7ae60fbcdb6f2580965ec`  
		Last Modified: Mon, 05 Apr 2021 20:58:56 GMT  
		Size: 64.5 MB (64531585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ebb1f89b905c30adc636a07475d0f7e1720a4b3cc15d4ea8e30ab637c91b7e`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-passenger`

```console
$ docker pull redmine@sha256:fb65384f72d4cdfdde814d4251c875f18a880266352429b55ebd579d4c173ee0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.2-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:c079166ff4bd19c8ad9336912641f489b7354401437cd7acee04999530650477
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236801276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f9c99e9a97ac10f42e489199a62f16eb28ae8368a638cd41ad31ecf1c6e5be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 18:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:42:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:42:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:42:59 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:55:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:56:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:56:28 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:56:28 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:56:28 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:56:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:56:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:17 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:57:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:57:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:57:17 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:57:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sun, 11 Apr 2021 06:57:33 GMT
ENV PASSENGER_VERSION=6.0.8
# Sun, 11 Apr 2021 06:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:50 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sun, 11 Apr 2021 06:57:50 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sun, 11 Apr 2021 06:57:50 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1596cf153142005038983af255e0d09ef62c65e139aa5c973c2d2baaa2044b0`  
		Last Modified: Sat, 10 Apr 2021 19:09:47 GMT  
		Size: 22.9 MB (22887036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed63bc8e0386fa836f8cf065b98fa401987445d1ab32e260f00e34398b353c`  
		Last Modified: Sat, 10 Apr 2021 19:09:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6acca6e42a84df58aeac107bc65a7bd29a5a702ca33992837a43d23689e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:20 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1370bc72633d9b6883d4baa5cfe7320f3310950f72f5753966432b3c5fb39af7`  
		Last Modified: Sun, 11 Apr 2021 07:03:35 GMT  
		Size: 93.9 MB (93906284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db1ff6e623ce6c864b167bcc6a6513b6864b9dc79a4d77823597370866a1c4e`  
		Last Modified: Sun, 11 Apr 2021 07:03:21 GMT  
		Size: 1.4 MB (1370219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aafa942955516a5b82908cc908e9fe16aa0e9d25e7c41513563f4d7dcd98e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de8b29a2583f478869875849b6bdc9aa17b8f1cf07835e579284513b946dba`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e2181bd63ce8a24b2330aa48fb52e8188a931903f495caaaaeb4ef6153e86`  
		Last Modified: Sun, 11 Apr 2021 07:03:18 GMT  
		Size: 3.1 MB (3057055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee7416a1645930503313e41e3183303a737aea90454566b7d83fac74e3707`  
		Last Modified: Sun, 11 Apr 2021 07:03:24 GMT  
		Size: 50.6 MB (50574847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f886f325a0ba2239c4905f09d7d6186c89f3202c59614d1181eeecf550cc69`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4e67ce39214f6c91a2e674f89f56c6396296fe4ae2975f2dc24082bfa2db9f`  
		Last Modified: Sun, 11 Apr 2021 07:03:56 GMT  
		Size: 20.4 MB (20363201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd0141a3a34bc643ef0b1a5907467d3643479f4c5bb357ffb15dbff0a695a22`  
		Last Modified: Sun, 11 Apr 2021 07:03:54 GMT  
		Size: 4.9 MB (4936711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.0`

```console
$ docker pull redmine@sha256:d748e2a03c4a6c25772fe3f8349339b0e1963b1ade3c1103fa09c892f3af61fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redmine:4.2.0` - linux; amd64

```console
$ docker pull redmine@sha256:674aaf0691b263a8306a5da9ca763ea706cf9eb73fa97fe5b80880e17e34793e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.5 MB (211501364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9f9e5072432e6d9ac85838768e7d2481b91de8b79dd3010b2d77d4194e7975`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 18:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:42:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:42:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:42:59 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:55:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:56:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:56:28 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:56:28 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:56:28 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:56:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:56:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:17 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:57:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:57:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:57:17 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:57:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1596cf153142005038983af255e0d09ef62c65e139aa5c973c2d2baaa2044b0`  
		Last Modified: Sat, 10 Apr 2021 19:09:47 GMT  
		Size: 22.9 MB (22887036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed63bc8e0386fa836f8cf065b98fa401987445d1ab32e260f00e34398b353c`  
		Last Modified: Sat, 10 Apr 2021 19:09:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6acca6e42a84df58aeac107bc65a7bd29a5a702ca33992837a43d23689e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:20 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1370bc72633d9b6883d4baa5cfe7320f3310950f72f5753966432b3c5fb39af7`  
		Last Modified: Sun, 11 Apr 2021 07:03:35 GMT  
		Size: 93.9 MB (93906284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db1ff6e623ce6c864b167bcc6a6513b6864b9dc79a4d77823597370866a1c4e`  
		Last Modified: Sun, 11 Apr 2021 07:03:21 GMT  
		Size: 1.4 MB (1370219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aafa942955516a5b82908cc908e9fe16aa0e9d25e7c41513563f4d7dcd98e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de8b29a2583f478869875849b6bdc9aa17b8f1cf07835e579284513b946dba`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e2181bd63ce8a24b2330aa48fb52e8188a931903f495caaaaeb4ef6153e86`  
		Last Modified: Sun, 11 Apr 2021 07:03:18 GMT  
		Size: 3.1 MB (3057055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee7416a1645930503313e41e3183303a737aea90454566b7d83fac74e3707`  
		Last Modified: Sun, 11 Apr 2021 07:03:24 GMT  
		Size: 50.6 MB (50574847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f886f325a0ba2239c4905f09d7d6186c89f3202c59614d1181eeecf550cc69`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:c5a5d3160bd8eaf254b337f502de2c7c6eca5e533afaf87013d16ebdcc40c882
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.7 MB (215708994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94de86d41e3b7f9b9c16ef7a058e074b1b018038726598e9151d8ff64b32769f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:34:59 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 07:35:00 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 07:35:01 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 07:38:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:38:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:38:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:38:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:38:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:38:53 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:37:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 17:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:39:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:39:58 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 17:40:01 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 17:40:02 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 17:40:11 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 17:40:11 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 17:40:12 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 17:40:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 17:44:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:44:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 17:44:51 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 17:44:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:44:54 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 17:44:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da9e41f31dbd59278885fc90a21f78df54ac8e0eeaac6cdfc706d58f3e5cbf9`  
		Last Modified: Sat, 10 Apr 2021 08:12:10 GMT  
		Size: 22.1 MB (22135924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738045962dd0fa8676cf7d722f50e91453ae0e03480b28c95a78b29cbe8c1aca`  
		Last Modified: Sat, 10 Apr 2021 08:12:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce548b7edc54230ecd0be27b260538194321967b7d16ef832e6f86b36ec3269c`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4574075c1b7c50bf542b82a25936d688f4f600298ebf34638e46a49915b6cc30`  
		Last Modified: Sat, 10 Apr 2021 17:59:45 GMT  
		Size: 89.5 MB (89482026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1a552ef67d98bc5894cdb93b2a31d6b45c9ba81f13e609629c00d62d5c8cd5`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 1.3 MB (1326336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8e8040892fd65e2920ca520c1f85934ecaf3cac205140f022d26450ddb4e7`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bf7390b6a87b298e37c8f4401109ac9abaa465b693dd974b717848d0557195`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd685807e7eef49564926e681ac910583fdc0032524d07aa1e3c579701924cea`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 3.1 MB (3057047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d377f01a1044a4d648cfe27174049a37901a12adcf773b420a8cb22670008`  
		Last Modified: Sat, 10 Apr 2021 17:59:26 GMT  
		Size: 64.5 MB (64484917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9309b37c7d17afa9ab0ce43eb207cb4c015cf8080e4ef0026f3605f1d63ea4`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:9b090f6a48322643c7aa5cca725c75dbca849e6b72fb179efd17ca1c878c30a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208872054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce4cd6b1e80353141e77cb6b90438a2b128cfa0dc8b26d3541592dc0d371b4fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:30:27 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 16:30:31 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 16:30:37 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 16:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:34:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:34:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:34:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:34:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:34:51 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:36:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:38:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:38:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:38:22 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:38:23 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:38:24 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:38:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:38:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 04:38:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 04:38:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:42:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:42:29 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:42:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:42:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:42:34 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:42:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544200d357634004457e98f7ac1f43b3a31ebffce5d7e19d2ca99541f0a33131`  
		Last Modified: Sat, 10 Apr 2021 17:19:41 GMT  
		Size: 22.0 MB (22018396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9172351c62ca591dae2a838e01000b6c57489cd47d7af7562e3a495a1caf73b7`  
		Last Modified: Sat, 10 Apr 2021 17:19:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09934e285d86d86fd34b9a3e6d7dec0a3c903bc1d3876022959c6fba45f6ffbd`  
		Last Modified: Sun, 11 Apr 2021 04:57:24 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7fc62da65346ee9c7607a212b41cdbf2c0dc5e365e7c18956017fe19fed731`  
		Last Modified: Sun, 11 Apr 2021 04:57:52 GMT  
		Size: 85.5 MB (85517651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1366c02dd0228cb0f5455a819f46c01c72614c8c2c903f30d8da3f4ba7b3eae0`  
		Last Modified: Sun, 11 Apr 2021 04:57:22 GMT  
		Size: 1.3 MB (1319111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6818a0f2ed85db5a6a199a883fbf6e4eb9f5c1ec90f99cf3b39d2b304b1411`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4544ee1e1bc77a527ff800db97c53158ca440f5fa79330dc3c54988c9ef29`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17ee6b4b9725c04744e6bd790ffa5ec91622e224b5cefe433dd05838c6d7aaf`  
		Last Modified: Sun, 11 Apr 2021 04:57:22 GMT  
		Size: 3.1 MB (3057054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea24d2bc0af67d878125d29f6e1e9bd9c69e601e0796cb3d218c66e6e46bec0`  
		Last Modified: Sun, 11 Apr 2021 04:57:38 GMT  
		Size: 64.3 MB (64343712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cf6d83da71cba257a0d5c791bf2cd1d18b7188c3a7c86a1a04362ccfabf95`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:ed7bf06cf7b08eb7ffdc233007259fabb4475c75c3601ceb0c042fc87080db0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222610474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831ae1d31498a4d3370d0b2a75ac9c10ffddf9837dc3cec001c3239efc9874c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:13:06 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 16:13:06 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 16:13:07 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 16:16:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:16:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:16:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:16:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:16:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:16:56 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:36:04 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:37:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:37:31 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:37:32 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:37:33 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:37:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:37:36 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 04:37:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 04:37:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:41:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:41:39 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:41:40 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:41:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:41:42 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:41:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b735094fd3dfe6c2254ce5bc9c940f71df11fa5f06460d079afd191ebc5c674`  
		Last Modified: Sat, 10 Apr 2021 16:49:23 GMT  
		Size: 22.7 MB (22732804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe803a3eac64f3210850b0bff3533351bd47cfcfe47db8de1dfa928d38082cf8`  
		Last Modified: Sat, 10 Apr 2021 16:49:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe02df6b0d5eaba2d093335c1841a204718b89b5937988b73befc4d70e0e65`  
		Last Modified: Sun, 11 Apr 2021 04:55:42 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6b6f8722801008dc9df47485fb2c8de3e8f64b6ffea6ca55a65a322d489582`  
		Last Modified: Sun, 11 Apr 2021 04:56:08 GMT  
		Size: 92.5 MB (92499331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99372a4bd2cbe51d9628e4fb5763221c86530233759f73d039c898f2a3ef983`  
		Last Modified: Sun, 11 Apr 2021 04:55:43 GMT  
		Size: 1.3 MB (1303583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df37457b9b0458d0364314681801996540e1932316815a2d4c6c7d79e313e51`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f4312e5c8dd083d638060fae2e7c29fbc564c923dcbb0fbde7164acd157ea3`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15912641909cdcaec9376c2b88a72afe5e67c5fc2e67e597f8b3dae13f5723cf`  
		Last Modified: Sun, 11 Apr 2021 04:55:42 GMT  
		Size: 3.1 MB (3057038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf21f8a15c6087c8df6dcd1246a8bcc1fc2cb0558cdd6add076415dab67fb76`  
		Last Modified: Sun, 11 Apr 2021 04:55:55 GMT  
		Size: 65.8 MB (65845943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734c10e558c8e573d6e1113e6234bf8a61362235ff0edf48089f2d749422b434`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.0` - linux; 386

```console
$ docker pull redmine@sha256:a7dfbfbcd168473d1c7b59540044e9be1240a86399758af156e9bc5039d266e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217797824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11f3b67e5b83fae70ed263d4bdc62727a2556e4e6a6500b2f8b8372aa991d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:43:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 02:43:52 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 02:43:52 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 02:48:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:48:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:48:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:48:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:48:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:48:10 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:12:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 16:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:13:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:13:37 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 16:13:37 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 16:13:38 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 16:13:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 16:13:39 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 16:13:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 16:13:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 16:14:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:14:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 16:14:37 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 16:14:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 16:14:38 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 16:14:38 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab4999cad906527dc1dec3fd24fa2f63b4cf3360e33768e9a3afaa30af81f7`  
		Last Modified: Sat, 10 Apr 2021 03:12:12 GMT  
		Size: 22.3 MB (22340618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59394b3c951d09cef112094acc41fbd8608139b79afcccf38fe6ab8fa34363c`  
		Last Modified: Sat, 10 Apr 2021 03:12:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4410c086f240a2556c34f99837c171fc5042ee25324d15eed68d6c823d6f2113`  
		Last Modified: Sat, 10 Apr 2021 16:20:40 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0253065be9c93a1dd65d60739959c872d5e54b24ce0278b1b406dcd9a92fe3`  
		Last Modified: Sat, 10 Apr 2021 16:21:04 GMT  
		Size: 95.5 MB (95537702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8174da1366e0c18236b9ff292261c829c40c6f64f8754aaea0a5054378c2163b`  
		Last Modified: Sat, 10 Apr 2021 16:20:40 GMT  
		Size: 1.3 MB (1338943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a85c94e995fd573909579b7e4bc809efcc8a0cd2fa4c52de0b6934660f8f1b9`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761295a090f25492b48fbb3de84b39bcf24c6ea7d9078df49b8b3e10928eb2`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5674eb34390ddbd43c4c23b1f8c317ab1aa39d015b542ff87e8421a51373b543`  
		Last Modified: Sat, 10 Apr 2021 16:20:39 GMT  
		Size: 3.1 MB (3057038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f18b357fea8d540c87223b845dfe4481d83983e189d41dd1eda244160799c3`  
		Last Modified: Sat, 10 Apr 2021 16:20:47 GMT  
		Size: 50.5 MB (50503021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b11c79faef3e548b798c71ffda1c95254e8f0cda712a838cd6fa199162edc71`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.0` - linux; mips64le

```console
$ docker pull redmine@sha256:d8dfe7820f83a620ce99dd6ff63b0846ca72a25d0e9ea0cba169adfbbbfac925
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222021251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:268ae94296a68b7d47b3d70b15e8d1ddd4720476ed9027f05d0f4cae4f73290f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:06:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:16:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:16:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:16:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:16:12 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:15:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:16:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:16:56 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:16:56 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:16:57 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:16:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 19:16:59 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 19:17:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 19:17:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 19:25:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:25:13 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 19:25:13 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 19:25:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 19:25:14 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 19:25:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a308e0916de51c8816bb907b1f46847b9e4f2a4c13ad8496699a943b1cb1192b`  
		Last Modified: Sat, 10 Apr 2021 15:52:29 GMT  
		Size: 23.1 MB (23101289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4aeaf82f75e03c0de4dc8cfbada529330605924f939a89eea76608b649fc61c`  
		Last Modified: Sat, 10 Apr 2021 15:52:19 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d76e50514a47201bc1e5d1ecd34cb3dd052f552ecc3327f756a2ff28e810fd`  
		Last Modified: Sat, 10 Apr 2021 19:44:24 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9894c487a5a062ca596adb69a0c0d1787a83ea05390fc69a9508850fbd0a2aee`  
		Last Modified: Sat, 10 Apr 2021 19:45:32 GMT  
		Size: 90.9 MB (90869502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b429b96dcf10c532cff19eb56cbb9a41a6e88d65179724f8e8d0a175cb4775`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 1.3 MB (1257309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62845c559925cc0291a80649bdc3e23c43fc80a48a73be6a897e6247d616f7ef`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6114ea006b8a2dfe2a8229a601a2f01991affc3feec2a428b26707c99cc92`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866e595f4eb90b05ffa193035de32d77043c97649769baa388e8ed71df9b4c68`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 3.1 MB (3056466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff3272561a535e8b5ba73ff286d51d976cf39ac87092e2f0fa420e43c3712c`  
		Last Modified: Sat, 10 Apr 2021 19:44:56 GMT  
		Size: 66.3 MB (66298266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5a45d6e6fe63215d266dd648b78c69dc5a5ca1f462be021b884fafacfd1f9a`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:613ce7722c4bcd975b4d86b7540bf3add1d5db78ea35459a83abf899bf544501
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239082666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab85f646932584743522c4882cfe4c8d378ae92ff7aea25b2022ea176204f8c6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:57:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:57:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:57:33 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:14:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:14:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:15:05 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:23:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:23:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:23:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:23:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:23:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:23:45 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 05:57:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:05:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:07:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:07:15 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:07:24 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:07:27 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:07:49 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:07:55 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:07:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:08:14 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:13:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:13:32 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:13:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:13:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:13:46 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:13:50 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cbbc810e9494a5dfcf8ee1e195a1a58bd57e76aadf8003b70553ed4eb09b2`  
		Last Modified: Sat, 10 Apr 2021 15:54:53 GMT  
		Size: 12.7 MB (12704371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa4e10ca5b1345262af0a6624b7f9980011d8180575de45104358ed122152a`  
		Last Modified: Sat, 10 Apr 2021 15:54:50 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969b8bec5707756c2c65c42151cedb5ed4aa7cfd90762da603a0c27fc694eb1e`  
		Last Modified: Sat, 10 Apr 2021 15:55:48 GMT  
		Size: 23.4 MB (23414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7799f120e744ecf4af99f5374dd470aed6475ca254813ff9b781f8bd5ee9ba`  
		Last Modified: Sat, 10 Apr 2021 15:55:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17b32b0803cb0c499e8847d76fd9c8188e04f99b0a49d3bb00fb57852da102`  
		Last Modified: Sun, 11 Apr 2021 07:07:58 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04001ba15d9c6379ed6823bd4d279724b7dc9c2c3b1779183e3d5e3cf7ced3e`  
		Last Modified: Sun, 11 Apr 2021 07:08:41 GMT  
		Size: 101.1 MB (101147239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7e01d32f1e67a82e76be158bd1f54e80d8e6d43e082bde15416b0cac68efe`  
		Last Modified: Sun, 11 Apr 2021 07:07:59 GMT  
		Size: 1.3 MB (1290574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579cddd918b5fec468e3a6b5d01ab1113193d9a60fe3f5d11de447084f315b6d`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5181bfb422524a8f6b2eace42ef46cd20f8181d2023edf01874b0d0a5f31bfe`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f706945ab1345126925f34b0a33dcd58dbd84322bd093b64077aa818112f46ee`  
		Last Modified: Sun, 11 Apr 2021 07:07:57 GMT  
		Size: 3.1 MB (3057048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c1a53028ee3ee0723cec0f90306634b171fa7905e55e906839bb7eb8601b4`  
		Last Modified: Sun, 11 Apr 2021 07:08:06 GMT  
		Size: 66.9 MB (66919035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a598556acae8e5996306debd91dadc7da82e6cc011a616f95017b1e043b4ecdb`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.0` - linux; s390x

```console
$ docker pull redmine@sha256:d86d5b58aa7e9dd6dc7547929ce5542856c7580dde88fb5b916c4ae6fc3cee9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222020361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89028240f1dee18298827636e792c7c5a0712b03a6445f2c4b28db0991c314e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:04:20 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 02:04:20 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 02:04:21 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 02:06:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:06:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:06:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:06:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:06:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:06:08 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:31:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 12:32:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:32:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:32:57 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 12:32:58 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 12:32:58 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 12:32:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 12:33:00 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 12:33:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 12:33:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 12:35:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:35:47 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 12:35:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 12:35:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 12:35:48 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 12:35:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3098c63e5609140d293715e979f3576527d20157d2f671592b79736f4d72ddd4`  
		Last Modified: Sat, 10 Apr 2021 02:22:38 GMT  
		Size: 23.1 MB (23066252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3547d43bbb52b78bdbe05cc38cf90175f678f4512422ef47540229443c7a1824`  
		Last Modified: Sat, 10 Apr 2021 02:22:37 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd4d29f072b64c3d7e17a9a81fe61294be125cd7f7c2fee6bddc6b5b61bafe7`  
		Last Modified: Sat, 10 Apr 2021 12:47:53 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4b26acacc50fc4a0c6155d028bde06b918cb698c1eafb066f77c98931b82ca`  
		Last Modified: Sat, 10 Apr 2021 12:48:10 GMT  
		Size: 91.6 MB (91641533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e338871896ec393957d527289b7c3ad84893f5da29ee7152a52c7cc97ccdd05a`  
		Last Modified: Sat, 10 Apr 2021 12:47:53 GMT  
		Size: 1.4 MB (1356207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24b741f8a77912f9f77062871d2a869002331460009e31de96fccbb3604b945`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db5b06d283b2c92a6908585d05e13858d8561b7c61b9c190de9807cd4bf05e4`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e29c0ae231298e90eea6df8a140e4608cff7d379598e181106f9b4de31a517`  
		Last Modified: Sat, 10 Apr 2021 12:47:52 GMT  
		Size: 3.1 MB (3057042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22351124edd3ea56412ba14138a1aafc8eb76b8f7b72842596372b3b8dbf3088`  
		Last Modified: Sat, 10 Apr 2021 12:48:02 GMT  
		Size: 66.3 MB (66327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea92b2f8e559d76b1121c336a586e7884919cb81519ff911a84e78a1e98194`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.0-alpine`

```console
$ docker pull redmine@sha256:29454a31d1cebcdc33cd50b35495532b6756e6608a036133c68263de8089b9a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.2.0-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:9d1c434ac62026273ff39820aad3eb9e532678a54012152712ab1a76311a8139
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.3 MB (164260126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5aa389f0b143c0ea7e350e485f5936594d02e5f31ee239353156b2609330376`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:39:43 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 10:39:45 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:47:42 GMT
ENV RUBY_MAJOR=2.7
# Mon, 05 Apr 2021 19:16:34 GMT
ENV RUBY_VERSION=2.7.3
# Mon, 05 Apr 2021 19:16:34 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Mon, 05 Apr 2021 19:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:20:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:20:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:20:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:21:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:21:02 GMT
CMD ["irb"]
# Mon, 05 Apr 2021 20:44:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Mon, 05 Apr 2021 20:44:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Mon, 05 Apr 2021 20:44:49 GMT
ENV RAILS_ENV=production
# Mon, 05 Apr 2021 20:44:49 GMT
WORKDIR /usr/src/redmine
# Mon, 05 Apr 2021 20:44:49 GMT
ENV HOME=/home/redmine
# Mon, 05 Apr 2021 20:44:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 05 Apr 2021 20:44:51 GMT
ENV REDMINE_VERSION=4.2.0
# Mon, 05 Apr 2021 20:44:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Mon, 05 Apr 2021 20:44:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 05 Apr 2021 20:44:55 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 05 Apr 2021 20:47:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 05 Apr 2021 20:47:14 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 05 Apr 2021 20:47:14 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 05 Apr 2021 20:47:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 05 Apr 2021 20:47:15 GMT
EXPOSE 3000
# Mon, 05 Apr 2021 20:47:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9df2de4dab84e51acacca9e65a3d9f7c9fa2f038bc11c2830bd9a97980823a0`  
		Last Modified: Thu, 01 Apr 2021 11:09:32 GMT  
		Size: 1.2 MB (1218696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc339b259bb6448a756fb9b42044f3450a7dcd6fc3bc0102a3cb6b7594daca19`  
		Last Modified: Thu, 01 Apr 2021 11:09:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bf4c0832c8a73d79344879220b7a99ed4ecccf6eb758384bec64d8719c63b8`  
		Last Modified: Mon, 05 Apr 2021 20:15:04 GMT  
		Size: 23.2 MB (23207724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e0141082ecc3e69444f52c2c25989a96c26e3f1db52ed818a2415be78f134a`  
		Last Modified: Mon, 05 Apr 2021 20:15:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed39d01534357156db6127eb2e8773b4392a8e1f7eeda26f6ee1e2a8e546bab7`  
		Last Modified: Mon, 05 Apr 2021 20:58:52 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a15e47cfeac0ace560ab1a638fc48e9778fd707f93c1e1f0f5ce10485c02ff`  
		Last Modified: Mon, 05 Apr 2021 20:59:04 GMT  
		Size: 69.4 MB (69428125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e444a04c0290dbedcaf3c8c2b51834f611b133a5d3972177b6cf6e8a7a8bd26`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d2998285fcc9b3ccd853c688ece46d699af9032ff15b3ce80d713c179b9ca2`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0bf3df829a8a10618bbfe5772d98aeda38ab59effc18261703062cb5ade296`  
		Last Modified: Mon, 05 Apr 2021 20:58:50 GMT  
		Size: 3.1 MB (3058322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1c7fbf7457fdf8ee116d68493251899d90f8b5d5f7ae60fbcdb6f2580965ec`  
		Last Modified: Mon, 05 Apr 2021 20:58:56 GMT  
		Size: 64.5 MB (64531585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ebb1f89b905c30adc636a07475d0f7e1720a4b3cc15d4ea8e30ab637c91b7e`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.0-passenger`

```console
$ docker pull redmine@sha256:fb65384f72d4cdfdde814d4251c875f18a880266352429b55ebd579d4c173ee0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.2.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:c079166ff4bd19c8ad9336912641f489b7354401437cd7acee04999530650477
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236801276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f9c99e9a97ac10f42e489199a62f16eb28ae8368a638cd41ad31ecf1c6e5be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 18:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:42:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:42:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:42:59 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:55:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:56:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:56:28 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:56:28 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:56:28 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:56:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:56:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:17 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:57:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:57:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:57:17 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:57:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sun, 11 Apr 2021 06:57:33 GMT
ENV PASSENGER_VERSION=6.0.8
# Sun, 11 Apr 2021 06:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:50 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sun, 11 Apr 2021 06:57:50 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sun, 11 Apr 2021 06:57:50 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1596cf153142005038983af255e0d09ef62c65e139aa5c973c2d2baaa2044b0`  
		Last Modified: Sat, 10 Apr 2021 19:09:47 GMT  
		Size: 22.9 MB (22887036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed63bc8e0386fa836f8cf065b98fa401987445d1ab32e260f00e34398b353c`  
		Last Modified: Sat, 10 Apr 2021 19:09:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6acca6e42a84df58aeac107bc65a7bd29a5a702ca33992837a43d23689e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:20 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1370bc72633d9b6883d4baa5cfe7320f3310950f72f5753966432b3c5fb39af7`  
		Last Modified: Sun, 11 Apr 2021 07:03:35 GMT  
		Size: 93.9 MB (93906284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db1ff6e623ce6c864b167bcc6a6513b6864b9dc79a4d77823597370866a1c4e`  
		Last Modified: Sun, 11 Apr 2021 07:03:21 GMT  
		Size: 1.4 MB (1370219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aafa942955516a5b82908cc908e9fe16aa0e9d25e7c41513563f4d7dcd98e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de8b29a2583f478869875849b6bdc9aa17b8f1cf07835e579284513b946dba`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e2181bd63ce8a24b2330aa48fb52e8188a931903f495caaaaeb4ef6153e86`  
		Last Modified: Sun, 11 Apr 2021 07:03:18 GMT  
		Size: 3.1 MB (3057055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee7416a1645930503313e41e3183303a737aea90454566b7d83fac74e3707`  
		Last Modified: Sun, 11 Apr 2021 07:03:24 GMT  
		Size: 50.6 MB (50574847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f886f325a0ba2239c4905f09d7d6186c89f3202c59614d1181eeecf550cc69`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4e67ce39214f6c91a2e674f89f56c6396296fe4ae2975f2dc24082bfa2db9f`  
		Last Modified: Sun, 11 Apr 2021 07:03:56 GMT  
		Size: 20.4 MB (20363201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd0141a3a34bc643ef0b1a5907467d3643479f4c5bb357ffb15dbff0a695a22`  
		Last Modified: Sun, 11 Apr 2021 07:03:54 GMT  
		Size: 4.9 MB (4936711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:alpine`

```console
$ docker pull redmine@sha256:29454a31d1cebcdc33cd50b35495532b6756e6608a036133c68263de8089b9a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:9d1c434ac62026273ff39820aad3eb9e532678a54012152712ab1a76311a8139
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **164.3 MB (164260126 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5aa389f0b143c0ea7e350e485f5936594d02e5f31ee239353156b2609330376`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:39:43 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 01 Apr 2021 10:39:45 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 10:47:42 GMT
ENV RUBY_MAJOR=2.7
# Mon, 05 Apr 2021 19:16:34 GMT
ENV RUBY_VERSION=2.7.3
# Mon, 05 Apr 2021 19:16:34 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Mon, 05 Apr 2021 19:20:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Mon, 05 Apr 2021 19:20:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Mon, 05 Apr 2021 19:20:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Mon, 05 Apr 2021 19:20:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 05 Apr 2021 19:21:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Mon, 05 Apr 2021 19:21:02 GMT
CMD ["irb"]
# Mon, 05 Apr 2021 20:44:40 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Mon, 05 Apr 2021 20:44:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Mon, 05 Apr 2021 20:44:49 GMT
ENV RAILS_ENV=production
# Mon, 05 Apr 2021 20:44:49 GMT
WORKDIR /usr/src/redmine
# Mon, 05 Apr 2021 20:44:49 GMT
ENV HOME=/home/redmine
# Mon, 05 Apr 2021 20:44:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 05 Apr 2021 20:44:51 GMT
ENV REDMINE_VERSION=4.2.0
# Mon, 05 Apr 2021 20:44:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Mon, 05 Apr 2021 20:44:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 05 Apr 2021 20:44:55 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 05 Apr 2021 20:47:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 05 Apr 2021 20:47:14 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 05 Apr 2021 20:47:14 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 05 Apr 2021 20:47:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 05 Apr 2021 20:47:15 GMT
EXPOSE 3000
# Mon, 05 Apr 2021 20:47:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9df2de4dab84e51acacca9e65a3d9f7c9fa2f038bc11c2830bd9a97980823a0`  
		Last Modified: Thu, 01 Apr 2021 11:09:32 GMT  
		Size: 1.2 MB (1218696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc339b259bb6448a756fb9b42044f3450a7dcd6fc3bc0102a3cb6b7594daca19`  
		Last Modified: Thu, 01 Apr 2021 11:09:34 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67bf4c0832c8a73d79344879220b7a99ed4ecccf6eb758384bec64d8719c63b8`  
		Last Modified: Mon, 05 Apr 2021 20:15:04 GMT  
		Size: 23.2 MB (23207724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e0141082ecc3e69444f52c2c25989a96c26e3f1db52ed818a2415be78f134a`  
		Last Modified: Mon, 05 Apr 2021 20:15:02 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed39d01534357156db6127eb2e8773b4392a8e1f7eeda26f6ee1e2a8e546bab7`  
		Last Modified: Mon, 05 Apr 2021 20:58:52 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a15e47cfeac0ace560ab1a638fc48e9778fd707f93c1e1f0f5ce10485c02ff`  
		Last Modified: Mon, 05 Apr 2021 20:59:04 GMT  
		Size: 69.4 MB (69428125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e444a04c0290dbedcaf3c8c2b51834f611b133a5d3972177b6cf6e8a7a8bd26`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d2998285fcc9b3ccd853c688ece46d699af9032ff15b3ce80d713c179b9ca2`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0bf3df829a8a10618bbfe5772d98aeda38ab59effc18261703062cb5ade296`  
		Last Modified: Mon, 05 Apr 2021 20:58:50 GMT  
		Size: 3.1 MB (3058322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1c7fbf7457fdf8ee116d68493251899d90f8b5d5f7ae60fbcdb6f2580965ec`  
		Last Modified: Mon, 05 Apr 2021 20:58:56 GMT  
		Size: 64.5 MB (64531585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ebb1f89b905c30adc636a07475d0f7e1720a4b3cc15d4ea8e30ab637c91b7e`  
		Last Modified: Mon, 05 Apr 2021 20:58:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:latest`

```console
$ docker pull redmine@sha256:d748e2a03c4a6c25772fe3f8349339b0e1963b1ade3c1103fa09c892f3af61fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `redmine:latest` - linux; amd64

```console
$ docker pull redmine@sha256:674aaf0691b263a8306a5da9ca763ea706cf9eb73fa97fe5b80880e17e34793e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.5 MB (211501364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b9f9e5072432e6d9ac85838768e7d2481b91de8b79dd3010b2d77d4194e7975`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 18:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:42:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:42:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:42:59 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:55:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:56:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:56:28 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:56:28 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:56:28 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:56:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:56:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:17 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:57:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:57:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:57:17 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:57:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1596cf153142005038983af255e0d09ef62c65e139aa5c973c2d2baaa2044b0`  
		Last Modified: Sat, 10 Apr 2021 19:09:47 GMT  
		Size: 22.9 MB (22887036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed63bc8e0386fa836f8cf065b98fa401987445d1ab32e260f00e34398b353c`  
		Last Modified: Sat, 10 Apr 2021 19:09:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6acca6e42a84df58aeac107bc65a7bd29a5a702ca33992837a43d23689e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:20 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1370bc72633d9b6883d4baa5cfe7320f3310950f72f5753966432b3c5fb39af7`  
		Last Modified: Sun, 11 Apr 2021 07:03:35 GMT  
		Size: 93.9 MB (93906284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db1ff6e623ce6c864b167bcc6a6513b6864b9dc79a4d77823597370866a1c4e`  
		Last Modified: Sun, 11 Apr 2021 07:03:21 GMT  
		Size: 1.4 MB (1370219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aafa942955516a5b82908cc908e9fe16aa0e9d25e7c41513563f4d7dcd98e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de8b29a2583f478869875849b6bdc9aa17b8f1cf07835e579284513b946dba`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e2181bd63ce8a24b2330aa48fb52e8188a931903f495caaaaeb4ef6153e86`  
		Last Modified: Sun, 11 Apr 2021 07:03:18 GMT  
		Size: 3.1 MB (3057055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee7416a1645930503313e41e3183303a737aea90454566b7d83fac74e3707`  
		Last Modified: Sun, 11 Apr 2021 07:03:24 GMT  
		Size: 50.6 MB (50574847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f886f325a0ba2239c4905f09d7d6186c89f3202c59614d1181eeecf550cc69`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:c5a5d3160bd8eaf254b337f502de2c7c6eca5e533afaf87013d16ebdcc40c882
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.7 MB (215708994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94de86d41e3b7f9b9c16ef7a058e074b1b018038726598e9151d8ff64b32769f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:51:31 GMT
ADD file:926533a23a69aa2481a9122b667bb6300a347154eea366c9e679a230aa7f373a in / 
# Sat, 10 Apr 2021 00:51:34 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 07:27:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 07:27:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 07:27:10 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 07:34:59 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 07:35:00 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 07:35:01 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 07:38:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 07:38:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 07:38:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 07:38:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 07:38:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 07:38:53 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 17:37:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 17:38:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 17:39:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:39:58 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 17:40:01 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 17:40:02 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 17:40:11 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 17:40:11 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 17:40:12 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 17:40:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 17:44:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 17:44:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 17:44:51 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 17:44:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 17:44:54 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 17:44:54 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:33d77752597b664d047cc829e58a223d6fb077b61f69ca0462fcfb9b78d5f69b`  
		Last Modified: Sat, 10 Apr 2021 00:59:22 GMT  
		Size: 24.9 MB (24873199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e8fc93885ff1edc1fec20b799c1c02e672d75d967815f7a98ffe7cb94969e2`  
		Last Modified: Sat, 10 Apr 2021 08:11:28 GMT  
		Size: 10.3 MB (10345305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8dfdecedfe5bd31f7499d5973d09b2665408cca73a9e1f83fea87d261763e6a`  
		Last Modified: Sat, 10 Apr 2021 08:11:23 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da9e41f31dbd59278885fc90a21f78df54ac8e0eeaac6cdfc706d58f3e5cbf9`  
		Last Modified: Sat, 10 Apr 2021 08:12:10 GMT  
		Size: 22.1 MB (22135924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738045962dd0fa8676cf7d722f50e91453ae0e03480b28c95a78b29cbe8c1aca`  
		Last Modified: Sat, 10 Apr 2021 08:12:05 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce548b7edc54230ecd0be27b260538194321967b7d16ef832e6f86b36ec3269c`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4574075c1b7c50bf542b82a25936d688f4f600298ebf34638e46a49915b6cc30`  
		Last Modified: Sat, 10 Apr 2021 17:59:45 GMT  
		Size: 89.5 MB (89482026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1a552ef67d98bc5894cdb93b2a31d6b45c9ba81f13e609629c00d62d5c8cd5`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 1.3 MB (1326336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a8e8040892fd65e2920ca520c1f85934ecaf3cac205140f022d26450ddb4e7`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bf7390b6a87b298e37c8f4401109ac9abaa465b693dd974b717848d0557195`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd685807e7eef49564926e681ac910583fdc0032524d07aa1e3c579701924cea`  
		Last Modified: Sat, 10 Apr 2021 17:59:13 GMT  
		Size: 3.1 MB (3057047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3d377f01a1044a4d648cfe27174049a37901a12adcf773b420a8cb22670008`  
		Last Modified: Sat, 10 Apr 2021 17:59:26 GMT  
		Size: 64.5 MB (64484917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c9309b37c7d17afa9ab0ce43eb207cb4c015cf8080e4ef0026f3605f1d63ea4`  
		Last Modified: Sat, 10 Apr 2021 17:59:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:9b090f6a48322643c7aa5cca725c75dbca849e6b72fb179efd17ca1c878c30a9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.9 MB (208872054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce4cd6b1e80353141e77cb6b90438a2b128cfa0dc8b26d3541592dc0d371b4fb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:45 GMT
ADD file:3fbd246a2de82566bcaaf62e3e0bf57175a7ad46b4156366a110661b31eab240 in / 
# Sat, 10 Apr 2021 00:59:47 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:21:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:21:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:21:36 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:30:27 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 16:30:31 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 16:30:37 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 16:34:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:34:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:34:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:34:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:34:48 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:34:51 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:36:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:38:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:38:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:38:22 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:38:23 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:38:24 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:38:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:38:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 04:38:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 04:38:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:42:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:42:29 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:42:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:42:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:42:34 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:42:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8c6bea184b33030fb923c3c09d634b73235dec3fe2d411db9fd22bda669f2c37`  
		Last Modified: Sat, 10 Apr 2021 01:07:51 GMT  
		Size: 22.7 MB (22739801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32a96003e74381aa8f941ca04050bac2ef44601573854f0c1f244c3a9e17d01`  
		Last Modified: Sat, 10 Apr 2021 17:18:43 GMT  
		Size: 9.9 MB (9872091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdc0d94d9639f64cb041cc65c24a66a9861b8c0ffba33a6eaa17b08d4b7ee1f`  
		Last Modified: Sat, 10 Apr 2021 17:18:36 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:544200d357634004457e98f7ac1f43b3a31ebffce5d7e19d2ca99541f0a33131`  
		Last Modified: Sat, 10 Apr 2021 17:19:41 GMT  
		Size: 22.0 MB (22018396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9172351c62ca591dae2a838e01000b6c57489cd47d7af7562e3a495a1caf73b7`  
		Last Modified: Sat, 10 Apr 2021 17:19:32 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09934e285d86d86fd34b9a3e6d7dec0a3c903bc1d3876022959c6fba45f6ffbd`  
		Last Modified: Sun, 11 Apr 2021 04:57:24 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7fc62da65346ee9c7607a212b41cdbf2c0dc5e365e7c18956017fe19fed731`  
		Last Modified: Sun, 11 Apr 2021 04:57:52 GMT  
		Size: 85.5 MB (85517651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1366c02dd0228cb0f5455a819f46c01c72614c8c2c903f30d8da3f4ba7b3eae0`  
		Last Modified: Sun, 11 Apr 2021 04:57:22 GMT  
		Size: 1.3 MB (1319111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d6818a0f2ed85db5a6a199a883fbf6e4eb9f5c1ec90f99cf3b39d2b304b1411`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a4544ee1e1bc77a527ff800db97c53158ca440f5fa79330dc3c54988c9ef29`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17ee6b4b9725c04744e6bd790ffa5ec91622e224b5cefe433dd05838c6d7aaf`  
		Last Modified: Sun, 11 Apr 2021 04:57:22 GMT  
		Size: 3.1 MB (3057054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea24d2bc0af67d878125d29f6e1e9bd9c69e601e0796cb3d218c66e6e46bec0`  
		Last Modified: Sun, 11 Apr 2021 04:57:38 GMT  
		Size: 64.3 MB (64343712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5cf6d83da71cba257a0d5c791bf2cd1d18b7188c3a7c86a1a04362ccfabf95`  
		Last Modified: Sun, 11 Apr 2021 04:57:20 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:ed7bf06cf7b08eb7ffdc233007259fabb4475c75c3601ceb0c042fc87080db0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.6 MB (222610474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:831ae1d31498a4d3370d0b2a75ac9c10ffddf9837dc3cec001c3239efc9874c0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:41:25 GMT
ADD file:b24da7eb23eeae04e00d0e45da29a89fe8f992e8dcf4ba482afb907b8015b7bf in / 
# Sat, 10 Apr 2021 00:41:28 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 16:05:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:05:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 16:05:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 16:13:06 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 16:13:06 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 16:13:07 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 16:16:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 16:16:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 16:16:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 16:16:52 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 16:16:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 16:16:56 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 04:36:04 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 04:37:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 04:37:30 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:37:31 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 04:37:32 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 04:37:33 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 04:37:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 04:37:36 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 04:37:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 04:37:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 04:41:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 04:41:39 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 04:41:40 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 04:41:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 04:41:42 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 04:41:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:15cb40b9c4df1a06940dc2a154c3be46844241235c1a091afa70da0ee2dc811a`  
		Last Modified: Sat, 10 Apr 2021 00:47:53 GMT  
		Size: 25.9 MB (25904582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d289ca2f3e2b5ab2015b85f9cc2daf060bc66943eb934d2c4bdabcbae6031b1`  
		Last Modified: Sat, 10 Apr 2021 16:48:38 GMT  
		Size: 11.3 MB (11262944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64dbc8b87c2241a1b73e9420a04309883e1c2157144321db6bef67d5ca1f651d`  
		Last Modified: Sat, 10 Apr 2021 16:48:34 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b735094fd3dfe6c2254ce5bc9c940f71df11fa5f06460d079afd191ebc5c674`  
		Last Modified: Sat, 10 Apr 2021 16:49:23 GMT  
		Size: 22.7 MB (22732804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe803a3eac64f3210850b0bff3533351bd47cfcfe47db8de1dfa928d38082cf8`  
		Last Modified: Sat, 10 Apr 2021 16:49:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebe02df6b0d5eaba2d093335c1841a204718b89b5937988b73befc4d70e0e65`  
		Last Modified: Sun, 11 Apr 2021 04:55:42 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6b6f8722801008dc9df47485fb2c8de3e8f64b6ffea6ca55a65a322d489582`  
		Last Modified: Sun, 11 Apr 2021 04:56:08 GMT  
		Size: 92.5 MB (92499331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99372a4bd2cbe51d9628e4fb5763221c86530233759f73d039c898f2a3ef983`  
		Last Modified: Sun, 11 Apr 2021 04:55:43 GMT  
		Size: 1.3 MB (1303583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df37457b9b0458d0364314681801996540e1932316815a2d4c6c7d79e313e51`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f4312e5c8dd083d638060fae2e7c29fbc564c923dcbb0fbde7164acd157ea3`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15912641909cdcaec9376c2b88a72afe5e67c5fc2e67e597f8b3dae13f5723cf`  
		Last Modified: Sun, 11 Apr 2021 04:55:42 GMT  
		Size: 3.1 MB (3057038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf21f8a15c6087c8df6dcd1246a8bcc1fc2cb0558cdd6add076415dab67fb76`  
		Last Modified: Sun, 11 Apr 2021 04:55:55 GMT  
		Size: 65.8 MB (65845943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734c10e558c8e573d6e1113e6234bf8a61362235ff0edf48089f2d749422b434`  
		Last Modified: Sun, 11 Apr 2021 04:55:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:a7dfbfbcd168473d1c7b59540044e9be1240a86399758af156e9bc5039d266e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217797824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c11f3b67e5b83fae70ed263d4bdc62727a2556e4e6a6500b2f8b8372aa991d81`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:42 GMT
ADD file:8885d4d13678543780bb04ba14b621179665f7951d5b261036a7092df9b376e7 in / 
# Sat, 10 Apr 2021 00:39:43 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 02:38:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 02:38:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 02:38:26 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:43:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 02:43:52 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 02:43:52 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 02:48:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:48:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:48:08 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:48:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:48:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:48:10 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 16:12:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 16:13:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 16:13:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:13:37 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 16:13:37 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 16:13:38 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 16:13:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 16:13:39 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 16:13:39 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 16:13:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 16:14:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 16:14:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 16:14:37 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 16:14:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 16:14:38 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 16:14:38 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7cc57a8772e5e479618650dfa70f315b474d3f205d04bde7f602f469c1928d84`  
		Last Modified: Sat, 10 Apr 2021 00:46:07 GMT  
		Size: 27.8 MB (27788987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad0fd260b5f4b604c9bfbc66ee8946e4667087566a076e75b234faaf8363fb9`  
		Last Modified: Sat, 10 Apr 2021 03:11:07 GMT  
		Size: 17.2 MB (17227278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f03815f2ae14591c00fdb7535113d4355263d840a9c34469ae708aea2e74966`  
		Last Modified: Sat, 10 Apr 2021 03:11:00 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ab4999cad906527dc1dec3fd24fa2f63b4cf3360e33768e9a3afaa30af81f7`  
		Last Modified: Sat, 10 Apr 2021 03:12:12 GMT  
		Size: 22.3 MB (22340618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59394b3c951d09cef112094acc41fbd8608139b79afcccf38fe6ab8fa34363c`  
		Last Modified: Sat, 10 Apr 2021 03:12:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4410c086f240a2556c34f99837c171fc5042ee25324d15eed68d6c823d6f2113`  
		Last Modified: Sat, 10 Apr 2021 16:20:40 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0253065be9c93a1dd65d60739959c872d5e54b24ce0278b1b406dcd9a92fe3`  
		Last Modified: Sat, 10 Apr 2021 16:21:04 GMT  
		Size: 95.5 MB (95537702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8174da1366e0c18236b9ff292261c829c40c6f64f8754aaea0a5054378c2163b`  
		Last Modified: Sat, 10 Apr 2021 16:20:40 GMT  
		Size: 1.3 MB (1338943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a85c94e995fd573909579b7e4bc809efcc8a0cd2fa4c52de0b6934660f8f1b9`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95761295a090f25492b48fbb3de84b39bcf24c6ea7d9078df49b8b3e10928eb2`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5674eb34390ddbd43c4c23b1f8c317ab1aa39d015b542ff87e8421a51373b543`  
		Last Modified: Sat, 10 Apr 2021 16:20:39 GMT  
		Size: 3.1 MB (3057038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f18b357fea8d540c87223b845dfe4481d83983e189d41dd1eda244160799c3`  
		Last Modified: Sat, 10 Apr 2021 16:20:47 GMT  
		Size: 50.5 MB (50503021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b11c79faef3e548b798c71ffda1c95254e8f0cda712a838cd6fa199162edc71`  
		Last Modified: Sat, 10 Apr 2021 16:20:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; mips64le

```console
$ docker pull redmine@sha256:d8dfe7820f83a620ce99dd6ff63b0846ca72a25d0e9ea0cba169adfbbbfac925
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222021251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:268ae94296a68b7d47b3d70b15e8d1ddd4720476ed9027f05d0f4cae4f73290f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:09:40 GMT
ADD file:0c93801c4a3719dfd4c047d7f2f4d52bf463eba2ab875da1dc54dcc832aae20b in / 
# Sat, 10 Apr 2021 01:09:41 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:48:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:48:09 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:06:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:06:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:16:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:16:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:16:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:16:12 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:16:12 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 19:15:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 19:16:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 19:16:56 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:16:56 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 19:16:56 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 19:16:57 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 19:16:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 19:16:59 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 19:17:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 19:17:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 19:25:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 19:25:13 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 19:25:13 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 19:25:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 19:25:14 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 19:25:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:09ea659ba566d9c3c62493e5ae0b964f1eee4fcf35aabc91c5c34ca1ad686541`  
		Last Modified: Sat, 10 Apr 2021 01:16:07 GMT  
		Size: 25.8 MB (25806410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0888f81cd19c2edf0d0fe84f5fb1dba53940bd1982c5e95c9ceaf4ad72aa0311`  
		Last Modified: Sat, 10 Apr 2021 15:51:16 GMT  
		Size: 11.6 MB (11627864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e50bd4635b27785e7856718cc2f506fba501fc95d94824bbe542e751541e73c`  
		Last Modified: Sat, 10 Apr 2021 15:51:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a308e0916de51c8816bb907b1f46847b9e4f2a4c13ad8496699a943b1cb1192b`  
		Last Modified: Sat, 10 Apr 2021 15:52:29 GMT  
		Size: 23.1 MB (23101289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4aeaf82f75e03c0de4dc8cfbada529330605924f939a89eea76608b649fc61c`  
		Last Modified: Sat, 10 Apr 2021 15:52:19 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d76e50514a47201bc1e5d1ecd34cb3dd052f552ecc3327f756a2ff28e810fd`  
		Last Modified: Sat, 10 Apr 2021 19:44:24 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9894c487a5a062ca596adb69a0c0d1787a83ea05390fc69a9508850fbd0a2aee`  
		Last Modified: Sat, 10 Apr 2021 19:45:32 GMT  
		Size: 90.9 MB (90869502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b429b96dcf10c532cff19eb56cbb9a41a6e88d65179724f8e8d0a175cb4775`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 1.3 MB (1257309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62845c559925cc0291a80649bdc3e23c43fc80a48a73be6a897e6247d616f7ef`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6114ea006b8a2dfe2a8229a601a2f01991affc3feec2a428b26707c99cc92`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866e595f4eb90b05ffa193035de32d77043c97649769baa388e8ed71df9b4c68`  
		Last Modified: Sat, 10 Apr 2021 19:44:25 GMT  
		Size: 3.1 MB (3056466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ff3272561a535e8b5ba73ff286d51d976cf39ac87092e2f0fa420e43c3712c`  
		Last Modified: Sat, 10 Apr 2021 19:44:56 GMT  
		Size: 66.3 MB (66298266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5a45d6e6fe63215d266dd648b78c69dc5a5ca1f462be021b884fafacfd1f9a`  
		Last Modified: Sat, 10 Apr 2021 19:44:21 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:613ce7722c4bcd975b4d86b7540bf3add1d5db78ea35459a83abf899bf544501
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.1 MB (239082666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab85f646932584743522c4882cfe4c8d378ae92ff7aea25b2022ea176204f8c6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:49 GMT
ADD file:ab87d4854aa8628ce8f4e603c0496499f6f28c3d2525ace782c7369691dafc8c in / 
# Sat, 10 Apr 2021 01:26:56 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 14:57:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 14:57:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 14:57:33 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 15:14:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 15:14:57 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 15:15:05 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 15:23:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 15:23:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 15:23:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 15:23:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 15:23:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 15:23:45 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 05:57:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:05:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:07:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:07:15 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:07:24 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:07:27 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:07:49 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:07:55 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:07:59 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:08:14 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:13:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:13:32 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:13:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:13:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:13:46 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:13:50 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3e1e599482ca47095f85e429b346b76375aa85015ddcca050e85c2a8b1fdda9c`  
		Last Modified: Sat, 10 Apr 2021 01:33:57 GMT  
		Size: 30.5 MB (30545933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250cbbc810e9494a5dfcf8ee1e195a1a58bd57e76aadf8003b70553ed4eb09b2`  
		Last Modified: Sat, 10 Apr 2021 15:54:53 GMT  
		Size: 12.7 MB (12704371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2aa4e10ca5b1345262af0a6624b7f9980011d8180575de45104358ed122152a`  
		Last Modified: Sat, 10 Apr 2021 15:54:50 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969b8bec5707756c2c65c42151cedb5ed4aa7cfd90762da603a0c27fc694eb1e`  
		Last Modified: Sat, 10 Apr 2021 15:55:48 GMT  
		Size: 23.4 MB (23414213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d7799f120e744ecf4af99f5374dd470aed6475ca254813ff9b781f8bd5ee9ba`  
		Last Modified: Sat, 10 Apr 2021 15:55:44 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d17b32b0803cb0c499e8847d76fd9c8188e04f99b0a49d3bb00fb57852da102`  
		Last Modified: Sun, 11 Apr 2021 07:07:58 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04001ba15d9c6379ed6823bd4d279724b7dc9c2c3b1779183e3d5e3cf7ced3e`  
		Last Modified: Sun, 11 Apr 2021 07:08:41 GMT  
		Size: 101.1 MB (101147239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7e01d32f1e67a82e76be158bd1f54e80d8e6d43e082bde15416b0cac68efe`  
		Last Modified: Sun, 11 Apr 2021 07:07:59 GMT  
		Size: 1.3 MB (1290574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579cddd918b5fec468e3a6b5d01ab1113193d9a60fe3f5d11de447084f315b6d`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5181bfb422524a8f6b2eace42ef46cd20f8181d2023edf01874b0d0a5f31bfe`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f706945ab1345126925f34b0a33dcd58dbd84322bd093b64077aa818112f46ee`  
		Last Modified: Sun, 11 Apr 2021 07:07:57 GMT  
		Size: 3.1 MB (3057048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201c1a53028ee3ee0723cec0f90306634b171fa7905e55e906839bb7eb8601b4`  
		Last Modified: Sun, 11 Apr 2021 07:08:06 GMT  
		Size: 66.9 MB (66919035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a598556acae8e5996306debd91dadc7da82e6cc011a616f95017b1e043b4ecdb`  
		Last Modified: Sun, 11 Apr 2021 07:07:55 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:d86d5b58aa7e9dd6dc7547929ce5542856c7580dde88fb5b916c4ae6fc3cee9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **222.0 MB (222020361 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89028240f1dee18298827636e792c7c5a0712b03a6445f2c4b28db0991c314e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:23 GMT
ADD file:dbe2182f8699f2a6011413ea01862e6c0e85853d922dffd72a28d994d23c79bc in / 
# Sat, 10 Apr 2021 00:42:25 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 01:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 01:51:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 01:51:46 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 02:04:20 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 02:04:20 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 02:04:21 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 02:06:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 02:06:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 02:06:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 02:06:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 02:06:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 02:06:08 GMT
CMD ["irb"]
# Sat, 10 Apr 2021 12:31:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 10 Apr 2021 12:32:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 12:32:57 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:32:57 GMT
ENV RAILS_ENV=production
# Sat, 10 Apr 2021 12:32:58 GMT
WORKDIR /usr/src/redmine
# Sat, 10 Apr 2021 12:32:58 GMT
ENV HOME=/home/redmine
# Sat, 10 Apr 2021 12:32:59 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 10 Apr 2021 12:33:00 GMT
ENV REDMINE_VERSION=4.2.0
# Sat, 10 Apr 2021 12:33:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sat, 10 Apr 2021 12:33:06 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 10 Apr 2021 12:35:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 10 Apr 2021 12:35:47 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 10 Apr 2021 12:35:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 10 Apr 2021 12:35:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 10 Apr 2021 12:35:48 GMT
EXPOSE 3000
# Sat, 10 Apr 2021 12:35:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65291f8717b3afd99b63cee867dd3e06b956a8ee6aa8580cc31d913b25de209d`  
		Last Modified: Sat, 10 Apr 2021 00:45:48 GMT  
		Size: 25.8 MB (25753787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c1e1850cea86d76ca69c7e014fa38730a01b6a7a6e1957745093b641be6947`  
		Last Modified: Sat, 10 Apr 2021 02:22:13 GMT  
		Size: 10.8 MB (10814272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9c5f18b62b368568a1040cba71445a611715e0c1d813045988453b628a8cec6`  
		Last Modified: Sat, 10 Apr 2021 02:22:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3098c63e5609140d293715e979f3576527d20157d2f671592b79736f4d72ddd4`  
		Last Modified: Sat, 10 Apr 2021 02:22:38 GMT  
		Size: 23.1 MB (23066252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3547d43bbb52b78bdbe05cc38cf90175f678f4512422ef47540229443c7a1824`  
		Last Modified: Sat, 10 Apr 2021 02:22:37 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd4d29f072b64c3d7e17a9a81fe61294be125cd7f7c2fee6bddc6b5b61bafe7`  
		Last Modified: Sat, 10 Apr 2021 12:47:53 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da4b26acacc50fc4a0c6155d028bde06b918cb698c1eafb066f77c98931b82ca`  
		Last Modified: Sat, 10 Apr 2021 12:48:10 GMT  
		Size: 91.6 MB (91641533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e338871896ec393957d527289b7c3ad84893f5da29ee7152a52c7cc97ccdd05a`  
		Last Modified: Sat, 10 Apr 2021 12:47:53 GMT  
		Size: 1.4 MB (1356207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24b741f8a77912f9f77062871d2a869002331460009e31de96fccbb3604b945`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db5b06d283b2c92a6908585d05e13858d8561b7c61b9c190de9807cd4bf05e4`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e29c0ae231298e90eea6df8a140e4608cff7d379598e181106f9b4de31a517`  
		Last Modified: Sat, 10 Apr 2021 12:47:52 GMT  
		Size: 3.1 MB (3057042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22351124edd3ea56412ba14138a1aafc8eb76b8f7b72842596372b3b8dbf3088`  
		Last Modified: Sat, 10 Apr 2021 12:48:02 GMT  
		Size: 66.3 MB (66327023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2ea92b2f8e559d76b1121c336a586e7884919cb81519ff911a84e78a1e98194`  
		Last Modified: Sat, 10 Apr 2021 12:47:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:passenger`

```console
$ docker pull redmine@sha256:fb65384f72d4cdfdde814d4251c875f18a880266352429b55ebd579d4c173ee0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:c079166ff4bd19c8ad9336912641f489b7354401437cd7acee04999530650477
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.8 MB (236801276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56f9c99e9a97ac10f42e489199a62f16eb28ae8368a638cd41ad31ecf1c6e5be`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:22 GMT
ADD file:c855b3c65f5ba94d548d7d2659094eeb63fbf7f8419ac8e07712c3320c38b62c in / 
# Sat, 10 Apr 2021 01:20:22 GMT
CMD ["bash"]
# Sat, 10 Apr 2021 18:33:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 10 Apr 2021 18:33:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 10 Apr 2021 18:33:13 GMT
ENV LANG=C.UTF-8
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_MAJOR=2.7
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_VERSION=2.7.3
# Sat, 10 Apr 2021 18:39:51 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Sat, 10 Apr 2021 18:42:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 10 Apr 2021 18:42:57 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:57 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 10 Apr 2021 18:42:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 10 Apr 2021 18:42:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 10 Apr 2021 18:42:59 GMT
CMD ["irb"]
# Sun, 11 Apr 2021 06:55:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 11 Apr 2021 06:56:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 				shared-mime-info 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 11 Apr 2021 06:56:28 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:56:28 GMT
ENV RAILS_ENV=production
# Sun, 11 Apr 2021 06:56:28 GMT
WORKDIR /usr/src/redmine
# Sun, 11 Apr 2021 06:56:28 GMT
ENV HOME=/home/redmine
# Sun, 11 Apr 2021 06:56:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_VERSION=4.2.0
# Sun, 11 Apr 2021 06:56:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=295864c580afa2a926e7a17f2ad10693f9b7a6d9f1ef523edb96b2368e7f07e5
# Sun, 11 Apr 2021 06:56:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 11 Apr 2021 06:57:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:17 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 11 Apr 2021 06:57:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 11 Apr 2021 06:57:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 11 Apr 2021 06:57:17 GMT
EXPOSE 3000
# Sun, 11 Apr 2021 06:57:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sun, 11 Apr 2021 06:57:33 GMT
ENV PASSENGER_VERSION=6.0.8
# Sun, 11 Apr 2021 06:57:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 11 Apr 2021 06:57:50 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sun, 11 Apr 2021 06:57:50 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sun, 11 Apr 2021 06:57:50 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:f7ec5a41d630a33a2d1db59b95d89d93de7ae5a619a3a8571b78457e48266eba`  
		Last Modified: Sat, 10 Apr 2021 01:25:20 GMT  
		Size: 27.1 MB (27139373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b15c6c91d18393629dfb99925359030db79ef60af0caed870f0c5dd606855c`  
		Last Modified: Sat, 10 Apr 2021 19:08:48 GMT  
		Size: 12.6 MB (12562303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ca8a753679e422eee3d9a0298d15f02fe19b68560283afe5ba9510a1a37b87f`  
		Last Modified: Sat, 10 Apr 2021 19:08:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1596cf153142005038983af255e0d09ef62c65e139aa5c973c2d2baaa2044b0`  
		Last Modified: Sat, 10 Apr 2021 19:09:47 GMT  
		Size: 22.9 MB (22887036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ed63bc8e0386fa836f8cf065b98fa401987445d1ab32e260f00e34398b353c`  
		Last Modified: Sat, 10 Apr 2021 19:09:45 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cc6acca6e42a84df58aeac107bc65a7bd29a5a702ca33992837a43d23689e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:20 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1370bc72633d9b6883d4baa5cfe7320f3310950f72f5753966432b3c5fb39af7`  
		Last Modified: Sun, 11 Apr 2021 07:03:35 GMT  
		Size: 93.9 MB (93906284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db1ff6e623ce6c864b167bcc6a6513b6864b9dc79a4d77823597370866a1c4e`  
		Last Modified: Sun, 11 Apr 2021 07:03:21 GMT  
		Size: 1.4 MB (1370219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1aafa942955516a5b82908cc908e9fe16aa0e9d25e7c41513563f4d7dcd98e7`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0de8b29a2583f478869875849b6bdc9aa17b8f1cf07835e579284513b946dba`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305e2181bd63ce8a24b2330aa48fb52e8188a931903f495caaaaeb4ef6153e86`  
		Last Modified: Sun, 11 Apr 2021 07:03:18 GMT  
		Size: 3.1 MB (3057055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cdee7416a1645930503313e41e3183303a737aea90454566b7d83fac74e3707`  
		Last Modified: Sun, 11 Apr 2021 07:03:24 GMT  
		Size: 50.6 MB (50574847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f886f325a0ba2239c4905f09d7d6186c89f3202c59614d1181eeecf550cc69`  
		Last Modified: Sun, 11 Apr 2021 07:03:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4e67ce39214f6c91a2e674f89f56c6396296fe4ae2975f2dc24082bfa2db9f`  
		Last Modified: Sun, 11 Apr 2021 07:03:56 GMT  
		Size: 20.4 MB (20363201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd0141a3a34bc643ef0b1a5907467d3643479f4c5bb357ffb15dbff0a695a22`  
		Last Modified: Sun, 11 Apr 2021 07:03:54 GMT  
		Size: 4.9 MB (4936711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
