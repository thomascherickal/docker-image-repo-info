<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `redmine`

-	[`redmine:4`](#redmine4)
-	[`redmine:4.0`](#redmine40)
-	[`redmine:4.0.7`](#redmine407)
-	[`redmine:4.0.7-alpine`](#redmine407-alpine)
-	[`redmine:4.0.7-passenger`](#redmine407-passenger)
-	[`redmine:4.0-alpine`](#redmine40-alpine)
-	[`redmine:4.0-passenger`](#redmine40-passenger)
-	[`redmine:4.1`](#redmine41)
-	[`redmine:4.1.1`](#redmine411)
-	[`redmine:4.1.1-alpine`](#redmine411-alpine)
-	[`redmine:4.1.1-passenger`](#redmine411-passenger)
-	[`redmine:4.1-alpine`](#redmine41-alpine)
-	[`redmine:4.1-passenger`](#redmine41-passenger)
-	[`redmine:4-alpine`](#redmine4-alpine)
-	[`redmine:4-passenger`](#redmine4-passenger)
-	[`redmine:alpine`](#redminealpine)
-	[`redmine:latest`](#redminelatest)
-	[`redmine:passenger`](#redminepassenger)

## `redmine:4`

```console
$ docker pull redmine@sha256:4fc25b4212caaa21ba5392c725335c94f9c69c2ac0334a0b16be6f117735c409
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
$ docker pull redmine@sha256:97f04d83cec0d51fb6ea2920706508a33317643816bdb670bc948cf69622f8d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215593452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:229055151ea08ad0130dc9db0123325d794744a53ff2b686ae36ac80998650cb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:47:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:47:41 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:47:41 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:47:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 05:47:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:49:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:20 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:49:20 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:49:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:49:20 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:49:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceaf427bdaab140ab3c03e03e397142d0f07a88cdd442cba1826fb438958620`  
		Last Modified: Thu, 19 Nov 2020 05:54:07 GMT  
		Size: 93.1 MB (93104105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332f2c839082a3548a096495ec34f3bc551c78437af681d10ce1edfb94ee264`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 1.4 MB (1369330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061509154252c143a6b5680bb73dfa52909d4a8b300d809dd0e1ac53da1f12d`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409c9bd29355b0269a77c26db749c2549cfbfca66ffd7dd6b1f04610b2623019`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53142f7c27fe4f4a12dfef13f9a10f4613b03ad98babf32482a6c25ff52f13`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 2.7 MB (2739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee5b56b6eec16ce4e488515ba41448ea784f5bf5a8fc75c36ce898c6b5a46bb`  
		Last Modified: Thu, 19 Nov 2020 05:53:55 GMT  
		Size: 57.3 MB (57280977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c5b8b7f7c3b21ee1b9ea7cbae6a70f0a9cfe48646a3c04077b0fe8c8c8d64`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:23b395e2de1a0731bdddab91d31a709eb752aea2165aae7fdc33a02784b153ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204941869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80962afba0c5bd6eaddbb0316791452c348f5d3c7af3631ff6e156853c949658`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 12:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 12:22:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 12:22:26 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 12:40:14 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 12:45:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 12:45:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:45:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 12:45:18 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 19:54:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 19:55:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:56:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 19:56:27 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 19:56:28 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 19:56:29 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 19:56:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 19:56:31 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 19:56:32 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 19:56:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:00:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:00:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:00:11 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:00:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:00:12 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:00:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7091bf042b25a050f741dc921d43bf4c0c72eb54389f565f5762676e67300f`  
		Last Modified: Fri, 11 Dec 2020 13:11:58 GMT  
		Size: 10.3 MB (10327588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6ad9c9fde8ad2da9cc18e3d6ca0e0cdfcf95751c2ef3ca3b907a1899a08deb`  
		Last Modified: Fri, 11 Dec 2020 13:11:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81aef85a39dd03e9d3f8fab64423b80dea3eee4bf68f6df2bfbed5a7cbd041`  
		Last Modified: Fri, 11 Dec 2020 13:13:17 GMT  
		Size: 20.7 MB (20713612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb8a80d30d5c462ac1282bebf1d5568b7f1c1f982281df0ce4e93c3e6e53ae`  
		Last Modified: Fri, 11 Dec 2020 13:13:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad080b6708861654d51cdb61102ae28988bf5041b5ff8a2c3dedab5101cabe7`  
		Last Modified: Fri, 11 Dec 2020 20:07:56 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25473046e79518d96f411be654f4cc1db33e5f8c92c1051c404972d3ace724`  
		Last Modified: Fri, 11 Dec 2020 20:08:25 GMT  
		Size: 88.7 MB (88684630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a5c2535ec1f07fac6e66a12db43365ad44d2ab38b337dcc96b23a0bff02ed2`  
		Last Modified: Fri, 11 Dec 2020 20:07:55 GMT  
		Size: 1.3 MB (1325720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec2ca9b1e35e4bf9657cd000209470cf63e8ec47965e330b06ff6743522bb`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9add9f870ea1a44a3bbc62c09b726563275b6141f2c7a0c0f36a47b936048df`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74d0c25df9427de71ea7e084c0c76790a9d192a71cd4e5a9af621eebbc260f7`  
		Last Modified: Fri, 11 Dec 2020 20:07:54 GMT  
		Size: 2.7 MB (2739775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a593ef648ed210adc22c1a4231a5b0e604de28da07018d976307255d9531d34`  
		Last Modified: Fri, 11 Dec 2020 20:08:06 GMT  
		Size: 56.3 MB (56302590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497392e307eb7ff39de47f101367f73b69db9589aff0918c1b5f48c20ac24e77`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:91fba4adfa601d02809183e7a3d3e590584d307ae47077700856fcd6a80968f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.1 MB (198095589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c548293de9660d77a7da7898df901c34ac08428786fb2419c1db3731567b7fd2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:25:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:25:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 07:25:07 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 07:52:47 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 07:56:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 07:56:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 07:56:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 07:56:31 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 00:02:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 00:02:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 00:03:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:03:23 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 00:03:24 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 00:03:25 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 00:03:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 00:03:28 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 00:03:29 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 00:03:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 00:06:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:06:41 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 00:06:42 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 00:06:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 00:06:43 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 00:06:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f808f0b3cb34b0decd4c61cf2a3876da6033ec045a98cf6cd42a1991c44120`  
		Last Modified: Wed, 18 Nov 2020 08:20:04 GMT  
		Size: 9.8 MB (9847840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea69b961e8974ee2251411fd6cd5b31ccad490b460b73bf6854d29cf9eaf3`  
		Last Modified: Wed, 18 Nov 2020 08:19:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba22755c3b92f079a1218ec82370a9d002fd6b572f20dd4a296226f6b39d7cf`  
		Last Modified: Wed, 18 Nov 2020 08:21:17 GMT  
		Size: 20.6 MB (20622607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7edcf7ca8b960fd2574835e024db1d8cf6006d7a406395de35ec3361ac7209f`  
		Last Modified: Wed, 18 Nov 2020 08:21:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5460041916d57389e886f4c1925aecccf61a1d4c782e927e6fdbbddfa8045b1e`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27983c99d327dd4affc8333a5814244c1234adb6d7e1d55005e61251c08d53fb`  
		Last Modified: Thu, 19 Nov 2020 00:13:43 GMT  
		Size: 84.7 MB (84725207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1324b22d1b94bc1fad2a134946f0b495ace2068b127aa1006f4f510b7e5bc0`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.3 MB (1318532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6673217b014d5a6178c6420c4617f9232685ff98ebc629d06114ac77e41cb099`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f61d703ff2bb268b7079b253ed5622e6ca490a8a8f5bd70ba641f9064fb52`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2006b3162cef090805e876162a655e5c1705b4ff2780eb5c8d0e1d9586810519`  
		Last Modified: Thu, 19 Nov 2020 00:13:13 GMT  
		Size: 2.7 MB (2739770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5ce813b40ff509195e79c4a1cacf5ed50b1119c974a6a3691327c3d3935ee5`  
		Last Modified: Thu, 19 Nov 2020 00:13:25 GMT  
		Size: 56.1 MB (56122951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c064249f5e00ecd193930b27786723f458d9c7ada61caa91c6ba24c3a6442754`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:70de4f1e65da97eaf03494bc73f5e26f0680cefd7ebb1701b49e8fb8a4581f47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211343295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474ecb6ae80c0e9082c661aeaa14620d930adf2096eb04e7fffc2dad0e9bf1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 10:02:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 10:02:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 10:02:22 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 10:16:52 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 10:20:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 10:20:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 10:20:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 10:20:09 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 03:54:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 03:55:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 03:55:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 03:56:00 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 03:56:01 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 03:56:02 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 03:56:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 03:56:05 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 03:56:06 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 03:56:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 03:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 03:59:13 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 03:59:14 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 03:59:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 03:59:15 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 03:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cfcfe44e857123ffa02834cfe1a4126099c7486ecc0223251b64c1a9482954`  
		Last Modified: Wed, 18 Nov 2020 10:43:14 GMT  
		Size: 11.2 MB (11244662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ea17e8a560a0e781a182aae71bb98b7d6c0f8b59de48c41ca0ba4f9006097c`  
		Last Modified: Wed, 18 Nov 2020 10:43:10 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40bed2a0ea8bd34e9eb6ad5b1402f0e6b5dabcd0e3072f495a0e122b1c66c9d`  
		Last Modified: Wed, 18 Nov 2020 10:44:28 GMT  
		Size: 21.3 MB (21288399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6f60a2ebf322104e26fa3e867de1c11d5a667874b9e15f5bcf80f453d19f7c`  
		Last Modified: Wed, 18 Nov 2020 10:44:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b179d423b480ed400f3a5bf0acd9ebc766db80e8667e50a39528db66304f4`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ce67aa919a56bf635b903ce59af070282c6c74aa7c0543ee0ca64ce559ee15`  
		Last Modified: Thu, 19 Nov 2020 04:07:04 GMT  
		Size: 91.7 MB (91682420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5772509129feac5e394a21dbbd14667f6ec08af6bb678342213070c0e9a1fc0a`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.3 MB (1302832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee2429d8b0d53adc0e45a1d0453f17cceb2c50c101fdc827aaf85ac96035832`  
		Last Modified: Thu, 19 Nov 2020 04:06:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa29860dedc18f73d32ae3fc035269752dc1fd19490ca3eb3f4d619988d659a`  
		Last Modified: Thu, 19 Nov 2020 04:06:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a3b3d232fc7ba6b3c5e37d64edfb61d17a7b418d0f247221f1f10335506595`  
		Last Modified: Thu, 19 Nov 2020 04:06:38 GMT  
		Size: 2.7 MB (2739773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39a9061731cfc320d029edf109fdb55b8ae6162bf0b05e13518337ae6ac1fcf`  
		Last Modified: Thu, 19 Nov 2020 04:06:49 GMT  
		Size: 57.2 MB (57218170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe8386baa19d0b373438491ac57dec304b3c833a541f9e1f61e9fe401f11f3d`  
		Last Modified: Thu, 19 Nov 2020 04:06:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; 386

```console
$ docker pull redmine@sha256:f05ab67f515695946ed6633edf17a3f289dd74a6dd6a9b813b6464087f51f30e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.1 MB (221054301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f7d45a1cc118f7f17322d9714cfaae3593d51621b667169f65018e62675e16`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:50:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:50:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 01:50:18 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 02:18:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 02:18:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 02:18:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 02:18:11 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 16:28:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 16:28:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:29:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:29:06 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 16:29:06 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 16:29:06 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 16:29:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 16:29:07 GMT
ENV REDMINE_VERSION=4.1.1
# Wed, 18 Nov 2020 16:29:07 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Wed, 18 Nov 2020 16:29:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 16:31:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:31:04 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 16:31:04 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 16:31:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:31:04 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 16:31:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fbd9e82fd11f8ad081f5e89024c72f30321709805d508e2e07cfa4ec8dc8da`  
		Last Modified: Wed, 18 Nov 2020 02:49:55 GMT  
		Size: 17.2 MB (17207426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f29890b7d3b20bd4d0d4da045c378afaa0ce98710734a94606b4f565594bcb5`  
		Last Modified: Wed, 18 Nov 2020 02:49:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd96c246e2c6a5f9fd496b0717504aff786edc6b58fb255622543c1af5e99e`  
		Last Modified: Wed, 18 Nov 2020 02:51:17 GMT  
		Size: 20.9 MB (20884752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcbfc10a807c014f44297d6e929aa7c8c5756dab2f54181c1cddc95403951b2`  
		Last Modified: Wed, 18 Nov 2020 02:51:13 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8897bbac36c81c5ca34cd30285949651ac03b8a6d8d3f4163fb7e80c60692494`  
		Last Modified: Wed, 18 Nov 2020 16:35:20 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f55c47f87eb292476768cb1d6c5c4a9133ba389656f8a8e5d3e451fac2e60f`  
		Last Modified: Wed, 18 Nov 2020 16:35:49 GMT  
		Size: 94.7 MB (94727984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357ab763d41a2ce00c108910a7eb09d9a52d6d4b49caefa8fde8f4c1b11d48a`  
		Last Modified: Wed, 18 Nov 2020 16:35:19 GMT  
		Size: 1.3 MB (1337919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae1b38b60e40631615232d45aebb7a34a57cb98eeddc2ac7f85de5c5553c8a`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2748ed72d3978b1a3e4898bd4b8c170ac4a31592455f1aaf90e5f70cef1e6b1d`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1001b3f18050630ba786830c891b880c9faced19fe4a39fcdda8937f88e8e`  
		Last Modified: Wed, 18 Nov 2020 16:35:19 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd148206259b30fbfb7ba54e464954391bce2786b87b584b35352d93a3067f8`  
		Last Modified: Wed, 18 Nov 2020 16:35:32 GMT  
		Size: 56.4 MB (56386149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009c7c03d7e082effcfc58964806b009ab6672b31380597557744e635dcc9f96`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; mips64le

```console
$ docker pull redmine@sha256:35eea7d0cb73b9a686ee12c47df5fef0d96183a64061dd0094dcf56f567d6492
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.4 MB (210421080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5279ec7ab65588c4dfb09e9311640a47e602dd589177dcd0a0bd5e9572cdc31c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:51:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:51:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 15:51:06 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 16:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 16:35:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:35:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 16:35:52 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:18:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:19:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:20:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:20:14 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:20:14 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:20:15 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:20:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:20:17 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 20:20:17 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 20:20:24 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:26:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:26:04 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:26:04 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:26:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:26:05 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:26:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864c3d7d0761fea04a3b1c6ac70ddd82c27b002138b03d3b89fa7be97abceb7`  
		Last Modified: Fri, 11 Dec 2020 16:54:07 GMT  
		Size: 11.6 MB (11608300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c58bddd16db870da684d956706ac7beb34a9a61a1637993de013305758cf280`  
		Last Modified: Fri, 11 Dec 2020 16:53:56 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724bc21f9dc167d33b39911e02e8ca816132ecbc3747d7f141b95a99de70f36`  
		Last Modified: Fri, 11 Dec 2020 16:56:27 GMT  
		Size: 21.6 MB (21637748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64df4fb893d9e4613191d83d82f0cd2b63f149bbfbfd363deec584d9644f4fa6`  
		Last Modified: Fri, 11 Dec 2020 16:56:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c186313904d91e281f8e1831122fcccb8ab04d6412b825dc8f7459bcc551fb`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48af7885230e30ca6d0084380ed8e14750622deb4c94bf05befe441f7523835`  
		Last Modified: Fri, 11 Dec 2020 20:37:10 GMT  
		Size: 90.1 MB (90072579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129e6fa772a517fe09bce5f15f1cbb879f1d2d805028d61c1ed129f9dee551b5`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.3 MB (1256645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c0a4dd492334ab9acc4b786f85e20ff8e91d8f994a47fd7c534f7fed84ec7`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a93c92ba03861a44a149916f51047a1ad284e34b83aeb90bdd4504238c1c1e2`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413a895834fed7a4125630a5fb75fecc0516bc14c6f5664d4d8882925b7760bf`  
		Last Modified: Fri, 11 Dec 2020 20:36:00 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfc83332192097ee67902d601513d8e50030905b3e5a007ac39165eb400dcad`  
		Last Modified: Fri, 11 Dec 2020 20:36:28 GMT  
		Size: 57.3 MB (57332039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a674d2c8b1e024562180c82c0597eba27e91c07e6c1c06c8903a540e1e0bdd3`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; ppc64le

```console
$ docker pull redmine@sha256:c3ea73afabbf5abdfb628b2873fb45815d1ef4c9b95b572a9a0015e6945eefe6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227408094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e775c0e85890cfa750dae96663aaa8263ea772923a290760ce0de9b4248dbf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:26:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 12:27:02 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 12:57:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 12:57:42 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 12:57:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 13:05:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 13:06:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 13:06:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 13:06:40 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 22:56:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 23:16:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 23:23:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:24:12 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 23:24:36 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 23:24:57 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 23:25:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 23:26:01 GMT
ENV REDMINE_VERSION=4.1.1
# Wed, 18 Nov 2020 23:26:23 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Wed, 18 Nov 2020 23:27:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 23:36:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:37:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 23:37:14 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 23:37:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 23:37:26 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 23:37:31 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dba4d658f9cef4692709806bbbe7aa3f108b09489d3abadcdd00af26e816`  
		Last Modified: Wed, 18 Nov 2020 13:22:24 GMT  
		Size: 12.7 MB (12687856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f433a44b3fa921ad6d8b09e5619993f6812dfc023bf9c1ef38db8077916dfd3`  
		Last Modified: Wed, 18 Nov 2020 13:22:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6122ffb25e816545dedec8b707cbdea5f9f2b3c7c2a183f9ae488e46c605bb`  
		Last Modified: Wed, 18 Nov 2020 13:24:12 GMT  
		Size: 22.0 MB (21970057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab94d3b1f8973fd676af9a7da7255d83d3fdd27976823cbe4531093d01bb5f37`  
		Last Modified: Wed, 18 Nov 2020 13:24:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88001e8a986c6b8ebd7392d6ff4d5086ad80462ed5989827c839d3bfb4a01256`  
		Last Modified: Thu, 19 Nov 2020 00:19:46 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89539658f86c698aa7459ac0cdc89685e83e9eabb35fda5f82bbafe99f899680`  
		Last Modified: Thu, 19 Nov 2020 00:20:07 GMT  
		Size: 100.3 MB (100343979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3aa80defc7bbd76afb4c318dc49286936ba18a4e02c316b3fea450caf5727`  
		Last Modified: Thu, 19 Nov 2020 00:19:45 GMT  
		Size: 1.3 MB (1290133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46476067be42396f83b1e0b86411f0ebb193a82c64a8b44cfe7fce12fb68a1fc`  
		Last Modified: Thu, 19 Nov 2020 00:19:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec78f45da7bc16720440b5cfb4662425a82274373104d14c4834ed6185111460`  
		Last Modified: Thu, 19 Nov 2020 00:19:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9d4b0e36b50c79e6977f2e38415655d5822d25f34ecf61019611bf963cbddc`  
		Last Modified: Thu, 19 Nov 2020 00:19:40 GMT  
		Size: 2.7 MB (2739776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b6640a34082c8700a151ec61ee56a940ed83e971f04c234b49da0526ed48ee`  
		Last Modified: Thu, 19 Nov 2020 00:19:48 GMT  
		Size: 57.8 MB (57840073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b1969b444ef8f9019b929408c483060e510efd0b8db7764de2391927bb84`  
		Last Modified: Thu, 19 Nov 2020 00:19:38 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; s390x

```console
$ docker pull redmine@sha256:5afbbd3ee43a0df0b0e47bdce40339edfe52fdbb7e15f32b7c99dfe13e037d46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210687321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72abefdbc79df1244ddf76dba03ecf53d87f03826bfee12474c75bdbb7158f8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 14:05:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 14:06:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 14:06:00 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:39:41 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 14:39:42 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 14:39:43 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 14:44:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 14:44:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 14:44:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 14:44:07 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:53:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:53:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:54:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:54:20 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:54:20 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:54:21 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:54:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:54:22 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 20:54:23 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 20:54:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:56:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:56:29 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:56:30 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:56:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:56:30 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:56:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7319ab475e590b72d37f20d16fbbd64f355ac72137f788fba1242aae760a6732`  
		Last Modified: Fri, 11 Dec 2020 14:58:05 GMT  
		Size: 10.8 MB (10796868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81262b7893747b34acbfca1a00cfc0c68a997043db4e4b0ca7c54b95ef42d3`  
		Last Modified: Fri, 11 Dec 2020 14:58:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2d6654f121a57b04ec9b4cd0328c79f7172e853a3c161296394c0a4eff283`  
		Last Modified: Fri, 11 Dec 2020 14:58:43 GMT  
		Size: 21.6 MB (21598273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554cb46f10b3fc8fe21d4894b92fd3a71978d0522f8f8483a20076965f766433`  
		Last Modified: Fri, 11 Dec 2020 14:58:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae3b3620abc202ccd0f4255185baf54839bf2b973b6e861c0d152a91932fdd1`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae562a30e04f377136d022a05202c0e304d868faf41178e4d93747f3dcf4e02`  
		Last Modified: Fri, 11 Dec 2020 21:00:52 GMT  
		Size: 90.8 MB (90834404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cf9abfa62fe46d287e76c82e923fb635c8d76e9daa28663547ae13c6961fde`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.4 MB (1355550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f42b8d97ca9305ed8fee32c1e42ddbe6147d0a1301c149b9465cf97819d559`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9486d1ae34f16fbe53268c5fa17157568a1679208eb74f8046aaf79b5c2ffd4`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a697087fccb24b639a6b93f6da510d3f6ce42ace5d9f9e64cd893108536edf5`  
		Last Modified: Fri, 11 Dec 2020 21:00:37 GMT  
		Size: 2.7 MB (2739767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bda450facc4353a24f90ffab51457fb80d6fcd340d01cda5540157a21f1c0d`  
		Last Modified: Fri, 11 Dec 2020 21:00:43 GMT  
		Size: 57.6 MB (57643997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5351b41a29cb67f7763dbe84a9ee387f3667913e513212ba1d94d227034010`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0`

```console
$ docker pull redmine@sha256:3679c964ce8393009f2e3d0f6c7c7c86ef08a2eff2627cef2deb365affae76d7
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
$ docker pull redmine@sha256:f1d81e1c91fe87656b32e4edfc6ec26aa67773895ac283e4b56b5941eba8a438
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.1 MB (206082641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65eab793f1211f94786ee23e4a674545b22304005ac74308d08785e4dc5a6c9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:50:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:50:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:50:39 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:50:39 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:50:39 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:50:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:50:40 GMT
ENV REDMINE_VERSION=4.0.7
# Thu, 19 Nov 2020 05:50:41 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Thu, 19 Nov 2020 05:50:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:52:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:52:59 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:52:59 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:52:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:52:59 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:53:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ada238ba6ad8b2dd3ee44ebf880f407ef77b6e8ef18564613880076913f91ff`  
		Last Modified: Thu, 19 Nov 2020 05:54:42 GMT  
		Size: 80.2 MB (80211306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a962dc4ad4915e05c9361f8d64db6efba63905a16a29e3a47db5e38a65d50`  
		Last Modified: Thu, 19 Nov 2020 05:54:27 GMT  
		Size: 1.4 MB (1355881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef70e0cbc1210c5711bca0a07af598051ffe8aa854083ba02c2e885409e3c3`  
		Last Modified: Thu, 19 Nov 2020 05:54:25 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8606322853346140003f3bb117f00370f60cd3747ae532eac6438f8d766e8b`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15201977050c5f95385464b7e3b2cbdff5d113bc06bc3d11a5177dd9378ab76`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 2.5 MB (2535006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dcabfc99984272250e6813b788ff805bc12b10fd5dea5037876fb46edc03d5`  
		Last Modified: Thu, 19 Nov 2020 05:54:34 GMT  
		Size: 60.9 MB (60880885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867e85145489202033bc67d43fcb68494d7f08492ac3fe16391d1c4aaea9fc5`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:bbf316306c9e3b649a4e5d65d85e172a3985ef3eccd6e8336f50e7947873de54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195742079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cf917b7859760887bbbbcd4952bfcd197e26ebd30b8759793c4decb62459d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 12:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 12:22:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 12:22:26 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 12:40:14 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 12:45:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 12:45:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:45:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 12:45:18 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 19:54:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:01:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:01:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:01:54 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:01:55 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:01:56 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:01:58 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:01:59 GMT
ENV REDMINE_VERSION=4.0.7
# Fri, 11 Dec 2020 20:01:59 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Fri, 11 Dec 2020 20:02:05 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:07:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:07:24 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:07:25 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:07:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:07:26 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:07:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7091bf042b25a050f741dc921d43bf4c0c72eb54389f565f5762676e67300f`  
		Last Modified: Fri, 11 Dec 2020 13:11:58 GMT  
		Size: 10.3 MB (10327588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6ad9c9fde8ad2da9cc18e3d6ca0e0cdfcf95751c2ef3ca3b907a1899a08deb`  
		Last Modified: Fri, 11 Dec 2020 13:11:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81aef85a39dd03e9d3f8fab64423b80dea3eee4bf68f6df2bfbed5a7cbd041`  
		Last Modified: Fri, 11 Dec 2020 13:13:17 GMT  
		Size: 20.7 MB (20713612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb8a80d30d5c462ac1282bebf1d5568b7f1c1f982281df0ce4e93c3e6e53ae`  
		Last Modified: Fri, 11 Dec 2020 13:13:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad080b6708861654d51cdb61102ae28988bf5041b5ff8a2c3dedab5101cabe7`  
		Last Modified: Fri, 11 Dec 2020 20:07:56 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a17904d461d768b9d20312c2c50644bd769b9a92eaf8381b97d04eacf5a14`  
		Last Modified: Fri, 11 Dec 2020 20:09:02 GMT  
		Size: 76.1 MB (76068830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd5060d74e6c2568c5f631078fb1c5f74be0d217fe9b5fddf51e5acb707797d`  
		Last Modified: Fri, 11 Dec 2020 20:08:40 GMT  
		Size: 1.3 MB (1314620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f062aab8a36fe2392b0ab05d2df58ce2529fc38ad39a34cf04904219527b05`  
		Last Modified: Fri, 11 Dec 2020 20:08:37 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35fcc596d1bac59bdd9c785f7809597ec0ff41f72c6bb5693302ee364305726`  
		Last Modified: Fri, 11 Dec 2020 20:08:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf59140b8ffb85b0767867787aab95968a138657c5da8481862ce52e65a5f91`  
		Last Modified: Fri, 11 Dec 2020 20:08:38 GMT  
		Size: 2.5 MB (2535502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8bf9575a6ae243883f1d0523f7936f2d134383c1e1c5b63cf04d464fa4bd8`  
		Last Modified: Fri, 11 Dec 2020 20:08:49 GMT  
		Size: 59.9 MB (59933974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805aa58e77283c73a4792dfe0b42c414f6e0926b6540f28ef3143508064c088f`  
		Last Modified: Fri, 11 Dec 2020 20:08:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:abec8e3a46b019256aaffbb31d37434b7df91bfd71296648e2a7d7e5578d9179
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.1 MB (189149513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d44da2d18fcfc3fc93c63adaad5de529210b8b0dd97ab9178b0ed37de38bae`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:25:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:25:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 07:25:07 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 07:52:47 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 07:56:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 07:56:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 07:56:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 07:56:31 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 00:02:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 00:07:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 00:08:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:08:06 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 00:08:06 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 00:08:07 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 00:08:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 00:08:10 GMT
ENV REDMINE_VERSION=4.0.7
# Thu, 19 Nov 2020 00:08:10 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Thu, 19 Nov 2020 00:08:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 00:12:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:12:49 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 00:12:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 00:12:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 00:12:52 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 00:12:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f808f0b3cb34b0decd4c61cf2a3876da6033ec045a98cf6cd42a1991c44120`  
		Last Modified: Wed, 18 Nov 2020 08:20:04 GMT  
		Size: 9.8 MB (9847840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea69b961e8974ee2251411fd6cd5b31ccad490b460b73bf6854d29cf9eaf3`  
		Last Modified: Wed, 18 Nov 2020 08:19:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba22755c3b92f079a1218ec82370a9d002fd6b572f20dd4a296226f6b39d7cf`  
		Last Modified: Wed, 18 Nov 2020 08:21:17 GMT  
		Size: 20.6 MB (20622607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7edcf7ca8b960fd2574835e024db1d8cf6006d7a406395de35ec3361ac7209f`  
		Last Modified: Wed, 18 Nov 2020 08:21:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5460041916d57389e886f4c1925aecccf61a1d4c782e927e6fdbbddfa8045b1e`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40640cd7e41db7bef9af04683d4cbaf603dfb8bc2ae9c779c3f036684f3cc4a0`  
		Last Modified: Thu, 19 Nov 2020 00:14:33 GMT  
		Size: 72.4 MB (72395931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d34c70bcfabe6aa0d8b061d9adad389ad339cce7e21227310e2849216b506d`  
		Last Modified: Thu, 19 Nov 2020 00:14:00 GMT  
		Size: 1.3 MB (1304801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10857781c1047e1514a05c75fd92683468e9a8d76eff989655d7650f59834501`  
		Last Modified: Thu, 19 Nov 2020 00:13:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173dd7cd359e48372144e61b222e9b2b7f1e8024d1d543c42895485b9bfeaf6d`  
		Last Modified: Thu, 19 Nov 2020 00:13:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a5eacae24254fd3cd2aa5a4ecd04dc48ac172e5b9fb33fa7d2c4c598a1431`  
		Last Modified: Thu, 19 Nov 2020 00:13:59 GMT  
		Size: 2.5 MB (2535510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256a2beea0818ffd2b73ce4ecf4c9b86196f9dd861cf102996bd230058cd2ac2`  
		Last Modified: Thu, 19 Nov 2020 00:14:13 GMT  
		Size: 59.7 MB (59724142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a51470a39e94dd0d6603a2b3080895a9c3858009c7dd57e489ed6ce2227570`  
		Last Modified: Thu, 19 Nov 2020 00:13:58 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:f839bd94162595378d9b9c4d10407d6e6a3e3fab7d54de9ee06f50bedcd4d2cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201858968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9059d4bccb755db712b1203c5f9366f88e08fc0208fc36635cb7eb42e167432c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 10:02:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 10:02:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 10:02:22 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 10:16:52 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 10:20:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 10:20:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 10:20:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 10:20:09 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 03:54:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 04:00:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 04:00:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 04:00:38 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 04:00:40 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 04:00:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 04:00:44 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 04:00:46 GMT
ENV REDMINE_VERSION=4.0.7
# Thu, 19 Nov 2020 04:00:48 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Thu, 19 Nov 2020 04:00:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 04:06:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 04:06:17 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 04:06:18 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 04:06:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 04:06:19 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 04:06:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cfcfe44e857123ffa02834cfe1a4126099c7486ecc0223251b64c1a9482954`  
		Last Modified: Wed, 18 Nov 2020 10:43:14 GMT  
		Size: 11.2 MB (11244662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ea17e8a560a0e781a182aae71bb98b7d6c0f8b59de48c41ca0ba4f9006097c`  
		Last Modified: Wed, 18 Nov 2020 10:43:10 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40bed2a0ea8bd34e9eb6ad5b1402f0e6b5dabcd0e3072f495a0e122b1c66c9d`  
		Last Modified: Wed, 18 Nov 2020 10:44:28 GMT  
		Size: 21.3 MB (21288399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6f60a2ebf322104e26fa3e867de1c11d5a667874b9e15f5bcf80f453d19f7c`  
		Last Modified: Wed, 18 Nov 2020 10:44:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b179d423b480ed400f3a5bf0acd9ebc766db80e8667e50a39528db66304f4`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa18cefceb2f70d585bacc692b7b0727ad403ce4f9cffaaf8a6dd5017b65334`  
		Last Modified: Thu, 19 Nov 2020 04:07:39 GMT  
		Size: 78.8 MB (78830492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba3bf88717dcbfccd026dcb3d287b27ac3a09bdb8db3b0a19b20ff9ba705e05`  
		Last Modified: Thu, 19 Nov 2020 04:07:17 GMT  
		Size: 1.3 MB (1290814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88874d94b62c77e0e09ead898e42469781eb29385f98c3d703b873c4082fd04`  
		Last Modified: Thu, 19 Nov 2020 04:07:15 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe483aed1a9d5d00dcb8a58769ddbb4daca58c5b26cda6fec2f43cc73fb08d9f`  
		Last Modified: Thu, 19 Nov 2020 04:07:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3376fa4d9a33da06b98f86d68f37d865bf8c67f5e90314b0c6258ddc2613aa6`  
		Last Modified: Thu, 19 Nov 2020 04:07:17 GMT  
		Size: 2.5 MB (2535502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73afd7cdd619798a37cc426f47370b6a48f3b1c60cbd28d3f9d4fbbf07e657b0`  
		Last Modified: Thu, 19 Nov 2020 04:07:28 GMT  
		Size: 60.8 MB (60802060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07638955ed9d1b1639b30b889d76ffbc43552f973876a88763bf8757a343e93`  
		Last Modified: Thu, 19 Nov 2020 04:07:15 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; 386

```console
$ docker pull redmine@sha256:27698f3463d0664aa59ea42503b1e16317e732d21fac60fc5f1746f6596a2e0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.4 MB (211364618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02279f9ca82952bc4055fe7b447f011fc2fcab2fd9ff2e3e13657d5238cdfad5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:50:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:50:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 01:50:18 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 02:18:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 02:18:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 02:18:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 02:18:11 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 16:28:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 16:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:32:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:32:03 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 16:32:03 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 16:32:03 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 16:32:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 16:32:04 GMT
ENV REDMINE_VERSION=4.0.7
# Wed, 18 Nov 2020 16:32:04 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Wed, 18 Nov 2020 16:32:07 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 16:34:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:34:52 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 16:34:52 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 16:34:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:34:52 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 16:34:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fbd9e82fd11f8ad081f5e89024c72f30321709805d508e2e07cfa4ec8dc8da`  
		Last Modified: Wed, 18 Nov 2020 02:49:55 GMT  
		Size: 17.2 MB (17207426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f29890b7d3b20bd4d0d4da045c378afaa0ce98710734a94606b4f565594bcb5`  
		Last Modified: Wed, 18 Nov 2020 02:49:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd96c246e2c6a5f9fd496b0717504aff786edc6b58fb255622543c1af5e99e`  
		Last Modified: Wed, 18 Nov 2020 02:51:17 GMT  
		Size: 20.9 MB (20884752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcbfc10a807c014f44297d6e929aa7c8c5756dab2f54181c1cddc95403951b2`  
		Last Modified: Wed, 18 Nov 2020 02:51:13 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8897bbac36c81c5ca34cd30285949651ac03b8a6d8d3f4163fb7e80c60692494`  
		Last Modified: Wed, 18 Nov 2020 16:35:20 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fccefb2e6ba49f0e61c910bcc557fa7487dd624b67829b35c64e7e8b3c4270`  
		Last Modified: Wed, 18 Nov 2020 16:36:28 GMT  
		Size: 81.6 MB (81647671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b227c5c28df4efdcb5163554b998c21fc1e2d3406d51664356651430c164613b`  
		Last Modified: Wed, 18 Nov 2020 16:36:01 GMT  
		Size: 1.3 MB (1326586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f999140f550fb926bb3aeac672a02f3fdec00eec479d8ce97b65183b583a38b`  
		Last Modified: Wed, 18 Nov 2020 16:35:59 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882f1067b8208aa035df8969420ccb4ddbfd2950a15f388de754760ba2090de1`  
		Last Modified: Wed, 18 Nov 2020 16:35:59 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15eed052fe93a4b85897dd3f5680df6a57a85e78011a8f3ee5dda30c803fa084`  
		Last Modified: Wed, 18 Nov 2020 16:36:00 GMT  
		Size: 2.5 MB (2535011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744045cc20eda60808ac03c07b849f1708a624d1716acf4b2d55729333ebc271`  
		Last Modified: Wed, 18 Nov 2020 16:36:14 GMT  
		Size: 60.0 MB (59992584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9f5e1e3adeab282b5e49403bffb30b765a26c5e24e80296f4b4445c47aa0d9`  
		Last Modified: Wed, 18 Nov 2020 16:35:59 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; mips64le

```console
$ docker pull redmine@sha256:f143bfc74621db59f9931c7d41081e63e9da2ca8c867c7d919b5003ce38a2857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.0 MB (201035419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e5817822bb0cab65118d4681a1c2fa00da60aa2b88aaea6acceecc80cc3427`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:51:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:51:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 15:51:06 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 16:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 16:35:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:35:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 16:35:52 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:18:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:27:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:27:48 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:27:48 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:27:49 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:27:49 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:27:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:27:51 GMT
ENV REDMINE_VERSION=4.0.7
# Fri, 11 Dec 2020 20:27:52 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Fri, 11 Dec 2020 20:27:59 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:35:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:35:37 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:35:38 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:35:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:35:38 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:35:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864c3d7d0761fea04a3b1c6ac70ddd82c27b002138b03d3b89fa7be97abceb7`  
		Last Modified: Fri, 11 Dec 2020 16:54:07 GMT  
		Size: 11.6 MB (11608300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c58bddd16db870da684d956706ac7beb34a9a61a1637993de013305758cf280`  
		Last Modified: Fri, 11 Dec 2020 16:53:56 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724bc21f9dc167d33b39911e02e8ca816132ecbc3747d7f141b95a99de70f36`  
		Last Modified: Fri, 11 Dec 2020 16:56:27 GMT  
		Size: 21.6 MB (21637748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64df4fb893d9e4613191d83d82f0cd2b63f149bbfbfd363deec584d9644f4fa6`  
		Last Modified: Fri, 11 Dec 2020 16:56:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c186313904d91e281f8e1831122fcccb8ab04d6412b825dc8f7459bcc551fb`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1b66f74adf4f1cfe878302e9a3dd8c355603adf791af125000b8bce7b3c9fe`  
		Last Modified: Fri, 11 Dec 2020 20:38:34 GMT  
		Size: 77.3 MB (77343980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757e16d86af07618ca22532df7e0f224bb824f8abd26a3a376b0f53805d6a4a8`  
		Last Modified: Fri, 11 Dec 2020 20:37:38 GMT  
		Size: 1.2 MB (1243308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98998b15d1c2145a23ed5eaa2e1e73ba804a5b814d83ed81282e5ea635045d2f`  
		Last Modified: Fri, 11 Dec 2020 20:37:35 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b989d4857802c6ba8c307901482c5f0d94afa791880cbfbc70d90a65b7e183`  
		Last Modified: Fri, 11 Dec 2020 20:37:34 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b35bc154dab4defdca7f30b7f9ce0957f73fa987d41728f083cf04ececab97b`  
		Last Modified: Fri, 11 Dec 2020 20:37:37 GMT  
		Size: 2.5 MB (2535008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1744c30cfa30a89c4a05146401120ae6084c028e3d8726a2d0fdd8c64f38ddb`  
		Last Modified: Fri, 11 Dec 2020 20:38:08 GMT  
		Size: 60.9 MB (60892789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ace4f0786f0d2c12ad51da4d4f9b617c7fcabccd2be475a73989775b3913a1b`  
		Last Modified: Fri, 11 Dec 2020 20:37:33 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:2671c83aaf2aeb6ab6dce824610600dd97747a08e550ab79f59d5f34d5c6952f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.4 MB (217419609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa4155c369154e5d7482637d82d58e1873a1d65d4909b66f1bb27fa4f43ddc82`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:26:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 12:27:02 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 12:57:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 12:57:42 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 12:57:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 13:05:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 13:06:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 13:06:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 13:06:40 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 22:56:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 23:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 23:48:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:48:25 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 23:48:32 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 23:48:39 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 23:48:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 23:48:57 GMT
ENV REDMINE_VERSION=4.0.7
# Wed, 18 Nov 2020 23:49:01 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Wed, 18 Nov 2020 23:49:22 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 00:18:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:18:25 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 00:18:32 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 00:18:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 00:18:58 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 00:19:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dba4d658f9cef4692709806bbbe7aa3f108b09489d3abadcdd00af26e816`  
		Last Modified: Wed, 18 Nov 2020 13:22:24 GMT  
		Size: 12.7 MB (12687856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f433a44b3fa921ad6d8b09e5619993f6812dfc023bf9c1ef38db8077916dfd3`  
		Last Modified: Wed, 18 Nov 2020 13:22:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6122ffb25e816545dedec8b707cbdea5f9f2b3c7c2a183f9ae488e46c605bb`  
		Last Modified: Wed, 18 Nov 2020 13:24:12 GMT  
		Size: 22.0 MB (21970057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab94d3b1f8973fd676af9a7da7255d83d3fdd27976823cbe4531093d01bb5f37`  
		Last Modified: Wed, 18 Nov 2020 13:24:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88001e8a986c6b8ebd7392d6ff4d5086ad80462ed5989827c839d3bfb4a01256`  
		Last Modified: Thu, 19 Nov 2020 00:19:46 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4641a85a4ca14fc65784c335d746de7b7c4e5a00b1ef34b96dd8a86e07c920c`  
		Last Modified: Thu, 19 Nov 2020 00:20:50 GMT  
		Size: 86.9 MB (86917606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c413756370ba8faf07d7938c3b3273afcc9742587788318c9d0bbb0fb93f5a4`  
		Last Modified: Thu, 19 Nov 2020 00:20:32 GMT  
		Size: 1.3 MB (1275521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495d23511540f4214d54d0557348051496dd4376024827eb01a5472bfcadc7a7`  
		Last Modified: Thu, 19 Nov 2020 00:20:28 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a729cd544d589e7ace12abffe43793b3847b9001fcf19999a232fae551fb987`  
		Last Modified: Thu, 19 Nov 2020 00:20:29 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eea726c1892ddde5f5b436b6a1d7da79e40123829f98f1c1ba1ddfe6d66293`  
		Last Modified: Thu, 19 Nov 2020 00:20:29 GMT  
		Size: 2.5 MB (2535500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e577d7a499c1a577c84ae867ea774e1fbbcc85270edf5eefd951bfbe94be0e18`  
		Last Modified: Thu, 19 Nov 2020 00:20:38 GMT  
		Size: 61.5 MB (61496848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0419e7f2d38d48046e6e64142f17a26917f2deb6348b1c5530dd976a1affd28`  
		Last Modified: Thu, 19 Nov 2020 00:20:28 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; s390x

```console
$ docker pull redmine@sha256:936af1cd2c5fa9ae76c3fc0a92a247ea3dc7c7935b684bc97c2248939e80220b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.2 MB (201232766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3f8d0c48edf18389f1fb7914abd1f4e66d007004757ce88cd3d253fe64a168e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 14:05:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 14:06:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 14:06:00 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:39:41 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 14:39:42 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 14:39:43 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 14:44:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 14:44:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 14:44:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 14:44:07 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:53:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:57:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:57:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:57:14 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:57:14 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:57:14 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:57:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:57:15 GMT
ENV REDMINE_VERSION=4.0.7
# Fri, 11 Dec 2020 20:57:16 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Fri, 11 Dec 2020 20:57:18 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 21:00:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 21:00:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 21:00:10 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 21:00:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:00:11 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 21:00:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7319ab475e590b72d37f20d16fbbd64f355ac72137f788fba1242aae760a6732`  
		Last Modified: Fri, 11 Dec 2020 14:58:05 GMT  
		Size: 10.8 MB (10796868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81262b7893747b34acbfca1a00cfc0c68a997043db4e4b0ca7c54b95ef42d3`  
		Last Modified: Fri, 11 Dec 2020 14:58:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2d6654f121a57b04ec9b4cd0328c79f7172e853a3c161296394c0a4eff283`  
		Last Modified: Fri, 11 Dec 2020 14:58:43 GMT  
		Size: 21.6 MB (21598273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554cb46f10b3fc8fe21d4894b92fd3a71978d0522f8f8483a20076965f766433`  
		Last Modified: Fri, 11 Dec 2020 14:58:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae3b3620abc202ccd0f4255185baf54839bf2b973b6e861c0d152a91932fdd1`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db0da0ebed3331b54770ee818853bb9fe17eac66d17ce9d883f272533e5df4f`  
		Last Modified: Fri, 11 Dec 2020 21:01:18 GMT  
		Size: 78.0 MB (77980911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09cf88df3ee5ba82c16ed10635acc637eef988004fecc93ba53bea82a06805`  
		Last Modified: Fri, 11 Dec 2020 21:01:07 GMT  
		Size: 1.3 MB (1342086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb80cf2bc5357487e49712ce9fd9516b650a38eeec55a7e76e8559cd13937c`  
		Last Modified: Fri, 11 Dec 2020 21:01:06 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d06aff335551f521f04064eee7a0bc1e3dd04d1bf8b5d3b139298abe263cd`  
		Last Modified: Fri, 11 Dec 2020 21:01:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37129132b920ef685e35c487b6e8b15062b8819dd2182485e3ac9c739db4d12b`  
		Last Modified: Fri, 11 Dec 2020 21:01:05 GMT  
		Size: 2.5 MB (2535511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6386fc3738311b2d5e03436398b6573942af4ad7f53f468c895981b5c953da5`  
		Last Modified: Fri, 11 Dec 2020 21:01:12 GMT  
		Size: 61.3 MB (61260654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba341ac95a2efce3592235d57df76c0d32dad0325466538eb06a7fc66ffff3db`  
		Last Modified: Fri, 11 Dec 2020 21:01:05 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.7`

```console
$ docker pull redmine@sha256:3679c964ce8393009f2e3d0f6c7c7c86ef08a2eff2627cef2deb365affae76d7
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

### `redmine:4.0.7` - linux; amd64

```console
$ docker pull redmine@sha256:f1d81e1c91fe87656b32e4edfc6ec26aa67773895ac283e4b56b5941eba8a438
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.1 MB (206082641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c65eab793f1211f94786ee23e4a674545b22304005ac74308d08785e4dc5a6c9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:50:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:50:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:50:39 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:50:39 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:50:39 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:50:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:50:40 GMT
ENV REDMINE_VERSION=4.0.7
# Thu, 19 Nov 2020 05:50:41 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Thu, 19 Nov 2020 05:50:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:52:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:52:59 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:52:59 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:52:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:52:59 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:53:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ada238ba6ad8b2dd3ee44ebf880f407ef77b6e8ef18564613880076913f91ff`  
		Last Modified: Thu, 19 Nov 2020 05:54:42 GMT  
		Size: 80.2 MB (80211306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a962dc4ad4915e05c9361f8d64db6efba63905a16a29e3a47db5e38a65d50`  
		Last Modified: Thu, 19 Nov 2020 05:54:27 GMT  
		Size: 1.4 MB (1355881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef70e0cbc1210c5711bca0a07af598051ffe8aa854083ba02c2e885409e3c3`  
		Last Modified: Thu, 19 Nov 2020 05:54:25 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8606322853346140003f3bb117f00370f60cd3747ae532eac6438f8d766e8b`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15201977050c5f95385464b7e3b2cbdff5d113bc06bc3d11a5177dd9378ab76`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 2.5 MB (2535006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dcabfc99984272250e6813b788ff805bc12b10fd5dea5037876fb46edc03d5`  
		Last Modified: Thu, 19 Nov 2020 05:54:34 GMT  
		Size: 60.9 MB (60880885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867e85145489202033bc67d43fcb68494d7f08492ac3fe16391d1c4aaea9fc5`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.7` - linux; arm variant v5

```console
$ docker pull redmine@sha256:bbf316306c9e3b649a4e5d65d85e172a3985ef3eccd6e8336f50e7947873de54
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195742079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:924cf917b7859760887bbbbcd4952bfcd197e26ebd30b8759793c4decb62459d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 12:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 12:22:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 12:22:26 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 12:40:14 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 12:45:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 12:45:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:45:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 12:45:18 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 19:54:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:01:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:01:53 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:01:54 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:01:55 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:01:56 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:01:58 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:01:59 GMT
ENV REDMINE_VERSION=4.0.7
# Fri, 11 Dec 2020 20:01:59 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Fri, 11 Dec 2020 20:02:05 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:07:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:07:24 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:07:25 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:07:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:07:26 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:07:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7091bf042b25a050f741dc921d43bf4c0c72eb54389f565f5762676e67300f`  
		Last Modified: Fri, 11 Dec 2020 13:11:58 GMT  
		Size: 10.3 MB (10327588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6ad9c9fde8ad2da9cc18e3d6ca0e0cdfcf95751c2ef3ca3b907a1899a08deb`  
		Last Modified: Fri, 11 Dec 2020 13:11:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81aef85a39dd03e9d3f8fab64423b80dea3eee4bf68f6df2bfbed5a7cbd041`  
		Last Modified: Fri, 11 Dec 2020 13:13:17 GMT  
		Size: 20.7 MB (20713612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb8a80d30d5c462ac1282bebf1d5568b7f1c1f982281df0ce4e93c3e6e53ae`  
		Last Modified: Fri, 11 Dec 2020 13:13:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad080b6708861654d51cdb61102ae28988bf5041b5ff8a2c3dedab5101cabe7`  
		Last Modified: Fri, 11 Dec 2020 20:07:56 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:906a17904d461d768b9d20312c2c50644bd769b9a92eaf8381b97d04eacf5a14`  
		Last Modified: Fri, 11 Dec 2020 20:09:02 GMT  
		Size: 76.1 MB (76068830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cd5060d74e6c2568c5f631078fb1c5f74be0d217fe9b5fddf51e5acb707797d`  
		Last Modified: Fri, 11 Dec 2020 20:08:40 GMT  
		Size: 1.3 MB (1314620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f062aab8a36fe2392b0ab05d2df58ce2529fc38ad39a34cf04904219527b05`  
		Last Modified: Fri, 11 Dec 2020 20:08:37 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35fcc596d1bac59bdd9c785f7809597ec0ff41f72c6bb5693302ee364305726`  
		Last Modified: Fri, 11 Dec 2020 20:08:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf59140b8ffb85b0767867787aab95968a138657c5da8481862ce52e65a5f91`  
		Last Modified: Fri, 11 Dec 2020 20:08:38 GMT  
		Size: 2.5 MB (2535502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b8bf9575a6ae243883f1d0523f7936f2d134383c1e1c5b63cf04d464fa4bd8`  
		Last Modified: Fri, 11 Dec 2020 20:08:49 GMT  
		Size: 59.9 MB (59933974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805aa58e77283c73a4792dfe0b42c414f6e0926b6540f28ef3143508064c088f`  
		Last Modified: Fri, 11 Dec 2020 20:08:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.7` - linux; arm variant v7

```console
$ docker pull redmine@sha256:abec8e3a46b019256aaffbb31d37434b7df91bfd71296648e2a7d7e5578d9179
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.1 MB (189149513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d44da2d18fcfc3fc93c63adaad5de529210b8b0dd97ab9178b0ed37de38bae`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:25:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:25:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 07:25:07 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 07:52:47 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 07:56:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 07:56:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 07:56:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 07:56:31 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 00:02:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 00:07:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 00:08:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:08:06 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 00:08:06 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 00:08:07 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 00:08:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 00:08:10 GMT
ENV REDMINE_VERSION=4.0.7
# Thu, 19 Nov 2020 00:08:10 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Thu, 19 Nov 2020 00:08:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 00:12:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:12:49 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 00:12:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 00:12:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 00:12:52 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 00:12:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f808f0b3cb34b0decd4c61cf2a3876da6033ec045a98cf6cd42a1991c44120`  
		Last Modified: Wed, 18 Nov 2020 08:20:04 GMT  
		Size: 9.8 MB (9847840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea69b961e8974ee2251411fd6cd5b31ccad490b460b73bf6854d29cf9eaf3`  
		Last Modified: Wed, 18 Nov 2020 08:19:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba22755c3b92f079a1218ec82370a9d002fd6b572f20dd4a296226f6b39d7cf`  
		Last Modified: Wed, 18 Nov 2020 08:21:17 GMT  
		Size: 20.6 MB (20622607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7edcf7ca8b960fd2574835e024db1d8cf6006d7a406395de35ec3361ac7209f`  
		Last Modified: Wed, 18 Nov 2020 08:21:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5460041916d57389e886f4c1925aecccf61a1d4c782e927e6fdbbddfa8045b1e`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40640cd7e41db7bef9af04683d4cbaf603dfb8bc2ae9c779c3f036684f3cc4a0`  
		Last Modified: Thu, 19 Nov 2020 00:14:33 GMT  
		Size: 72.4 MB (72395931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d34c70bcfabe6aa0d8b061d9adad389ad339cce7e21227310e2849216b506d`  
		Last Modified: Thu, 19 Nov 2020 00:14:00 GMT  
		Size: 1.3 MB (1304801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10857781c1047e1514a05c75fd92683468e9a8d76eff989655d7650f59834501`  
		Last Modified: Thu, 19 Nov 2020 00:13:57 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173dd7cd359e48372144e61b222e9b2b7f1e8024d1d543c42895485b9bfeaf6d`  
		Last Modified: Thu, 19 Nov 2020 00:13:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863a5eacae24254fd3cd2aa5a4ecd04dc48ac172e5b9fb33fa7d2c4c598a1431`  
		Last Modified: Thu, 19 Nov 2020 00:13:59 GMT  
		Size: 2.5 MB (2535510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256a2beea0818ffd2b73ce4ecf4c9b86196f9dd861cf102996bd230058cd2ac2`  
		Last Modified: Thu, 19 Nov 2020 00:14:13 GMT  
		Size: 59.7 MB (59724142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a51470a39e94dd0d6603a2b3080895a9c3858009c7dd57e489ed6ce2227570`  
		Last Modified: Thu, 19 Nov 2020 00:13:58 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.7` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:f839bd94162595378d9b9c4d10407d6e6a3e3fab7d54de9ee06f50bedcd4d2cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201858968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9059d4bccb755db712b1203c5f9366f88e08fc0208fc36635cb7eb42e167432c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 10:02:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 10:02:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 10:02:22 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 10:16:52 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 10:20:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 10:20:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 10:20:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 10:20:09 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 03:54:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 04:00:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 04:00:37 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 04:00:38 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 04:00:40 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 04:00:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 04:00:44 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 04:00:46 GMT
ENV REDMINE_VERSION=4.0.7
# Thu, 19 Nov 2020 04:00:48 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Thu, 19 Nov 2020 04:00:54 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 04:06:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 04:06:17 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 04:06:18 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 04:06:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 04:06:19 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 04:06:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cfcfe44e857123ffa02834cfe1a4126099c7486ecc0223251b64c1a9482954`  
		Last Modified: Wed, 18 Nov 2020 10:43:14 GMT  
		Size: 11.2 MB (11244662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ea17e8a560a0e781a182aae71bb98b7d6c0f8b59de48c41ca0ba4f9006097c`  
		Last Modified: Wed, 18 Nov 2020 10:43:10 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40bed2a0ea8bd34e9eb6ad5b1402f0e6b5dabcd0e3072f495a0e122b1c66c9d`  
		Last Modified: Wed, 18 Nov 2020 10:44:28 GMT  
		Size: 21.3 MB (21288399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6f60a2ebf322104e26fa3e867de1c11d5a667874b9e15f5bcf80f453d19f7c`  
		Last Modified: Wed, 18 Nov 2020 10:44:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b179d423b480ed400f3a5bf0acd9ebc766db80e8667e50a39528db66304f4`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa18cefceb2f70d585bacc692b7b0727ad403ce4f9cffaaf8a6dd5017b65334`  
		Last Modified: Thu, 19 Nov 2020 04:07:39 GMT  
		Size: 78.8 MB (78830492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba3bf88717dcbfccd026dcb3d287b27ac3a09bdb8db3b0a19b20ff9ba705e05`  
		Last Modified: Thu, 19 Nov 2020 04:07:17 GMT  
		Size: 1.3 MB (1290814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88874d94b62c77e0e09ead898e42469781eb29385f98c3d703b873c4082fd04`  
		Last Modified: Thu, 19 Nov 2020 04:07:15 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe483aed1a9d5d00dcb8a58769ddbb4daca58c5b26cda6fec2f43cc73fb08d9f`  
		Last Modified: Thu, 19 Nov 2020 04:07:15 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3376fa4d9a33da06b98f86d68f37d865bf8c67f5e90314b0c6258ddc2613aa6`  
		Last Modified: Thu, 19 Nov 2020 04:07:17 GMT  
		Size: 2.5 MB (2535502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73afd7cdd619798a37cc426f47370b6a48f3b1c60cbd28d3f9d4fbbf07e657b0`  
		Last Modified: Thu, 19 Nov 2020 04:07:28 GMT  
		Size: 60.8 MB (60802060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b07638955ed9d1b1639b30b889d76ffbc43552f973876a88763bf8757a343e93`  
		Last Modified: Thu, 19 Nov 2020 04:07:15 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.7` - linux; 386

```console
$ docker pull redmine@sha256:27698f3463d0664aa59ea42503b1e16317e732d21fac60fc5f1746f6596a2e0f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.4 MB (211364618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02279f9ca82952bc4055fe7b447f011fc2fcab2fd9ff2e3e13657d5238cdfad5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:50:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:50:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 01:50:18 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 02:18:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 02:18:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 02:18:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 02:18:11 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 16:28:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 16:31:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:32:03 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:32:03 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 16:32:03 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 16:32:03 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 16:32:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 16:32:04 GMT
ENV REDMINE_VERSION=4.0.7
# Wed, 18 Nov 2020 16:32:04 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Wed, 18 Nov 2020 16:32:07 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 16:34:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:34:52 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 16:34:52 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 16:34:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:34:52 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 16:34:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fbd9e82fd11f8ad081f5e89024c72f30321709805d508e2e07cfa4ec8dc8da`  
		Last Modified: Wed, 18 Nov 2020 02:49:55 GMT  
		Size: 17.2 MB (17207426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f29890b7d3b20bd4d0d4da045c378afaa0ce98710734a94606b4f565594bcb5`  
		Last Modified: Wed, 18 Nov 2020 02:49:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd96c246e2c6a5f9fd496b0717504aff786edc6b58fb255622543c1af5e99e`  
		Last Modified: Wed, 18 Nov 2020 02:51:17 GMT  
		Size: 20.9 MB (20884752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcbfc10a807c014f44297d6e929aa7c8c5756dab2f54181c1cddc95403951b2`  
		Last Modified: Wed, 18 Nov 2020 02:51:13 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8897bbac36c81c5ca34cd30285949651ac03b8a6d8d3f4163fb7e80c60692494`  
		Last Modified: Wed, 18 Nov 2020 16:35:20 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1fccefb2e6ba49f0e61c910bcc557fa7487dd624b67829b35c64e7e8b3c4270`  
		Last Modified: Wed, 18 Nov 2020 16:36:28 GMT  
		Size: 81.6 MB (81647671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b227c5c28df4efdcb5163554b998c21fc1e2d3406d51664356651430c164613b`  
		Last Modified: Wed, 18 Nov 2020 16:36:01 GMT  
		Size: 1.3 MB (1326586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f999140f550fb926bb3aeac672a02f3fdec00eec479d8ce97b65183b583a38b`  
		Last Modified: Wed, 18 Nov 2020 16:35:59 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882f1067b8208aa035df8969420ccb4ddbfd2950a15f388de754760ba2090de1`  
		Last Modified: Wed, 18 Nov 2020 16:35:59 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15eed052fe93a4b85897dd3f5680df6a57a85e78011a8f3ee5dda30c803fa084`  
		Last Modified: Wed, 18 Nov 2020 16:36:00 GMT  
		Size: 2.5 MB (2535011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744045cc20eda60808ac03c07b849f1708a624d1716acf4b2d55729333ebc271`  
		Last Modified: Wed, 18 Nov 2020 16:36:14 GMT  
		Size: 60.0 MB (59992584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9f5e1e3adeab282b5e49403bffb30b765a26c5e24e80296f4b4445c47aa0d9`  
		Last Modified: Wed, 18 Nov 2020 16:35:59 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.7` - linux; mips64le

```console
$ docker pull redmine@sha256:f143bfc74621db59f9931c7d41081e63e9da2ca8c867c7d919b5003ce38a2857
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.0 MB (201035419 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9e5817822bb0cab65118d4681a1c2fa00da60aa2b88aaea6acceecc80cc3427`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:51:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:51:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 15:51:06 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 16:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 16:35:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:35:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 16:35:52 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:18:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:27:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:27:48 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:27:48 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:27:49 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:27:49 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:27:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:27:51 GMT
ENV REDMINE_VERSION=4.0.7
# Fri, 11 Dec 2020 20:27:52 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Fri, 11 Dec 2020 20:27:59 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:35:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:35:37 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:35:38 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:35:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:35:38 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:35:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864c3d7d0761fea04a3b1c6ac70ddd82c27b002138b03d3b89fa7be97abceb7`  
		Last Modified: Fri, 11 Dec 2020 16:54:07 GMT  
		Size: 11.6 MB (11608300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c58bddd16db870da684d956706ac7beb34a9a61a1637993de013305758cf280`  
		Last Modified: Fri, 11 Dec 2020 16:53:56 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724bc21f9dc167d33b39911e02e8ca816132ecbc3747d7f141b95a99de70f36`  
		Last Modified: Fri, 11 Dec 2020 16:56:27 GMT  
		Size: 21.6 MB (21637748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64df4fb893d9e4613191d83d82f0cd2b63f149bbfbfd363deec584d9644f4fa6`  
		Last Modified: Fri, 11 Dec 2020 16:56:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c186313904d91e281f8e1831122fcccb8ab04d6412b825dc8f7459bcc551fb`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1b66f74adf4f1cfe878302e9a3dd8c355603adf791af125000b8bce7b3c9fe`  
		Last Modified: Fri, 11 Dec 2020 20:38:34 GMT  
		Size: 77.3 MB (77343980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757e16d86af07618ca22532df7e0f224bb824f8abd26a3a376b0f53805d6a4a8`  
		Last Modified: Fri, 11 Dec 2020 20:37:38 GMT  
		Size: 1.2 MB (1243308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98998b15d1c2145a23ed5eaa2e1e73ba804a5b814d83ed81282e5ea635045d2f`  
		Last Modified: Fri, 11 Dec 2020 20:37:35 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b989d4857802c6ba8c307901482c5f0d94afa791880cbfbc70d90a65b7e183`  
		Last Modified: Fri, 11 Dec 2020 20:37:34 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b35bc154dab4defdca7f30b7f9ce0957f73fa987d41728f083cf04ececab97b`  
		Last Modified: Fri, 11 Dec 2020 20:37:37 GMT  
		Size: 2.5 MB (2535008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1744c30cfa30a89c4a05146401120ae6084c028e3d8726a2d0fdd8c64f38ddb`  
		Last Modified: Fri, 11 Dec 2020 20:38:08 GMT  
		Size: 60.9 MB (60892789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ace4f0786f0d2c12ad51da4d4f9b617c7fcabccd2be475a73989775b3913a1b`  
		Last Modified: Fri, 11 Dec 2020 20:37:33 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.7` - linux; ppc64le

```console
$ docker pull redmine@sha256:2671c83aaf2aeb6ab6dce824610600dd97747a08e550ab79f59d5f34d5c6952f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.4 MB (217419609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa4155c369154e5d7482637d82d58e1873a1d65d4909b66f1bb27fa4f43ddc82`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:26:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 12:27:02 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 12:57:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 12:57:42 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 12:57:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 13:05:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 13:06:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 13:06:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 13:06:40 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 22:56:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 23:46:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 23:48:20 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:48:25 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 23:48:32 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 23:48:39 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 23:48:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 23:48:57 GMT
ENV REDMINE_VERSION=4.0.7
# Wed, 18 Nov 2020 23:49:01 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Wed, 18 Nov 2020 23:49:22 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 00:18:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:18:25 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 00:18:32 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 00:18:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 00:18:58 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 00:19:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dba4d658f9cef4692709806bbbe7aa3f108b09489d3abadcdd00af26e816`  
		Last Modified: Wed, 18 Nov 2020 13:22:24 GMT  
		Size: 12.7 MB (12687856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f433a44b3fa921ad6d8b09e5619993f6812dfc023bf9c1ef38db8077916dfd3`  
		Last Modified: Wed, 18 Nov 2020 13:22:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6122ffb25e816545dedec8b707cbdea5f9f2b3c7c2a183f9ae488e46c605bb`  
		Last Modified: Wed, 18 Nov 2020 13:24:12 GMT  
		Size: 22.0 MB (21970057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab94d3b1f8973fd676af9a7da7255d83d3fdd27976823cbe4531093d01bb5f37`  
		Last Modified: Wed, 18 Nov 2020 13:24:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88001e8a986c6b8ebd7392d6ff4d5086ad80462ed5989827c839d3bfb4a01256`  
		Last Modified: Thu, 19 Nov 2020 00:19:46 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4641a85a4ca14fc65784c335d746de7b7c4e5a00b1ef34b96dd8a86e07c920c`  
		Last Modified: Thu, 19 Nov 2020 00:20:50 GMT  
		Size: 86.9 MB (86917606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c413756370ba8faf07d7938c3b3273afcc9742587788318c9d0bbb0fb93f5a4`  
		Last Modified: Thu, 19 Nov 2020 00:20:32 GMT  
		Size: 1.3 MB (1275521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495d23511540f4214d54d0557348051496dd4376024827eb01a5472bfcadc7a7`  
		Last Modified: Thu, 19 Nov 2020 00:20:28 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a729cd544d589e7ace12abffe43793b3847b9001fcf19999a232fae551fb987`  
		Last Modified: Thu, 19 Nov 2020 00:20:29 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eea726c1892ddde5f5b436b6a1d7da79e40123829f98f1c1ba1ddfe6d66293`  
		Last Modified: Thu, 19 Nov 2020 00:20:29 GMT  
		Size: 2.5 MB (2535500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e577d7a499c1a577c84ae867ea774e1fbbcc85270edf5eefd951bfbe94be0e18`  
		Last Modified: Thu, 19 Nov 2020 00:20:38 GMT  
		Size: 61.5 MB (61496848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0419e7f2d38d48046e6e64142f17a26917f2deb6348b1c5530dd976a1affd28`  
		Last Modified: Thu, 19 Nov 2020 00:20:28 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.7` - linux; s390x

```console
$ docker pull redmine@sha256:936af1cd2c5fa9ae76c3fc0a92a247ea3dc7c7935b684bc97c2248939e80220b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.2 MB (201232766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3f8d0c48edf18389f1fb7914abd1f4e66d007004757ce88cd3d253fe64a168e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 14:05:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 14:06:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 14:06:00 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:39:41 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 14:39:42 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 14:39:43 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 14:44:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 14:44:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 14:44:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 14:44:07 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:53:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:57:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:57:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:57:14 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:57:14 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:57:14 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:57:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:57:15 GMT
ENV REDMINE_VERSION=4.0.7
# Fri, 11 Dec 2020 20:57:16 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Fri, 11 Dec 2020 20:57:18 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 21:00:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 21:00:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 21:00:10 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 21:00:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 21:00:11 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 21:00:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7319ab475e590b72d37f20d16fbbd64f355ac72137f788fba1242aae760a6732`  
		Last Modified: Fri, 11 Dec 2020 14:58:05 GMT  
		Size: 10.8 MB (10796868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81262b7893747b34acbfca1a00cfc0c68a997043db4e4b0ca7c54b95ef42d3`  
		Last Modified: Fri, 11 Dec 2020 14:58:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2d6654f121a57b04ec9b4cd0328c79f7172e853a3c161296394c0a4eff283`  
		Last Modified: Fri, 11 Dec 2020 14:58:43 GMT  
		Size: 21.6 MB (21598273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554cb46f10b3fc8fe21d4894b92fd3a71978d0522f8f8483a20076965f766433`  
		Last Modified: Fri, 11 Dec 2020 14:58:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae3b3620abc202ccd0f4255185baf54839bf2b973b6e861c0d152a91932fdd1`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db0da0ebed3331b54770ee818853bb9fe17eac66d17ce9d883f272533e5df4f`  
		Last Modified: Fri, 11 Dec 2020 21:01:18 GMT  
		Size: 78.0 MB (77980911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c09cf88df3ee5ba82c16ed10635acc637eef988004fecc93ba53bea82a06805`  
		Last Modified: Fri, 11 Dec 2020 21:01:07 GMT  
		Size: 1.3 MB (1342086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8cb80cf2bc5357487e49712ce9fd9516b650a38eeec55a7e76e8559cd13937c`  
		Last Modified: Fri, 11 Dec 2020 21:01:06 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d06aff335551f521f04064eee7a0bc1e3dd04d1bf8b5d3b139298abe263cd`  
		Last Modified: Fri, 11 Dec 2020 21:01:05 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37129132b920ef685e35c487b6e8b15062b8819dd2182485e3ac9c739db4d12b`  
		Last Modified: Fri, 11 Dec 2020 21:01:05 GMT  
		Size: 2.5 MB (2535511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6386fc3738311b2d5e03436398b6573942af4ad7f53f468c895981b5c953da5`  
		Last Modified: Fri, 11 Dec 2020 21:01:12 GMT  
		Size: 61.3 MB (61260654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba341ac95a2efce3592235d57df76c0d32dad0325466538eb06a7fc66ffff3db`  
		Last Modified: Fri, 11 Dec 2020 21:01:05 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.7-alpine`

```console
$ docker pull redmine@sha256:ad7382f05ccf37ce1612e65b6a480211ab7d82e421cf40b8882d4158fb2142ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0.7-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:5ab5b25a7f6cd570c5dfe652fab11c71b2005262a5e5e84c3606c79a4e3a4b5b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172913667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201e41566cd75f7407ac15b8c4141bd86192131e9aa378924e24a484be64a7ea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:01:32 GMT
RUN apk add --no-cache 		gmp-dev
# Fri, 24 Apr 2020 13:01:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 26 Jun 2020 21:31:26 GMT
ENV LANG=C.UTF-8
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 26 Jun 2020 21:58:02 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 26 Jun 2020 22:02:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 26 Jun 2020 22:02:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Jun 2020 22:02:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 26 Jun 2020 22:02:57 GMT
CMD ["irb"]
# Sat, 27 Jun 2020 00:25:13 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 27 Jun 2020 00:31:21 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Sat, 27 Jun 2020 00:31:22 GMT
ENV RAILS_ENV=production
# Sat, 27 Jun 2020 00:31:22 GMT
WORKDIR /usr/src/redmine
# Sat, 27 Jun 2020 00:31:22 GMT
ENV HOME=/home/redmine
# Sat, 27 Jun 2020 00:31:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 27 Jun 2020 00:31:23 GMT
ENV REDMINE_VERSION=4.0.7
# Sat, 27 Jun 2020 00:31:23 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Sat, 27 Jun 2020 00:31:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 27 Jun 2020 00:33:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Jun 2020 00:33:04 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 27 Jun 2020 00:33:04 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 27 Jun 2020 00:33:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 27 Jun 2020 00:33:05 GMT
EXPOSE 3000
# Sat, 27 Jun 2020 00:33:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8ae8202b42d1c70c3a7f65680eabc1c562a29227549b9a1b33dc03943b20d2`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 1.1 MB (1131841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21786fe7c0d7561a5b89ca15d8a1c3e4ea673820cd79f1308bdfd8eb3cb7142`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb235115f8edc3a10cc9c312b6e1abb565211c93fa76ab48d17268515854e8be`  
		Last Modified: Fri, 26 Jun 2020 22:32:52 GMT  
		Size: 22.0 MB (22034884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c29a4c064b384d769d0155220d34ae1d2fddf90c92c2da398542082e780530`  
		Last Modified: Fri, 26 Jun 2020 22:32:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c476068e888bb1f351101b749200705a002008950a4e439b52a7b4c7d918fcb`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14876154f43c2933de788e3f4d1c5d8f032f1e67d81fe9950b35b0c036bc95b`  
		Last Modified: Sat, 27 Jun 2020 00:35:12 GMT  
		Size: 84.3 MB (84335465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7eef6551123b1102419f8867186a7430e1f29913c500ef5efa543f27818974`  
		Last Modified: Sat, 27 Jun 2020 00:34:53 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ed76f4a7e483ddf6d602bfbd15c28c63ff1e062dbb401fc2e4523c79d8636`  
		Last Modified: Sat, 27 Jun 2020 00:34:53 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e11b4834cabb36d0909293bb99b488be2f141b52752722f2c21bd34b33fb0`  
		Last Modified: Sat, 27 Jun 2020 00:34:54 GMT  
		Size: 2.5 MB (2536756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba48b7acabab37ea58cc7aaf5b2a2144576b846cab0b0b0be5ff157e55c024a`  
		Last Modified: Sat, 27 Jun 2020 00:35:01 GMT  
		Size: 60.1 MB (60057562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89734c2ad326a224a21a217c3bbbdf11b8d44e364c2998f9db5aa683adf41d63`  
		Last Modified: Sat, 27 Jun 2020 00:34:53 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.7-passenger`

```console
$ docker pull redmine@sha256:69370c9ce1870e27f47b17cc3a1084ac720b1695ed699be24f80e48360f195f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0.7-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:e1df2a54a49f148d4a2a26098b6254a8e608f59574bd4bf5bbd08e2b1013e847
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230959014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5481e26776a3d675958f585a76c23f1639e433e57487fb794c0158619bdbf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:50:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:50:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:50:39 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:50:39 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:50:39 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:50:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:50:40 GMT
ENV REDMINE_VERSION=4.0.7
# Thu, 19 Nov 2020 05:50:41 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Thu, 19 Nov 2020 05:50:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:52:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:52:59 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:52:59 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:52:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:52:59 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:53:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Thu, 19 Nov 2020 05:53:12 GMT
ENV PASSENGER_VERSION=6.0.7
# Thu, 19 Nov 2020 05:53:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:53:29 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Thu, 19 Nov 2020 05:53:30 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Thu, 19 Nov 2020 05:53:30 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ada238ba6ad8b2dd3ee44ebf880f407ef77b6e8ef18564613880076913f91ff`  
		Last Modified: Thu, 19 Nov 2020 05:54:42 GMT  
		Size: 80.2 MB (80211306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a962dc4ad4915e05c9361f8d64db6efba63905a16a29e3a47db5e38a65d50`  
		Last Modified: Thu, 19 Nov 2020 05:54:27 GMT  
		Size: 1.4 MB (1355881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef70e0cbc1210c5711bca0a07af598051ffe8aa854083ba02c2e885409e3c3`  
		Last Modified: Thu, 19 Nov 2020 05:54:25 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8606322853346140003f3bb117f00370f60cd3747ae532eac6438f8d766e8b`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15201977050c5f95385464b7e3b2cbdff5d113bc06bc3d11a5177dd9378ab76`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 2.5 MB (2535006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dcabfc99984272250e6813b788ff805bc12b10fd5dea5037876fb46edc03d5`  
		Last Modified: Thu, 19 Nov 2020 05:54:34 GMT  
		Size: 60.9 MB (60880885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867e85145489202033bc67d43fcb68494d7f08492ac3fe16391d1c4aaea9fc5`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58de2fb61411ab3c2eb56884cb2bc477dede310850076fb6f7bd0dcd08f7d2f6`  
		Last Modified: Thu, 19 Nov 2020 05:54:52 GMT  
		Size: 20.0 MB (19954441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b6ce75cc17d96618a4420ed4e2caec18ec9618bacccde640f4342a385edee`  
		Last Modified: Thu, 19 Nov 2020 05:54:49 GMT  
		Size: 4.9 MB (4921932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-alpine`

```console
$ docker pull redmine@sha256:ad7382f05ccf37ce1612e65b6a480211ab7d82e421cf40b8882d4158fb2142ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:5ab5b25a7f6cd570c5dfe652fab11c71b2005262a5e5e84c3606c79a4e3a4b5b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.9 MB (172913667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:201e41566cd75f7407ac15b8c4141bd86192131e9aa378924e24a484be64a7ea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:01:32 GMT
RUN apk add --no-cache 		gmp-dev
# Fri, 24 Apr 2020 13:01:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 26 Jun 2020 21:31:26 GMT
ENV LANG=C.UTF-8
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 26 Jun 2020 21:58:02 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 26 Jun 2020 22:02:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 26 Jun 2020 22:02:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Jun 2020 22:02:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 26 Jun 2020 22:02:57 GMT
CMD ["irb"]
# Sat, 27 Jun 2020 00:25:13 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 27 Jun 2020 00:31:21 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Sat, 27 Jun 2020 00:31:22 GMT
ENV RAILS_ENV=production
# Sat, 27 Jun 2020 00:31:22 GMT
WORKDIR /usr/src/redmine
# Sat, 27 Jun 2020 00:31:22 GMT
ENV HOME=/home/redmine
# Sat, 27 Jun 2020 00:31:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 27 Jun 2020 00:31:23 GMT
ENV REDMINE_VERSION=4.0.7
# Sat, 27 Jun 2020 00:31:23 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Sat, 27 Jun 2020 00:31:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 27 Jun 2020 00:33:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Jun 2020 00:33:04 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 27 Jun 2020 00:33:04 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 27 Jun 2020 00:33:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 27 Jun 2020 00:33:05 GMT
EXPOSE 3000
# Sat, 27 Jun 2020 00:33:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8ae8202b42d1c70c3a7f65680eabc1c562a29227549b9a1b33dc03943b20d2`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 1.1 MB (1131841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21786fe7c0d7561a5b89ca15d8a1c3e4ea673820cd79f1308bdfd8eb3cb7142`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb235115f8edc3a10cc9c312b6e1abb565211c93fa76ab48d17268515854e8be`  
		Last Modified: Fri, 26 Jun 2020 22:32:52 GMT  
		Size: 22.0 MB (22034884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c29a4c064b384d769d0155220d34ae1d2fddf90c92c2da398542082e780530`  
		Last Modified: Fri, 26 Jun 2020 22:32:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c476068e888bb1f351101b749200705a002008950a4e439b52a7b4c7d918fcb`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14876154f43c2933de788e3f4d1c5d8f032f1e67d81fe9950b35b0c036bc95b`  
		Last Modified: Sat, 27 Jun 2020 00:35:12 GMT  
		Size: 84.3 MB (84335465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7eef6551123b1102419f8867186a7430e1f29913c500ef5efa543f27818974`  
		Last Modified: Sat, 27 Jun 2020 00:34:53 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68ed76f4a7e483ddf6d602bfbd15c28c63ff1e062dbb401fc2e4523c79d8636`  
		Last Modified: Sat, 27 Jun 2020 00:34:53 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351e11b4834cabb36d0909293bb99b488be2f141b52752722f2c21bd34b33fb0`  
		Last Modified: Sat, 27 Jun 2020 00:34:54 GMT  
		Size: 2.5 MB (2536756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba48b7acabab37ea58cc7aaf5b2a2144576b846cab0b0b0be5ff157e55c024a`  
		Last Modified: Sat, 27 Jun 2020 00:35:01 GMT  
		Size: 60.1 MB (60057562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89734c2ad326a224a21a217c3bbbdf11b8d44e364c2998f9db5aa683adf41d63`  
		Last Modified: Sat, 27 Jun 2020 00:34:53 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-passenger`

```console
$ docker pull redmine@sha256:69370c9ce1870e27f47b17cc3a1084ac720b1695ed699be24f80e48360f195f6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:e1df2a54a49f148d4a2a26098b6254a8e608f59574bd4bf5bbd08e2b1013e847
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230959014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c5481e26776a3d675958f585a76c23f1639e433e57487fb794c0158619bdbf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:50:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:50:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:50:39 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:50:39 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:50:39 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:50:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:50:40 GMT
ENV REDMINE_VERSION=4.0.7
# Thu, 19 Nov 2020 05:50:41 GMT
ENV REDMINE_DOWNLOAD_MD5=baad690fdccd7f0282d53beb0ee2c47b
# Thu, 19 Nov 2020 05:50:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:52:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:52:59 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:52:59 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:52:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:52:59 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:53:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Thu, 19 Nov 2020 05:53:12 GMT
ENV PASSENGER_VERSION=6.0.7
# Thu, 19 Nov 2020 05:53:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:53:29 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Thu, 19 Nov 2020 05:53:30 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Thu, 19 Nov 2020 05:53:30 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ada238ba6ad8b2dd3ee44ebf880f407ef77b6e8ef18564613880076913f91ff`  
		Last Modified: Thu, 19 Nov 2020 05:54:42 GMT  
		Size: 80.2 MB (80211306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0a962dc4ad4915e05c9361f8d64db6efba63905a16a29e3a47db5e38a65d50`  
		Last Modified: Thu, 19 Nov 2020 05:54:27 GMT  
		Size: 1.4 MB (1355881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef70e0cbc1210c5711bca0a07af598051ffe8aa854083ba02c2e885409e3c3`  
		Last Modified: Thu, 19 Nov 2020 05:54:25 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8606322853346140003f3bb117f00370f60cd3747ae532eac6438f8d766e8b`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15201977050c5f95385464b7e3b2cbdff5d113bc06bc3d11a5177dd9378ab76`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 2.5 MB (2535006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94dcabfc99984272250e6813b788ff805bc12b10fd5dea5037876fb46edc03d5`  
		Last Modified: Thu, 19 Nov 2020 05:54:34 GMT  
		Size: 60.9 MB (60880885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a867e85145489202033bc67d43fcb68494d7f08492ac3fe16391d1c4aaea9fc5`  
		Last Modified: Thu, 19 Nov 2020 05:54:26 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58de2fb61411ab3c2eb56884cb2bc477dede310850076fb6f7bd0dcd08f7d2f6`  
		Last Modified: Thu, 19 Nov 2020 05:54:52 GMT  
		Size: 20.0 MB (19954441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b6b6ce75cc17d96618a4420ed4e2caec18ec9618bacccde640f4342a385edee`  
		Last Modified: Thu, 19 Nov 2020 05:54:49 GMT  
		Size: 4.9 MB (4921932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1`

```console
$ docker pull redmine@sha256:4fc25b4212caaa21ba5392c725335c94f9c69c2ac0334a0b16be6f117735c409
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
$ docker pull redmine@sha256:97f04d83cec0d51fb6ea2920706508a33317643816bdb670bc948cf69622f8d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215593452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:229055151ea08ad0130dc9db0123325d794744a53ff2b686ae36ac80998650cb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:47:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:47:41 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:47:41 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:47:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 05:47:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:49:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:20 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:49:20 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:49:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:49:20 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:49:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceaf427bdaab140ab3c03e03e397142d0f07a88cdd442cba1826fb438958620`  
		Last Modified: Thu, 19 Nov 2020 05:54:07 GMT  
		Size: 93.1 MB (93104105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332f2c839082a3548a096495ec34f3bc551c78437af681d10ce1edfb94ee264`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 1.4 MB (1369330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061509154252c143a6b5680bb73dfa52909d4a8b300d809dd0e1ac53da1f12d`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409c9bd29355b0269a77c26db749c2549cfbfca66ffd7dd6b1f04610b2623019`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53142f7c27fe4f4a12dfef13f9a10f4613b03ad98babf32482a6c25ff52f13`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 2.7 MB (2739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee5b56b6eec16ce4e488515ba41448ea784f5bf5a8fc75c36ce898c6b5a46bb`  
		Last Modified: Thu, 19 Nov 2020 05:53:55 GMT  
		Size: 57.3 MB (57280977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c5b8b7f7c3b21ee1b9ea7cbae6a70f0a9cfe48646a3c04077b0fe8c8c8d64`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:23b395e2de1a0731bdddab91d31a709eb752aea2165aae7fdc33a02784b153ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204941869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80962afba0c5bd6eaddbb0316791452c348f5d3c7af3631ff6e156853c949658`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 12:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 12:22:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 12:22:26 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 12:40:14 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 12:45:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 12:45:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:45:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 12:45:18 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 19:54:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 19:55:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:56:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 19:56:27 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 19:56:28 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 19:56:29 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 19:56:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 19:56:31 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 19:56:32 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 19:56:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:00:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:00:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:00:11 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:00:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:00:12 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:00:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7091bf042b25a050f741dc921d43bf4c0c72eb54389f565f5762676e67300f`  
		Last Modified: Fri, 11 Dec 2020 13:11:58 GMT  
		Size: 10.3 MB (10327588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6ad9c9fde8ad2da9cc18e3d6ca0e0cdfcf95751c2ef3ca3b907a1899a08deb`  
		Last Modified: Fri, 11 Dec 2020 13:11:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81aef85a39dd03e9d3f8fab64423b80dea3eee4bf68f6df2bfbed5a7cbd041`  
		Last Modified: Fri, 11 Dec 2020 13:13:17 GMT  
		Size: 20.7 MB (20713612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb8a80d30d5c462ac1282bebf1d5568b7f1c1f982281df0ce4e93c3e6e53ae`  
		Last Modified: Fri, 11 Dec 2020 13:13:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad080b6708861654d51cdb61102ae28988bf5041b5ff8a2c3dedab5101cabe7`  
		Last Modified: Fri, 11 Dec 2020 20:07:56 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25473046e79518d96f411be654f4cc1db33e5f8c92c1051c404972d3ace724`  
		Last Modified: Fri, 11 Dec 2020 20:08:25 GMT  
		Size: 88.7 MB (88684630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a5c2535ec1f07fac6e66a12db43365ad44d2ab38b337dcc96b23a0bff02ed2`  
		Last Modified: Fri, 11 Dec 2020 20:07:55 GMT  
		Size: 1.3 MB (1325720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec2ca9b1e35e4bf9657cd000209470cf63e8ec47965e330b06ff6743522bb`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9add9f870ea1a44a3bbc62c09b726563275b6141f2c7a0c0f36a47b936048df`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74d0c25df9427de71ea7e084c0c76790a9d192a71cd4e5a9af621eebbc260f7`  
		Last Modified: Fri, 11 Dec 2020 20:07:54 GMT  
		Size: 2.7 MB (2739775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a593ef648ed210adc22c1a4231a5b0e604de28da07018d976307255d9531d34`  
		Last Modified: Fri, 11 Dec 2020 20:08:06 GMT  
		Size: 56.3 MB (56302590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497392e307eb7ff39de47f101367f73b69db9589aff0918c1b5f48c20ac24e77`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:91fba4adfa601d02809183e7a3d3e590584d307ae47077700856fcd6a80968f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.1 MB (198095589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c548293de9660d77a7da7898df901c34ac08428786fb2419c1db3731567b7fd2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:25:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:25:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 07:25:07 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 07:52:47 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 07:56:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 07:56:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 07:56:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 07:56:31 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 00:02:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 00:02:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 00:03:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:03:23 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 00:03:24 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 00:03:25 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 00:03:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 00:03:28 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 00:03:29 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 00:03:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 00:06:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:06:41 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 00:06:42 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 00:06:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 00:06:43 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 00:06:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f808f0b3cb34b0decd4c61cf2a3876da6033ec045a98cf6cd42a1991c44120`  
		Last Modified: Wed, 18 Nov 2020 08:20:04 GMT  
		Size: 9.8 MB (9847840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea69b961e8974ee2251411fd6cd5b31ccad490b460b73bf6854d29cf9eaf3`  
		Last Modified: Wed, 18 Nov 2020 08:19:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba22755c3b92f079a1218ec82370a9d002fd6b572f20dd4a296226f6b39d7cf`  
		Last Modified: Wed, 18 Nov 2020 08:21:17 GMT  
		Size: 20.6 MB (20622607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7edcf7ca8b960fd2574835e024db1d8cf6006d7a406395de35ec3361ac7209f`  
		Last Modified: Wed, 18 Nov 2020 08:21:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5460041916d57389e886f4c1925aecccf61a1d4c782e927e6fdbbddfa8045b1e`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27983c99d327dd4affc8333a5814244c1234adb6d7e1d55005e61251c08d53fb`  
		Last Modified: Thu, 19 Nov 2020 00:13:43 GMT  
		Size: 84.7 MB (84725207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1324b22d1b94bc1fad2a134946f0b495ace2068b127aa1006f4f510b7e5bc0`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.3 MB (1318532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6673217b014d5a6178c6420c4617f9232685ff98ebc629d06114ac77e41cb099`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f61d703ff2bb268b7079b253ed5622e6ca490a8a8f5bd70ba641f9064fb52`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2006b3162cef090805e876162a655e5c1705b4ff2780eb5c8d0e1d9586810519`  
		Last Modified: Thu, 19 Nov 2020 00:13:13 GMT  
		Size: 2.7 MB (2739770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5ce813b40ff509195e79c4a1cacf5ed50b1119c974a6a3691327c3d3935ee5`  
		Last Modified: Thu, 19 Nov 2020 00:13:25 GMT  
		Size: 56.1 MB (56122951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c064249f5e00ecd193930b27786723f458d9c7ada61caa91c6ba24c3a6442754`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:70de4f1e65da97eaf03494bc73f5e26f0680cefd7ebb1701b49e8fb8a4581f47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211343295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474ecb6ae80c0e9082c661aeaa14620d930adf2096eb04e7fffc2dad0e9bf1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 10:02:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 10:02:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 10:02:22 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 10:16:52 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 10:20:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 10:20:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 10:20:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 10:20:09 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 03:54:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 03:55:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 03:55:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 03:56:00 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 03:56:01 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 03:56:02 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 03:56:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 03:56:05 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 03:56:06 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 03:56:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 03:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 03:59:13 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 03:59:14 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 03:59:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 03:59:15 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 03:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cfcfe44e857123ffa02834cfe1a4126099c7486ecc0223251b64c1a9482954`  
		Last Modified: Wed, 18 Nov 2020 10:43:14 GMT  
		Size: 11.2 MB (11244662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ea17e8a560a0e781a182aae71bb98b7d6c0f8b59de48c41ca0ba4f9006097c`  
		Last Modified: Wed, 18 Nov 2020 10:43:10 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40bed2a0ea8bd34e9eb6ad5b1402f0e6b5dabcd0e3072f495a0e122b1c66c9d`  
		Last Modified: Wed, 18 Nov 2020 10:44:28 GMT  
		Size: 21.3 MB (21288399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6f60a2ebf322104e26fa3e867de1c11d5a667874b9e15f5bcf80f453d19f7c`  
		Last Modified: Wed, 18 Nov 2020 10:44:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b179d423b480ed400f3a5bf0acd9ebc766db80e8667e50a39528db66304f4`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ce67aa919a56bf635b903ce59af070282c6c74aa7c0543ee0ca64ce559ee15`  
		Last Modified: Thu, 19 Nov 2020 04:07:04 GMT  
		Size: 91.7 MB (91682420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5772509129feac5e394a21dbbd14667f6ec08af6bb678342213070c0e9a1fc0a`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.3 MB (1302832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee2429d8b0d53adc0e45a1d0453f17cceb2c50c101fdc827aaf85ac96035832`  
		Last Modified: Thu, 19 Nov 2020 04:06:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa29860dedc18f73d32ae3fc035269752dc1fd19490ca3eb3f4d619988d659a`  
		Last Modified: Thu, 19 Nov 2020 04:06:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a3b3d232fc7ba6b3c5e37d64edfb61d17a7b418d0f247221f1f10335506595`  
		Last Modified: Thu, 19 Nov 2020 04:06:38 GMT  
		Size: 2.7 MB (2739773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39a9061731cfc320d029edf109fdb55b8ae6162bf0b05e13518337ae6ac1fcf`  
		Last Modified: Thu, 19 Nov 2020 04:06:49 GMT  
		Size: 57.2 MB (57218170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe8386baa19d0b373438491ac57dec304b3c833a541f9e1f61e9fe401f11f3d`  
		Last Modified: Thu, 19 Nov 2020 04:06:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; 386

```console
$ docker pull redmine@sha256:f05ab67f515695946ed6633edf17a3f289dd74a6dd6a9b813b6464087f51f30e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.1 MB (221054301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f7d45a1cc118f7f17322d9714cfaae3593d51621b667169f65018e62675e16`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:50:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:50:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 01:50:18 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 02:18:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 02:18:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 02:18:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 02:18:11 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 16:28:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 16:28:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:29:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:29:06 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 16:29:06 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 16:29:06 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 16:29:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 16:29:07 GMT
ENV REDMINE_VERSION=4.1.1
# Wed, 18 Nov 2020 16:29:07 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Wed, 18 Nov 2020 16:29:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 16:31:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:31:04 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 16:31:04 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 16:31:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:31:04 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 16:31:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fbd9e82fd11f8ad081f5e89024c72f30321709805d508e2e07cfa4ec8dc8da`  
		Last Modified: Wed, 18 Nov 2020 02:49:55 GMT  
		Size: 17.2 MB (17207426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f29890b7d3b20bd4d0d4da045c378afaa0ce98710734a94606b4f565594bcb5`  
		Last Modified: Wed, 18 Nov 2020 02:49:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd96c246e2c6a5f9fd496b0717504aff786edc6b58fb255622543c1af5e99e`  
		Last Modified: Wed, 18 Nov 2020 02:51:17 GMT  
		Size: 20.9 MB (20884752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcbfc10a807c014f44297d6e929aa7c8c5756dab2f54181c1cddc95403951b2`  
		Last Modified: Wed, 18 Nov 2020 02:51:13 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8897bbac36c81c5ca34cd30285949651ac03b8a6d8d3f4163fb7e80c60692494`  
		Last Modified: Wed, 18 Nov 2020 16:35:20 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f55c47f87eb292476768cb1d6c5c4a9133ba389656f8a8e5d3e451fac2e60f`  
		Last Modified: Wed, 18 Nov 2020 16:35:49 GMT  
		Size: 94.7 MB (94727984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357ab763d41a2ce00c108910a7eb09d9a52d6d4b49caefa8fde8f4c1b11d48a`  
		Last Modified: Wed, 18 Nov 2020 16:35:19 GMT  
		Size: 1.3 MB (1337919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae1b38b60e40631615232d45aebb7a34a57cb98eeddc2ac7f85de5c5553c8a`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2748ed72d3978b1a3e4898bd4b8c170ac4a31592455f1aaf90e5f70cef1e6b1d`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1001b3f18050630ba786830c891b880c9faced19fe4a39fcdda8937f88e8e`  
		Last Modified: Wed, 18 Nov 2020 16:35:19 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd148206259b30fbfb7ba54e464954391bce2786b87b584b35352d93a3067f8`  
		Last Modified: Wed, 18 Nov 2020 16:35:32 GMT  
		Size: 56.4 MB (56386149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009c7c03d7e082effcfc58964806b009ab6672b31380597557744e635dcc9f96`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; mips64le

```console
$ docker pull redmine@sha256:35eea7d0cb73b9a686ee12c47df5fef0d96183a64061dd0094dcf56f567d6492
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.4 MB (210421080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5279ec7ab65588c4dfb09e9311640a47e602dd589177dcd0a0bd5e9572cdc31c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:51:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:51:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 15:51:06 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 16:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 16:35:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:35:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 16:35:52 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:18:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:19:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:20:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:20:14 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:20:14 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:20:15 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:20:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:20:17 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 20:20:17 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 20:20:24 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:26:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:26:04 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:26:04 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:26:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:26:05 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:26:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864c3d7d0761fea04a3b1c6ac70ddd82c27b002138b03d3b89fa7be97abceb7`  
		Last Modified: Fri, 11 Dec 2020 16:54:07 GMT  
		Size: 11.6 MB (11608300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c58bddd16db870da684d956706ac7beb34a9a61a1637993de013305758cf280`  
		Last Modified: Fri, 11 Dec 2020 16:53:56 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724bc21f9dc167d33b39911e02e8ca816132ecbc3747d7f141b95a99de70f36`  
		Last Modified: Fri, 11 Dec 2020 16:56:27 GMT  
		Size: 21.6 MB (21637748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64df4fb893d9e4613191d83d82f0cd2b63f149bbfbfd363deec584d9644f4fa6`  
		Last Modified: Fri, 11 Dec 2020 16:56:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c186313904d91e281f8e1831122fcccb8ab04d6412b825dc8f7459bcc551fb`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48af7885230e30ca6d0084380ed8e14750622deb4c94bf05befe441f7523835`  
		Last Modified: Fri, 11 Dec 2020 20:37:10 GMT  
		Size: 90.1 MB (90072579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129e6fa772a517fe09bce5f15f1cbb879f1d2d805028d61c1ed129f9dee551b5`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.3 MB (1256645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c0a4dd492334ab9acc4b786f85e20ff8e91d8f994a47fd7c534f7fed84ec7`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a93c92ba03861a44a149916f51047a1ad284e34b83aeb90bdd4504238c1c1e2`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413a895834fed7a4125630a5fb75fecc0516bc14c6f5664d4d8882925b7760bf`  
		Last Modified: Fri, 11 Dec 2020 20:36:00 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfc83332192097ee67902d601513d8e50030905b3e5a007ac39165eb400dcad`  
		Last Modified: Fri, 11 Dec 2020 20:36:28 GMT  
		Size: 57.3 MB (57332039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a674d2c8b1e024562180c82c0597eba27e91c07e6c1c06c8903a540e1e0bdd3`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:c3ea73afabbf5abdfb628b2873fb45815d1ef4c9b95b572a9a0015e6945eefe6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227408094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e775c0e85890cfa750dae96663aaa8263ea772923a290760ce0de9b4248dbf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:26:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 12:27:02 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 12:57:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 12:57:42 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 12:57:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 13:05:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 13:06:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 13:06:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 13:06:40 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 22:56:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 23:16:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 23:23:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:24:12 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 23:24:36 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 23:24:57 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 23:25:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 23:26:01 GMT
ENV REDMINE_VERSION=4.1.1
# Wed, 18 Nov 2020 23:26:23 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Wed, 18 Nov 2020 23:27:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 23:36:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:37:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 23:37:14 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 23:37:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 23:37:26 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 23:37:31 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dba4d658f9cef4692709806bbbe7aa3f108b09489d3abadcdd00af26e816`  
		Last Modified: Wed, 18 Nov 2020 13:22:24 GMT  
		Size: 12.7 MB (12687856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f433a44b3fa921ad6d8b09e5619993f6812dfc023bf9c1ef38db8077916dfd3`  
		Last Modified: Wed, 18 Nov 2020 13:22:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6122ffb25e816545dedec8b707cbdea5f9f2b3c7c2a183f9ae488e46c605bb`  
		Last Modified: Wed, 18 Nov 2020 13:24:12 GMT  
		Size: 22.0 MB (21970057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab94d3b1f8973fd676af9a7da7255d83d3fdd27976823cbe4531093d01bb5f37`  
		Last Modified: Wed, 18 Nov 2020 13:24:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88001e8a986c6b8ebd7392d6ff4d5086ad80462ed5989827c839d3bfb4a01256`  
		Last Modified: Thu, 19 Nov 2020 00:19:46 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89539658f86c698aa7459ac0cdc89685e83e9eabb35fda5f82bbafe99f899680`  
		Last Modified: Thu, 19 Nov 2020 00:20:07 GMT  
		Size: 100.3 MB (100343979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3aa80defc7bbd76afb4c318dc49286936ba18a4e02c316b3fea450caf5727`  
		Last Modified: Thu, 19 Nov 2020 00:19:45 GMT  
		Size: 1.3 MB (1290133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46476067be42396f83b1e0b86411f0ebb193a82c64a8b44cfe7fce12fb68a1fc`  
		Last Modified: Thu, 19 Nov 2020 00:19:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec78f45da7bc16720440b5cfb4662425a82274373104d14c4834ed6185111460`  
		Last Modified: Thu, 19 Nov 2020 00:19:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9d4b0e36b50c79e6977f2e38415655d5822d25f34ecf61019611bf963cbddc`  
		Last Modified: Thu, 19 Nov 2020 00:19:40 GMT  
		Size: 2.7 MB (2739776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b6640a34082c8700a151ec61ee56a940ed83e971f04c234b49da0526ed48ee`  
		Last Modified: Thu, 19 Nov 2020 00:19:48 GMT  
		Size: 57.8 MB (57840073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b1969b444ef8f9019b929408c483060e510efd0b8db7764de2391927bb84`  
		Last Modified: Thu, 19 Nov 2020 00:19:38 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; s390x

```console
$ docker pull redmine@sha256:5afbbd3ee43a0df0b0e47bdce40339edfe52fdbb7e15f32b7c99dfe13e037d46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210687321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72abefdbc79df1244ddf76dba03ecf53d87f03826bfee12474c75bdbb7158f8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 14:05:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 14:06:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 14:06:00 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:39:41 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 14:39:42 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 14:39:43 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 14:44:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 14:44:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 14:44:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 14:44:07 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:53:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:53:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:54:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:54:20 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:54:20 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:54:21 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:54:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:54:22 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 20:54:23 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 20:54:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:56:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:56:29 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:56:30 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:56:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:56:30 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:56:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7319ab475e590b72d37f20d16fbbd64f355ac72137f788fba1242aae760a6732`  
		Last Modified: Fri, 11 Dec 2020 14:58:05 GMT  
		Size: 10.8 MB (10796868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81262b7893747b34acbfca1a00cfc0c68a997043db4e4b0ca7c54b95ef42d3`  
		Last Modified: Fri, 11 Dec 2020 14:58:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2d6654f121a57b04ec9b4cd0328c79f7172e853a3c161296394c0a4eff283`  
		Last Modified: Fri, 11 Dec 2020 14:58:43 GMT  
		Size: 21.6 MB (21598273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554cb46f10b3fc8fe21d4894b92fd3a71978d0522f8f8483a20076965f766433`  
		Last Modified: Fri, 11 Dec 2020 14:58:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae3b3620abc202ccd0f4255185baf54839bf2b973b6e861c0d152a91932fdd1`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae562a30e04f377136d022a05202c0e304d868faf41178e4d93747f3dcf4e02`  
		Last Modified: Fri, 11 Dec 2020 21:00:52 GMT  
		Size: 90.8 MB (90834404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cf9abfa62fe46d287e76c82e923fb635c8d76e9daa28663547ae13c6961fde`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.4 MB (1355550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f42b8d97ca9305ed8fee32c1e42ddbe6147d0a1301c149b9465cf97819d559`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9486d1ae34f16fbe53268c5fa17157568a1679208eb74f8046aaf79b5c2ffd4`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a697087fccb24b639a6b93f6da510d3f6ce42ace5d9f9e64cd893108536edf5`  
		Last Modified: Fri, 11 Dec 2020 21:00:37 GMT  
		Size: 2.7 MB (2739767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bda450facc4353a24f90ffab51457fb80d6fcd340d01cda5540157a21f1c0d`  
		Last Modified: Fri, 11 Dec 2020 21:00:43 GMT  
		Size: 57.6 MB (57643997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5351b41a29cb67f7763dbe84a9ee387f3667913e513212ba1d94d227034010`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.1`

```console
$ docker pull redmine@sha256:4fc25b4212caaa21ba5392c725335c94f9c69c2ac0334a0b16be6f117735c409
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

### `redmine:4.1.1` - linux; amd64

```console
$ docker pull redmine@sha256:97f04d83cec0d51fb6ea2920706508a33317643816bdb670bc948cf69622f8d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215593452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:229055151ea08ad0130dc9db0123325d794744a53ff2b686ae36ac80998650cb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:47:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:47:41 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:47:41 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:47:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 05:47:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:49:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:20 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:49:20 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:49:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:49:20 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:49:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceaf427bdaab140ab3c03e03e397142d0f07a88cdd442cba1826fb438958620`  
		Last Modified: Thu, 19 Nov 2020 05:54:07 GMT  
		Size: 93.1 MB (93104105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332f2c839082a3548a096495ec34f3bc551c78437af681d10ce1edfb94ee264`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 1.4 MB (1369330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061509154252c143a6b5680bb73dfa52909d4a8b300d809dd0e1ac53da1f12d`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409c9bd29355b0269a77c26db749c2549cfbfca66ffd7dd6b1f04610b2623019`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53142f7c27fe4f4a12dfef13f9a10f4613b03ad98babf32482a6c25ff52f13`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 2.7 MB (2739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee5b56b6eec16ce4e488515ba41448ea784f5bf5a8fc75c36ce898c6b5a46bb`  
		Last Modified: Thu, 19 Nov 2020 05:53:55 GMT  
		Size: 57.3 MB (57280977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c5b8b7f7c3b21ee1b9ea7cbae6a70f0a9cfe48646a3c04077b0fe8c8c8d64`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:23b395e2de1a0731bdddab91d31a709eb752aea2165aae7fdc33a02784b153ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204941869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80962afba0c5bd6eaddbb0316791452c348f5d3c7af3631ff6e156853c949658`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 12:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 12:22:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 12:22:26 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 12:40:14 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 12:45:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 12:45:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:45:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 12:45:18 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 19:54:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 19:55:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:56:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 19:56:27 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 19:56:28 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 19:56:29 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 19:56:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 19:56:31 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 19:56:32 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 19:56:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:00:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:00:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:00:11 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:00:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:00:12 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:00:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7091bf042b25a050f741dc921d43bf4c0c72eb54389f565f5762676e67300f`  
		Last Modified: Fri, 11 Dec 2020 13:11:58 GMT  
		Size: 10.3 MB (10327588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6ad9c9fde8ad2da9cc18e3d6ca0e0cdfcf95751c2ef3ca3b907a1899a08deb`  
		Last Modified: Fri, 11 Dec 2020 13:11:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81aef85a39dd03e9d3f8fab64423b80dea3eee4bf68f6df2bfbed5a7cbd041`  
		Last Modified: Fri, 11 Dec 2020 13:13:17 GMT  
		Size: 20.7 MB (20713612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb8a80d30d5c462ac1282bebf1d5568b7f1c1f982281df0ce4e93c3e6e53ae`  
		Last Modified: Fri, 11 Dec 2020 13:13:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad080b6708861654d51cdb61102ae28988bf5041b5ff8a2c3dedab5101cabe7`  
		Last Modified: Fri, 11 Dec 2020 20:07:56 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25473046e79518d96f411be654f4cc1db33e5f8c92c1051c404972d3ace724`  
		Last Modified: Fri, 11 Dec 2020 20:08:25 GMT  
		Size: 88.7 MB (88684630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a5c2535ec1f07fac6e66a12db43365ad44d2ab38b337dcc96b23a0bff02ed2`  
		Last Modified: Fri, 11 Dec 2020 20:07:55 GMT  
		Size: 1.3 MB (1325720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec2ca9b1e35e4bf9657cd000209470cf63e8ec47965e330b06ff6743522bb`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9add9f870ea1a44a3bbc62c09b726563275b6141f2c7a0c0f36a47b936048df`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74d0c25df9427de71ea7e084c0c76790a9d192a71cd4e5a9af621eebbc260f7`  
		Last Modified: Fri, 11 Dec 2020 20:07:54 GMT  
		Size: 2.7 MB (2739775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a593ef648ed210adc22c1a4231a5b0e604de28da07018d976307255d9531d34`  
		Last Modified: Fri, 11 Dec 2020 20:08:06 GMT  
		Size: 56.3 MB (56302590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497392e307eb7ff39de47f101367f73b69db9589aff0918c1b5f48c20ac24e77`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:91fba4adfa601d02809183e7a3d3e590584d307ae47077700856fcd6a80968f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.1 MB (198095589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c548293de9660d77a7da7898df901c34ac08428786fb2419c1db3731567b7fd2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:25:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:25:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 07:25:07 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 07:52:47 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 07:56:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 07:56:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 07:56:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 07:56:31 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 00:02:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 00:02:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 00:03:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:03:23 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 00:03:24 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 00:03:25 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 00:03:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 00:03:28 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 00:03:29 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 00:03:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 00:06:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:06:41 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 00:06:42 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 00:06:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 00:06:43 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 00:06:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f808f0b3cb34b0decd4c61cf2a3876da6033ec045a98cf6cd42a1991c44120`  
		Last Modified: Wed, 18 Nov 2020 08:20:04 GMT  
		Size: 9.8 MB (9847840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea69b961e8974ee2251411fd6cd5b31ccad490b460b73bf6854d29cf9eaf3`  
		Last Modified: Wed, 18 Nov 2020 08:19:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba22755c3b92f079a1218ec82370a9d002fd6b572f20dd4a296226f6b39d7cf`  
		Last Modified: Wed, 18 Nov 2020 08:21:17 GMT  
		Size: 20.6 MB (20622607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7edcf7ca8b960fd2574835e024db1d8cf6006d7a406395de35ec3361ac7209f`  
		Last Modified: Wed, 18 Nov 2020 08:21:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5460041916d57389e886f4c1925aecccf61a1d4c782e927e6fdbbddfa8045b1e`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27983c99d327dd4affc8333a5814244c1234adb6d7e1d55005e61251c08d53fb`  
		Last Modified: Thu, 19 Nov 2020 00:13:43 GMT  
		Size: 84.7 MB (84725207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1324b22d1b94bc1fad2a134946f0b495ace2068b127aa1006f4f510b7e5bc0`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.3 MB (1318532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6673217b014d5a6178c6420c4617f9232685ff98ebc629d06114ac77e41cb099`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f61d703ff2bb268b7079b253ed5622e6ca490a8a8f5bd70ba641f9064fb52`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2006b3162cef090805e876162a655e5c1705b4ff2780eb5c8d0e1d9586810519`  
		Last Modified: Thu, 19 Nov 2020 00:13:13 GMT  
		Size: 2.7 MB (2739770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5ce813b40ff509195e79c4a1cacf5ed50b1119c974a6a3691327c3d3935ee5`  
		Last Modified: Thu, 19 Nov 2020 00:13:25 GMT  
		Size: 56.1 MB (56122951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c064249f5e00ecd193930b27786723f458d9c7ada61caa91c6ba24c3a6442754`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:70de4f1e65da97eaf03494bc73f5e26f0680cefd7ebb1701b49e8fb8a4581f47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211343295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474ecb6ae80c0e9082c661aeaa14620d930adf2096eb04e7fffc2dad0e9bf1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 10:02:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 10:02:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 10:02:22 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 10:16:52 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 10:20:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 10:20:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 10:20:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 10:20:09 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 03:54:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 03:55:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 03:55:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 03:56:00 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 03:56:01 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 03:56:02 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 03:56:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 03:56:05 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 03:56:06 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 03:56:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 03:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 03:59:13 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 03:59:14 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 03:59:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 03:59:15 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 03:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cfcfe44e857123ffa02834cfe1a4126099c7486ecc0223251b64c1a9482954`  
		Last Modified: Wed, 18 Nov 2020 10:43:14 GMT  
		Size: 11.2 MB (11244662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ea17e8a560a0e781a182aae71bb98b7d6c0f8b59de48c41ca0ba4f9006097c`  
		Last Modified: Wed, 18 Nov 2020 10:43:10 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40bed2a0ea8bd34e9eb6ad5b1402f0e6b5dabcd0e3072f495a0e122b1c66c9d`  
		Last Modified: Wed, 18 Nov 2020 10:44:28 GMT  
		Size: 21.3 MB (21288399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6f60a2ebf322104e26fa3e867de1c11d5a667874b9e15f5bcf80f453d19f7c`  
		Last Modified: Wed, 18 Nov 2020 10:44:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b179d423b480ed400f3a5bf0acd9ebc766db80e8667e50a39528db66304f4`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ce67aa919a56bf635b903ce59af070282c6c74aa7c0543ee0ca64ce559ee15`  
		Last Modified: Thu, 19 Nov 2020 04:07:04 GMT  
		Size: 91.7 MB (91682420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5772509129feac5e394a21dbbd14667f6ec08af6bb678342213070c0e9a1fc0a`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.3 MB (1302832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee2429d8b0d53adc0e45a1d0453f17cceb2c50c101fdc827aaf85ac96035832`  
		Last Modified: Thu, 19 Nov 2020 04:06:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa29860dedc18f73d32ae3fc035269752dc1fd19490ca3eb3f4d619988d659a`  
		Last Modified: Thu, 19 Nov 2020 04:06:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a3b3d232fc7ba6b3c5e37d64edfb61d17a7b418d0f247221f1f10335506595`  
		Last Modified: Thu, 19 Nov 2020 04:06:38 GMT  
		Size: 2.7 MB (2739773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39a9061731cfc320d029edf109fdb55b8ae6162bf0b05e13518337ae6ac1fcf`  
		Last Modified: Thu, 19 Nov 2020 04:06:49 GMT  
		Size: 57.2 MB (57218170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe8386baa19d0b373438491ac57dec304b3c833a541f9e1f61e9fe401f11f3d`  
		Last Modified: Thu, 19 Nov 2020 04:06:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.1` - linux; 386

```console
$ docker pull redmine@sha256:f05ab67f515695946ed6633edf17a3f289dd74a6dd6a9b813b6464087f51f30e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.1 MB (221054301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f7d45a1cc118f7f17322d9714cfaae3593d51621b667169f65018e62675e16`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:50:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:50:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 01:50:18 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 02:18:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 02:18:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 02:18:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 02:18:11 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 16:28:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 16:28:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:29:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:29:06 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 16:29:06 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 16:29:06 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 16:29:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 16:29:07 GMT
ENV REDMINE_VERSION=4.1.1
# Wed, 18 Nov 2020 16:29:07 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Wed, 18 Nov 2020 16:29:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 16:31:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:31:04 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 16:31:04 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 16:31:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:31:04 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 16:31:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fbd9e82fd11f8ad081f5e89024c72f30321709805d508e2e07cfa4ec8dc8da`  
		Last Modified: Wed, 18 Nov 2020 02:49:55 GMT  
		Size: 17.2 MB (17207426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f29890b7d3b20bd4d0d4da045c378afaa0ce98710734a94606b4f565594bcb5`  
		Last Modified: Wed, 18 Nov 2020 02:49:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd96c246e2c6a5f9fd496b0717504aff786edc6b58fb255622543c1af5e99e`  
		Last Modified: Wed, 18 Nov 2020 02:51:17 GMT  
		Size: 20.9 MB (20884752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcbfc10a807c014f44297d6e929aa7c8c5756dab2f54181c1cddc95403951b2`  
		Last Modified: Wed, 18 Nov 2020 02:51:13 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8897bbac36c81c5ca34cd30285949651ac03b8a6d8d3f4163fb7e80c60692494`  
		Last Modified: Wed, 18 Nov 2020 16:35:20 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f55c47f87eb292476768cb1d6c5c4a9133ba389656f8a8e5d3e451fac2e60f`  
		Last Modified: Wed, 18 Nov 2020 16:35:49 GMT  
		Size: 94.7 MB (94727984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357ab763d41a2ce00c108910a7eb09d9a52d6d4b49caefa8fde8f4c1b11d48a`  
		Last Modified: Wed, 18 Nov 2020 16:35:19 GMT  
		Size: 1.3 MB (1337919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae1b38b60e40631615232d45aebb7a34a57cb98eeddc2ac7f85de5c5553c8a`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2748ed72d3978b1a3e4898bd4b8c170ac4a31592455f1aaf90e5f70cef1e6b1d`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1001b3f18050630ba786830c891b880c9faced19fe4a39fcdda8937f88e8e`  
		Last Modified: Wed, 18 Nov 2020 16:35:19 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd148206259b30fbfb7ba54e464954391bce2786b87b584b35352d93a3067f8`  
		Last Modified: Wed, 18 Nov 2020 16:35:32 GMT  
		Size: 56.4 MB (56386149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009c7c03d7e082effcfc58964806b009ab6672b31380597557744e635dcc9f96`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.1` - linux; mips64le

```console
$ docker pull redmine@sha256:35eea7d0cb73b9a686ee12c47df5fef0d96183a64061dd0094dcf56f567d6492
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.4 MB (210421080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5279ec7ab65588c4dfb09e9311640a47e602dd589177dcd0a0bd5e9572cdc31c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:51:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:51:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 15:51:06 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 16:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 16:35:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:35:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 16:35:52 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:18:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:19:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:20:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:20:14 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:20:14 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:20:15 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:20:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:20:17 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 20:20:17 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 20:20:24 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:26:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:26:04 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:26:04 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:26:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:26:05 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:26:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864c3d7d0761fea04a3b1c6ac70ddd82c27b002138b03d3b89fa7be97abceb7`  
		Last Modified: Fri, 11 Dec 2020 16:54:07 GMT  
		Size: 11.6 MB (11608300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c58bddd16db870da684d956706ac7beb34a9a61a1637993de013305758cf280`  
		Last Modified: Fri, 11 Dec 2020 16:53:56 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724bc21f9dc167d33b39911e02e8ca816132ecbc3747d7f141b95a99de70f36`  
		Last Modified: Fri, 11 Dec 2020 16:56:27 GMT  
		Size: 21.6 MB (21637748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64df4fb893d9e4613191d83d82f0cd2b63f149bbfbfd363deec584d9644f4fa6`  
		Last Modified: Fri, 11 Dec 2020 16:56:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c186313904d91e281f8e1831122fcccb8ab04d6412b825dc8f7459bcc551fb`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48af7885230e30ca6d0084380ed8e14750622deb4c94bf05befe441f7523835`  
		Last Modified: Fri, 11 Dec 2020 20:37:10 GMT  
		Size: 90.1 MB (90072579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129e6fa772a517fe09bce5f15f1cbb879f1d2d805028d61c1ed129f9dee551b5`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.3 MB (1256645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c0a4dd492334ab9acc4b786f85e20ff8e91d8f994a47fd7c534f7fed84ec7`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a93c92ba03861a44a149916f51047a1ad284e34b83aeb90bdd4504238c1c1e2`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413a895834fed7a4125630a5fb75fecc0516bc14c6f5664d4d8882925b7760bf`  
		Last Modified: Fri, 11 Dec 2020 20:36:00 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfc83332192097ee67902d601513d8e50030905b3e5a007ac39165eb400dcad`  
		Last Modified: Fri, 11 Dec 2020 20:36:28 GMT  
		Size: 57.3 MB (57332039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a674d2c8b1e024562180c82c0597eba27e91c07e6c1c06c8903a540e1e0bdd3`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:c3ea73afabbf5abdfb628b2873fb45815d1ef4c9b95b572a9a0015e6945eefe6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227408094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e775c0e85890cfa750dae96663aaa8263ea772923a290760ce0de9b4248dbf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:26:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 12:27:02 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 12:57:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 12:57:42 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 12:57:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 13:05:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 13:06:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 13:06:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 13:06:40 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 22:56:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 23:16:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 23:23:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:24:12 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 23:24:36 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 23:24:57 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 23:25:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 23:26:01 GMT
ENV REDMINE_VERSION=4.1.1
# Wed, 18 Nov 2020 23:26:23 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Wed, 18 Nov 2020 23:27:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 23:36:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:37:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 23:37:14 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 23:37:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 23:37:26 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 23:37:31 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dba4d658f9cef4692709806bbbe7aa3f108b09489d3abadcdd00af26e816`  
		Last Modified: Wed, 18 Nov 2020 13:22:24 GMT  
		Size: 12.7 MB (12687856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f433a44b3fa921ad6d8b09e5619993f6812dfc023bf9c1ef38db8077916dfd3`  
		Last Modified: Wed, 18 Nov 2020 13:22:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6122ffb25e816545dedec8b707cbdea5f9f2b3c7c2a183f9ae488e46c605bb`  
		Last Modified: Wed, 18 Nov 2020 13:24:12 GMT  
		Size: 22.0 MB (21970057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab94d3b1f8973fd676af9a7da7255d83d3fdd27976823cbe4531093d01bb5f37`  
		Last Modified: Wed, 18 Nov 2020 13:24:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88001e8a986c6b8ebd7392d6ff4d5086ad80462ed5989827c839d3bfb4a01256`  
		Last Modified: Thu, 19 Nov 2020 00:19:46 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89539658f86c698aa7459ac0cdc89685e83e9eabb35fda5f82bbafe99f899680`  
		Last Modified: Thu, 19 Nov 2020 00:20:07 GMT  
		Size: 100.3 MB (100343979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3aa80defc7bbd76afb4c318dc49286936ba18a4e02c316b3fea450caf5727`  
		Last Modified: Thu, 19 Nov 2020 00:19:45 GMT  
		Size: 1.3 MB (1290133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46476067be42396f83b1e0b86411f0ebb193a82c64a8b44cfe7fce12fb68a1fc`  
		Last Modified: Thu, 19 Nov 2020 00:19:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec78f45da7bc16720440b5cfb4662425a82274373104d14c4834ed6185111460`  
		Last Modified: Thu, 19 Nov 2020 00:19:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9d4b0e36b50c79e6977f2e38415655d5822d25f34ecf61019611bf963cbddc`  
		Last Modified: Thu, 19 Nov 2020 00:19:40 GMT  
		Size: 2.7 MB (2739776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b6640a34082c8700a151ec61ee56a940ed83e971f04c234b49da0526ed48ee`  
		Last Modified: Thu, 19 Nov 2020 00:19:48 GMT  
		Size: 57.8 MB (57840073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b1969b444ef8f9019b929408c483060e510efd0b8db7764de2391927bb84`  
		Last Modified: Thu, 19 Nov 2020 00:19:38 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.1` - linux; s390x

```console
$ docker pull redmine@sha256:5afbbd3ee43a0df0b0e47bdce40339edfe52fdbb7e15f32b7c99dfe13e037d46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210687321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72abefdbc79df1244ddf76dba03ecf53d87f03826bfee12474c75bdbb7158f8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 14:05:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 14:06:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 14:06:00 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:39:41 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 14:39:42 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 14:39:43 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 14:44:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 14:44:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 14:44:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 14:44:07 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:53:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:53:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:54:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:54:20 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:54:20 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:54:21 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:54:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:54:22 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 20:54:23 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 20:54:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:56:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:56:29 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:56:30 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:56:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:56:30 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:56:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7319ab475e590b72d37f20d16fbbd64f355ac72137f788fba1242aae760a6732`  
		Last Modified: Fri, 11 Dec 2020 14:58:05 GMT  
		Size: 10.8 MB (10796868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81262b7893747b34acbfca1a00cfc0c68a997043db4e4b0ca7c54b95ef42d3`  
		Last Modified: Fri, 11 Dec 2020 14:58:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2d6654f121a57b04ec9b4cd0328c79f7172e853a3c161296394c0a4eff283`  
		Last Modified: Fri, 11 Dec 2020 14:58:43 GMT  
		Size: 21.6 MB (21598273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554cb46f10b3fc8fe21d4894b92fd3a71978d0522f8f8483a20076965f766433`  
		Last Modified: Fri, 11 Dec 2020 14:58:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae3b3620abc202ccd0f4255185baf54839bf2b973b6e861c0d152a91932fdd1`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae562a30e04f377136d022a05202c0e304d868faf41178e4d93747f3dcf4e02`  
		Last Modified: Fri, 11 Dec 2020 21:00:52 GMT  
		Size: 90.8 MB (90834404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cf9abfa62fe46d287e76c82e923fb635c8d76e9daa28663547ae13c6961fde`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.4 MB (1355550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f42b8d97ca9305ed8fee32c1e42ddbe6147d0a1301c149b9465cf97819d559`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9486d1ae34f16fbe53268c5fa17157568a1679208eb74f8046aaf79b5c2ffd4`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a697087fccb24b639a6b93f6da510d3f6ce42ace5d9f9e64cd893108536edf5`  
		Last Modified: Fri, 11 Dec 2020 21:00:37 GMT  
		Size: 2.7 MB (2739767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bda450facc4353a24f90ffab51457fb80d6fcd340d01cda5540157a21f1c0d`  
		Last Modified: Fri, 11 Dec 2020 21:00:43 GMT  
		Size: 57.6 MB (57643997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5351b41a29cb67f7763dbe84a9ee387f3667913e513212ba1d94d227034010`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.1-alpine`

```console
$ docker pull redmine@sha256:deb3e5905b57732069ca7a8101139f4d03539698d15761948fb68e7fcccfbbbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:78fd8d9d940ba992e2a33b657fda2b4cf88782b14790107bf768d45177dd6cc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.5 MB (171497540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a1414db38346739e8aea9ca4c9b429ab68eab03a71c8bd6410e5a295fd4981`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:01:32 GMT
RUN apk add --no-cache 		gmp-dev
# Fri, 24 Apr 2020 13:01:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 26 Jun 2020 21:31:26 GMT
ENV LANG=C.UTF-8
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 26 Jun 2020 21:58:02 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 26 Jun 2020 22:02:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 26 Jun 2020 22:02:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Jun 2020 22:02:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 26 Jun 2020 22:02:57 GMT
CMD ["irb"]
# Sat, 27 Jun 2020 00:25:13 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 27 Jun 2020 00:25:26 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 27 Jun 2020 00:25:27 GMT
ENV RAILS_ENV=production
# Sat, 27 Jun 2020 00:25:27 GMT
WORKDIR /usr/src/redmine
# Sat, 27 Jun 2020 00:25:28 GMT
ENV HOME=/home/redmine
# Sat, 27 Jun 2020 00:25:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 27 Jun 2020 00:25:29 GMT
ENV REDMINE_VERSION=4.1.1
# Sat, 27 Jun 2020 00:25:29 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Sat, 27 Jun 2020 00:25:32 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 27 Jun 2020 00:27:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Jun 2020 00:27:17 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 27 Jun 2020 00:27:17 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 27 Jun 2020 00:27:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 27 Jun 2020 00:27:17 GMT
EXPOSE 3000
# Sat, 27 Jun 2020 00:27:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8ae8202b42d1c70c3a7f65680eabc1c562a29227549b9a1b33dc03943b20d2`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 1.1 MB (1131841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21786fe7c0d7561a5b89ca15d8a1c3e4ea673820cd79f1308bdfd8eb3cb7142`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb235115f8edc3a10cc9c312b6e1abb565211c93fa76ab48d17268515854e8be`  
		Last Modified: Fri, 26 Jun 2020 22:32:52 GMT  
		Size: 22.0 MB (22034884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c29a4c064b384d769d0155220d34ae1d2fddf90c92c2da398542082e780530`  
		Last Modified: Fri, 26 Jun 2020 22:32:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c476068e888bb1f351101b749200705a002008950a4e439b52a7b4c7d918fcb`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45862f5b557674a750247e6b190c60394e0b39aabe07d9b9aaf93d692898e2c4`  
		Last Modified: Sat, 27 Jun 2020 00:34:16 GMT  
		Size: 86.4 MB (86363568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6acc4528111e9b0ffe75dbb915d2acab87480fde026496ddce3b83fe8ec1de`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1784ebb8ec3fd8526b0fa4bf0b54698e1bcd7b576e438d69593d8e83a58b0827`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa2fd8dfdffc038300d0b8bc6adc0e71e6f0f79c354fdec413049bb35475c9`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 2.7 MB (2740358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b4d7861d6f4c034c489f4c7b07e64beba357d0cdaa623e10207d11da6156b4`  
		Last Modified: Sat, 27 Jun 2020 00:34:08 GMT  
		Size: 56.4 MB (56409729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1376d9ce0b49da4e05452216d93a5a6d8637962c939c8499a7f8b70649283474`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.1-passenger`

```console
$ docker pull redmine@sha256:5a4a19b0c0a63edf33e94bfe6c24edf734d7ce5045150a4d1210e334063d44ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:b0480b6630ec7282e8aa09359a5a1700f668c38d8016438e9101ebeeb7c9252f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.5 MB (240467558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c41cc26645f19911933cc36cb8a8a7c5306e0d826c9bf6fffd44a7407b991fe5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:47:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:47:41 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:47:41 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:47:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 05:47:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:49:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:20 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:49:20 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:49:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:49:20 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:49:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Thu, 19 Nov 2020 05:49:39 GMT
ENV PASSENGER_VERSION=6.0.7
# Thu, 19 Nov 2020 05:49:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:57 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Thu, 19 Nov 2020 05:49:57 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Thu, 19 Nov 2020 05:49:58 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceaf427bdaab140ab3c03e03e397142d0f07a88cdd442cba1826fb438958620`  
		Last Modified: Thu, 19 Nov 2020 05:54:07 GMT  
		Size: 93.1 MB (93104105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332f2c839082a3548a096495ec34f3bc551c78437af681d10ce1edfb94ee264`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 1.4 MB (1369330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061509154252c143a6b5680bb73dfa52909d4a8b300d809dd0e1ac53da1f12d`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409c9bd29355b0269a77c26db749c2549cfbfca66ffd7dd6b1f04610b2623019`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53142f7c27fe4f4a12dfef13f9a10f4613b03ad98babf32482a6c25ff52f13`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 2.7 MB (2739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee5b56b6eec16ce4e488515ba41448ea784f5bf5a8fc75c36ce898c6b5a46bb`  
		Last Modified: Thu, 19 Nov 2020 05:53:55 GMT  
		Size: 57.3 MB (57280977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c5b8b7f7c3b21ee1b9ea7cbae6a70f0a9cfe48646a3c04077b0fe8c8c8d64`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe718b527ed48d5acde8b6e369a9906a5742eecf6fb634c03de4658ce359980`  
		Last Modified: Thu, 19 Nov 2020 05:54:18 GMT  
		Size: 20.0 MB (19952149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd401b8b07edacf0f7e26dfa17e1e02a1ff174e3b43f0dacc172b1bcdb18cf6`  
		Last Modified: Thu, 19 Nov 2020 05:54:16 GMT  
		Size: 4.9 MB (4921957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-alpine`

```console
$ docker pull redmine@sha256:deb3e5905b57732069ca7a8101139f4d03539698d15761948fb68e7fcccfbbbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:78fd8d9d940ba992e2a33b657fda2b4cf88782b14790107bf768d45177dd6cc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.5 MB (171497540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a1414db38346739e8aea9ca4c9b429ab68eab03a71c8bd6410e5a295fd4981`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:01:32 GMT
RUN apk add --no-cache 		gmp-dev
# Fri, 24 Apr 2020 13:01:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 26 Jun 2020 21:31:26 GMT
ENV LANG=C.UTF-8
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 26 Jun 2020 21:58:02 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 26 Jun 2020 22:02:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 26 Jun 2020 22:02:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Jun 2020 22:02:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 26 Jun 2020 22:02:57 GMT
CMD ["irb"]
# Sat, 27 Jun 2020 00:25:13 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 27 Jun 2020 00:25:26 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 27 Jun 2020 00:25:27 GMT
ENV RAILS_ENV=production
# Sat, 27 Jun 2020 00:25:27 GMT
WORKDIR /usr/src/redmine
# Sat, 27 Jun 2020 00:25:28 GMT
ENV HOME=/home/redmine
# Sat, 27 Jun 2020 00:25:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 27 Jun 2020 00:25:29 GMT
ENV REDMINE_VERSION=4.1.1
# Sat, 27 Jun 2020 00:25:29 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Sat, 27 Jun 2020 00:25:32 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 27 Jun 2020 00:27:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Jun 2020 00:27:17 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 27 Jun 2020 00:27:17 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 27 Jun 2020 00:27:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 27 Jun 2020 00:27:17 GMT
EXPOSE 3000
# Sat, 27 Jun 2020 00:27:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8ae8202b42d1c70c3a7f65680eabc1c562a29227549b9a1b33dc03943b20d2`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 1.1 MB (1131841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21786fe7c0d7561a5b89ca15d8a1c3e4ea673820cd79f1308bdfd8eb3cb7142`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb235115f8edc3a10cc9c312b6e1abb565211c93fa76ab48d17268515854e8be`  
		Last Modified: Fri, 26 Jun 2020 22:32:52 GMT  
		Size: 22.0 MB (22034884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c29a4c064b384d769d0155220d34ae1d2fddf90c92c2da398542082e780530`  
		Last Modified: Fri, 26 Jun 2020 22:32:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c476068e888bb1f351101b749200705a002008950a4e439b52a7b4c7d918fcb`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45862f5b557674a750247e6b190c60394e0b39aabe07d9b9aaf93d692898e2c4`  
		Last Modified: Sat, 27 Jun 2020 00:34:16 GMT  
		Size: 86.4 MB (86363568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6acc4528111e9b0ffe75dbb915d2acab87480fde026496ddce3b83fe8ec1de`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1784ebb8ec3fd8526b0fa4bf0b54698e1bcd7b576e438d69593d8e83a58b0827`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa2fd8dfdffc038300d0b8bc6adc0e71e6f0f79c354fdec413049bb35475c9`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 2.7 MB (2740358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b4d7861d6f4c034c489f4c7b07e64beba357d0cdaa623e10207d11da6156b4`  
		Last Modified: Sat, 27 Jun 2020 00:34:08 GMT  
		Size: 56.4 MB (56409729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1376d9ce0b49da4e05452216d93a5a6d8637962c939c8499a7f8b70649283474`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-passenger`

```console
$ docker pull redmine@sha256:5a4a19b0c0a63edf33e94bfe6c24edf734d7ce5045150a4d1210e334063d44ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:b0480b6630ec7282e8aa09359a5a1700f668c38d8016438e9101ebeeb7c9252f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.5 MB (240467558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c41cc26645f19911933cc36cb8a8a7c5306e0d826c9bf6fffd44a7407b991fe5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:47:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:47:41 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:47:41 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:47:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 05:47:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:49:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:20 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:49:20 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:49:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:49:20 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:49:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Thu, 19 Nov 2020 05:49:39 GMT
ENV PASSENGER_VERSION=6.0.7
# Thu, 19 Nov 2020 05:49:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:57 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Thu, 19 Nov 2020 05:49:57 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Thu, 19 Nov 2020 05:49:58 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceaf427bdaab140ab3c03e03e397142d0f07a88cdd442cba1826fb438958620`  
		Last Modified: Thu, 19 Nov 2020 05:54:07 GMT  
		Size: 93.1 MB (93104105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332f2c839082a3548a096495ec34f3bc551c78437af681d10ce1edfb94ee264`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 1.4 MB (1369330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061509154252c143a6b5680bb73dfa52909d4a8b300d809dd0e1ac53da1f12d`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409c9bd29355b0269a77c26db749c2549cfbfca66ffd7dd6b1f04610b2623019`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53142f7c27fe4f4a12dfef13f9a10f4613b03ad98babf32482a6c25ff52f13`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 2.7 MB (2739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee5b56b6eec16ce4e488515ba41448ea784f5bf5a8fc75c36ce898c6b5a46bb`  
		Last Modified: Thu, 19 Nov 2020 05:53:55 GMT  
		Size: 57.3 MB (57280977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c5b8b7f7c3b21ee1b9ea7cbae6a70f0a9cfe48646a3c04077b0fe8c8c8d64`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe718b527ed48d5acde8b6e369a9906a5742eecf6fb634c03de4658ce359980`  
		Last Modified: Thu, 19 Nov 2020 05:54:18 GMT  
		Size: 20.0 MB (19952149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd401b8b07edacf0f7e26dfa17e1e02a1ff174e3b43f0dacc172b1bcdb18cf6`  
		Last Modified: Thu, 19 Nov 2020 05:54:16 GMT  
		Size: 4.9 MB (4921957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:deb3e5905b57732069ca7a8101139f4d03539698d15761948fb68e7fcccfbbbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:78fd8d9d940ba992e2a33b657fda2b4cf88782b14790107bf768d45177dd6cc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.5 MB (171497540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a1414db38346739e8aea9ca4c9b429ab68eab03a71c8bd6410e5a295fd4981`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:01:32 GMT
RUN apk add --no-cache 		gmp-dev
# Fri, 24 Apr 2020 13:01:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 26 Jun 2020 21:31:26 GMT
ENV LANG=C.UTF-8
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 26 Jun 2020 21:58:02 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 26 Jun 2020 22:02:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 26 Jun 2020 22:02:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Jun 2020 22:02:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 26 Jun 2020 22:02:57 GMT
CMD ["irb"]
# Sat, 27 Jun 2020 00:25:13 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 27 Jun 2020 00:25:26 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 27 Jun 2020 00:25:27 GMT
ENV RAILS_ENV=production
# Sat, 27 Jun 2020 00:25:27 GMT
WORKDIR /usr/src/redmine
# Sat, 27 Jun 2020 00:25:28 GMT
ENV HOME=/home/redmine
# Sat, 27 Jun 2020 00:25:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 27 Jun 2020 00:25:29 GMT
ENV REDMINE_VERSION=4.1.1
# Sat, 27 Jun 2020 00:25:29 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Sat, 27 Jun 2020 00:25:32 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 27 Jun 2020 00:27:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Jun 2020 00:27:17 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 27 Jun 2020 00:27:17 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 27 Jun 2020 00:27:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 27 Jun 2020 00:27:17 GMT
EXPOSE 3000
# Sat, 27 Jun 2020 00:27:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8ae8202b42d1c70c3a7f65680eabc1c562a29227549b9a1b33dc03943b20d2`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 1.1 MB (1131841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21786fe7c0d7561a5b89ca15d8a1c3e4ea673820cd79f1308bdfd8eb3cb7142`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb235115f8edc3a10cc9c312b6e1abb565211c93fa76ab48d17268515854e8be`  
		Last Modified: Fri, 26 Jun 2020 22:32:52 GMT  
		Size: 22.0 MB (22034884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c29a4c064b384d769d0155220d34ae1d2fddf90c92c2da398542082e780530`  
		Last Modified: Fri, 26 Jun 2020 22:32:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c476068e888bb1f351101b749200705a002008950a4e439b52a7b4c7d918fcb`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45862f5b557674a750247e6b190c60394e0b39aabe07d9b9aaf93d692898e2c4`  
		Last Modified: Sat, 27 Jun 2020 00:34:16 GMT  
		Size: 86.4 MB (86363568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6acc4528111e9b0ffe75dbb915d2acab87480fde026496ddce3b83fe8ec1de`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1784ebb8ec3fd8526b0fa4bf0b54698e1bcd7b576e438d69593d8e83a58b0827`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa2fd8dfdffc038300d0b8bc6adc0e71e6f0f79c354fdec413049bb35475c9`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 2.7 MB (2740358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b4d7861d6f4c034c489f4c7b07e64beba357d0cdaa623e10207d11da6156b4`  
		Last Modified: Sat, 27 Jun 2020 00:34:08 GMT  
		Size: 56.4 MB (56409729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1376d9ce0b49da4e05452216d93a5a6d8637962c939c8499a7f8b70649283474`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:5a4a19b0c0a63edf33e94bfe6c24edf734d7ce5045150a4d1210e334063d44ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:b0480b6630ec7282e8aa09359a5a1700f668c38d8016438e9101ebeeb7c9252f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.5 MB (240467558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c41cc26645f19911933cc36cb8a8a7c5306e0d826c9bf6fffd44a7407b991fe5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:47:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:47:41 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:47:41 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:47:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 05:47:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:49:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:20 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:49:20 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:49:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:49:20 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:49:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Thu, 19 Nov 2020 05:49:39 GMT
ENV PASSENGER_VERSION=6.0.7
# Thu, 19 Nov 2020 05:49:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:57 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Thu, 19 Nov 2020 05:49:57 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Thu, 19 Nov 2020 05:49:58 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceaf427bdaab140ab3c03e03e397142d0f07a88cdd442cba1826fb438958620`  
		Last Modified: Thu, 19 Nov 2020 05:54:07 GMT  
		Size: 93.1 MB (93104105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332f2c839082a3548a096495ec34f3bc551c78437af681d10ce1edfb94ee264`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 1.4 MB (1369330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061509154252c143a6b5680bb73dfa52909d4a8b300d809dd0e1ac53da1f12d`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409c9bd29355b0269a77c26db749c2549cfbfca66ffd7dd6b1f04610b2623019`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53142f7c27fe4f4a12dfef13f9a10f4613b03ad98babf32482a6c25ff52f13`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 2.7 MB (2739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee5b56b6eec16ce4e488515ba41448ea784f5bf5a8fc75c36ce898c6b5a46bb`  
		Last Modified: Thu, 19 Nov 2020 05:53:55 GMT  
		Size: 57.3 MB (57280977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c5b8b7f7c3b21ee1b9ea7cbae6a70f0a9cfe48646a3c04077b0fe8c8c8d64`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe718b527ed48d5acde8b6e369a9906a5742eecf6fb634c03de4658ce359980`  
		Last Modified: Thu, 19 Nov 2020 05:54:18 GMT  
		Size: 20.0 MB (19952149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd401b8b07edacf0f7e26dfa17e1e02a1ff174e3b43f0dacc172b1bcdb18cf6`  
		Last Modified: Thu, 19 Nov 2020 05:54:16 GMT  
		Size: 4.9 MB (4921957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:alpine`

```console
$ docker pull redmine@sha256:deb3e5905b57732069ca7a8101139f4d03539698d15761948fb68e7fcccfbbbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:78fd8d9d940ba992e2a33b657fda2b4cf88782b14790107bf768d45177dd6cc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.5 MB (171497540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08a1414db38346739e8aea9ca4c9b429ab68eab03a71c8bd6410e5a295fd4981`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 13:01:32 GMT
RUN apk add --no-cache 		gmp-dev
# Fri, 24 Apr 2020 13:01:32 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 26 Jun 2020 21:31:26 GMT
ENV LANG=C.UTF-8
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 26 Jun 2020 21:58:01 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 26 Jun 2020 21:58:02 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 26 Jun 2020 22:02:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 26 Jun 2020 22:02:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 26 Jun 2020 22:02:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 26 Jun 2020 22:02:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 26 Jun 2020 22:02:57 GMT
CMD ["irb"]
# Sat, 27 Jun 2020 00:25:13 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 27 Jun 2020 00:25:26 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 27 Jun 2020 00:25:27 GMT
ENV RAILS_ENV=production
# Sat, 27 Jun 2020 00:25:27 GMT
WORKDIR /usr/src/redmine
# Sat, 27 Jun 2020 00:25:28 GMT
ENV HOME=/home/redmine
# Sat, 27 Jun 2020 00:25:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 27 Jun 2020 00:25:29 GMT
ENV REDMINE_VERSION=4.1.1
# Sat, 27 Jun 2020 00:25:29 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Sat, 27 Jun 2020 00:25:32 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 27 Jun 2020 00:27:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Jun 2020 00:27:17 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 27 Jun 2020 00:27:17 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 27 Jun 2020 00:27:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 27 Jun 2020 00:27:17 GMT
EXPOSE 3000
# Sat, 27 Jun 2020 00:27:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8ae8202b42d1c70c3a7f65680eabc1c562a29227549b9a1b33dc03943b20d2`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 1.1 MB (1131841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21786fe7c0d7561a5b89ca15d8a1c3e4ea673820cd79f1308bdfd8eb3cb7142`  
		Last Modified: Fri, 24 Apr 2020 13:21:01 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb235115f8edc3a10cc9c312b6e1abb565211c93fa76ab48d17268515854e8be`  
		Last Modified: Fri, 26 Jun 2020 22:32:52 GMT  
		Size: 22.0 MB (22034884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c29a4c064b384d769d0155220d34ae1d2fddf90c92c2da398542082e780530`  
		Last Modified: Fri, 26 Jun 2020 22:32:47 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c476068e888bb1f351101b749200705a002008950a4e439b52a7b4c7d918fcb`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45862f5b557674a750247e6b190c60394e0b39aabe07d9b9aaf93d692898e2c4`  
		Last Modified: Sat, 27 Jun 2020 00:34:16 GMT  
		Size: 86.4 MB (86363568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6acc4528111e9b0ffe75dbb915d2acab87480fde026496ddce3b83fe8ec1de`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 135.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1784ebb8ec3fd8526b0fa4bf0b54698e1bcd7b576e438d69593d8e83a58b0827`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abaa2fd8dfdffc038300d0b8bc6adc0e71e6f0f79c354fdec413049bb35475c9`  
		Last Modified: Sat, 27 Jun 2020 00:33:58 GMT  
		Size: 2.7 MB (2740358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b4d7861d6f4c034c489f4c7b07e64beba357d0cdaa623e10207d11da6156b4`  
		Last Modified: Sat, 27 Jun 2020 00:34:08 GMT  
		Size: 56.4 MB (56409729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1376d9ce0b49da4e05452216d93a5a6d8637962c939c8499a7f8b70649283474`  
		Last Modified: Sat, 27 Jun 2020 00:33:56 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:latest`

```console
$ docker pull redmine@sha256:4fc25b4212caaa21ba5392c725335c94f9c69c2ac0334a0b16be6f117735c409
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
$ docker pull redmine@sha256:97f04d83cec0d51fb6ea2920706508a33317643816bdb670bc948cf69622f8d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.6 MB (215593452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:229055151ea08ad0130dc9db0123325d794744a53ff2b686ae36ac80998650cb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:47:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:47:41 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:47:41 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:47:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 05:47:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:49:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:20 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:49:20 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:49:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:49:20 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:49:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceaf427bdaab140ab3c03e03e397142d0f07a88cdd442cba1826fb438958620`  
		Last Modified: Thu, 19 Nov 2020 05:54:07 GMT  
		Size: 93.1 MB (93104105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332f2c839082a3548a096495ec34f3bc551c78437af681d10ce1edfb94ee264`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 1.4 MB (1369330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061509154252c143a6b5680bb73dfa52909d4a8b300d809dd0e1ac53da1f12d`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409c9bd29355b0269a77c26db749c2549cfbfca66ffd7dd6b1f04610b2623019`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53142f7c27fe4f4a12dfef13f9a10f4613b03ad98babf32482a6c25ff52f13`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 2.7 MB (2739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee5b56b6eec16ce4e488515ba41448ea784f5bf5a8fc75c36ce898c6b5a46bb`  
		Last Modified: Thu, 19 Nov 2020 05:53:55 GMT  
		Size: 57.3 MB (57280977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c5b8b7f7c3b21ee1b9ea7cbae6a70f0a9cfe48646a3c04077b0fe8c8c8d64`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:23b395e2de1a0731bdddab91d31a709eb752aea2165aae7fdc33a02784b153ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204941869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80962afba0c5bd6eaddbb0316791452c348f5d3c7af3631ff6e156853c949658`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:49 GMT
ADD file:58ebb3ffaf26d9b7621efba5f109ae9d22832f2f22865cda36604b138cbdb7b8 in / 
# Fri, 11 Dec 2020 02:04:56 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 12:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 12:22:25 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 12:22:26 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 12:40:13 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 12:40:14 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 12:45:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 12:45:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 12:45:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 12:45:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 12:45:18 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 19:54:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 19:55:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 19:56:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 19:56:27 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 19:56:28 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 19:56:29 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 19:56:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 19:56:31 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 19:56:32 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 19:56:38 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:00:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:00:09 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:00:11 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:00:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:00:12 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:00:12 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8cbd1f790d64c77fcac6c9dbfe4d4c82f0365de9438f1a42b0560dc88f9e6a55`  
		Last Modified: Fri, 11 Dec 2020 02:14:44 GMT  
		Size: 24.8 MB (24843461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7091bf042b25a050f741dc921d43bf4c0c72eb54389f565f5762676e67300f`  
		Last Modified: Fri, 11 Dec 2020 13:11:58 GMT  
		Size: 10.3 MB (10327588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6ad9c9fde8ad2da9cc18e3d6ca0e0cdfcf95751c2ef3ca3b907a1899a08deb`  
		Last Modified: Fri, 11 Dec 2020 13:11:52 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c81aef85a39dd03e9d3f8fab64423b80dea3eee4bf68f6df2bfbed5a7cbd041`  
		Last Modified: Fri, 11 Dec 2020 13:13:17 GMT  
		Size: 20.7 MB (20713612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bb8a80d30d5c462ac1282bebf1d5568b7f1c1f982281df0ce4e93c3e6e53ae`  
		Last Modified: Fri, 11 Dec 2020 13:13:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cad080b6708861654d51cdb61102ae28988bf5041b5ff8a2c3dedab5101cabe7`  
		Last Modified: Fri, 11 Dec 2020 20:07:56 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e25473046e79518d96f411be654f4cc1db33e5f8c92c1051c404972d3ace724`  
		Last Modified: Fri, 11 Dec 2020 20:08:25 GMT  
		Size: 88.7 MB (88684630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a5c2535ec1f07fac6e66a12db43365ad44d2ab38b337dcc96b23a0bff02ed2`  
		Last Modified: Fri, 11 Dec 2020 20:07:55 GMT  
		Size: 1.3 MB (1325720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f5ec2ca9b1e35e4bf9657cd000209470cf63e8ec47965e330b06ff6743522bb`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9add9f870ea1a44a3bbc62c09b726563275b6141f2c7a0c0f36a47b936048df`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74d0c25df9427de71ea7e084c0c76790a9d192a71cd4e5a9af621eebbc260f7`  
		Last Modified: Fri, 11 Dec 2020 20:07:54 GMT  
		Size: 2.7 MB (2739775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a593ef648ed210adc22c1a4231a5b0e604de28da07018d976307255d9531d34`  
		Last Modified: Fri, 11 Dec 2020 20:08:06 GMT  
		Size: 56.3 MB (56302590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497392e307eb7ff39de47f101367f73b69db9589aff0918c1b5f48c20ac24e77`  
		Last Modified: Fri, 11 Dec 2020 20:07:53 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:91fba4adfa601d02809183e7a3d3e590584d307ae47077700856fcd6a80968f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.1 MB (198095589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c548293de9660d77a7da7898df901c34ac08428786fb2419c1db3731567b7fd2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:06 GMT
ADD file:2035658a8d20545ee7b2ab3ee791a371925fca7968ac29435303da24a1378f34 in / 
# Tue, 17 Nov 2020 20:21:10 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 07:25:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 07:25:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 07:25:07 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 07:52:45 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 07:52:47 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 07:56:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 07:56:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:26 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 07:56:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 07:56:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 07:56:31 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 00:02:06 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 00:02:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 00:03:22 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:03:23 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 00:03:24 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 00:03:25 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 00:03:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 00:03:28 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 00:03:29 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 00:03:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 00:06:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 00:06:41 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 00:06:42 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 00:06:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 00:06:43 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 00:06:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d5029e4b387017f20ad9f77baf3b81dd41f851d6340363b842a8a1d9786a60a0`  
		Last Modified: Tue, 17 Nov 2020 20:31:46 GMT  
		Size: 22.7 MB (22714186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f808f0b3cb34b0decd4c61cf2a3876da6033ec045a98cf6cd42a1991c44120`  
		Last Modified: Wed, 18 Nov 2020 08:20:04 GMT  
		Size: 9.8 MB (9847840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661ea69b961e8974ee2251411fd6cd5b31ccad490b460b73bf6854d29cf9eaf3`  
		Last Modified: Wed, 18 Nov 2020 08:19:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba22755c3b92f079a1218ec82370a9d002fd6b572f20dd4a296226f6b39d7cf`  
		Last Modified: Wed, 18 Nov 2020 08:21:17 GMT  
		Size: 20.6 MB (20622607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7edcf7ca8b960fd2574835e024db1d8cf6006d7a406395de35ec3361ac7209f`  
		Last Modified: Wed, 18 Nov 2020 08:21:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5460041916d57389e886f4c1925aecccf61a1d4c782e927e6fdbbddfa8045b1e`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27983c99d327dd4affc8333a5814244c1234adb6d7e1d55005e61251c08d53fb`  
		Last Modified: Thu, 19 Nov 2020 00:13:43 GMT  
		Size: 84.7 MB (84725207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1324b22d1b94bc1fad2a134946f0b495ace2068b127aa1006f4f510b7e5bc0`  
		Last Modified: Thu, 19 Nov 2020 00:13:14 GMT  
		Size: 1.3 MB (1318532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6673217b014d5a6178c6420c4617f9232685ff98ebc629d06114ac77e41cb099`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f61d703ff2bb268b7079b253ed5622e6ca490a8a8f5bd70ba641f9064fb52`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2006b3162cef090805e876162a655e5c1705b4ff2780eb5c8d0e1d9586810519`  
		Last Modified: Thu, 19 Nov 2020 00:13:13 GMT  
		Size: 2.7 MB (2739770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5ce813b40ff509195e79c4a1cacf5ed50b1119c974a6a3691327c3d3935ee5`  
		Last Modified: Thu, 19 Nov 2020 00:13:25 GMT  
		Size: 56.1 MB (56122951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c064249f5e00ecd193930b27786723f458d9c7ada61caa91c6ba24c3a6442754`  
		Last Modified: Thu, 19 Nov 2020 00:13:11 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:70de4f1e65da97eaf03494bc73f5e26f0680cefd7ebb1701b49e8fb8a4581f47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211343295 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474ecb6ae80c0e9082c661aeaa14620d930adf2096eb04e7fffc2dad0e9bf1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:31 GMT
ADD file:a70d8c01f8f04f36038968567af779883f3b5ba3147b662b7d170d80418bc23c in / 
# Tue, 17 Nov 2020 20:23:32 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 10:02:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 10:02:21 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 10:02:22 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 10:16:52 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 10:16:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 10:20:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 10:20:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 10:20:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 10:20:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 10:20:09 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 03:54:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 03:55:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 03:55:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 03:56:00 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 03:56:01 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 03:56:02 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 03:56:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 03:56:05 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 03:56:06 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 03:56:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 03:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 03:59:13 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 03:59:14 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 03:59:14 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 03:59:15 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 03:59:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:29ade854e0dcedde295dd89890d45271e9df839e42124558eb5283508ca70f5c`  
		Last Modified: Tue, 17 Nov 2020 20:32:02 GMT  
		Size: 25.9 MB (25862532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cfcfe44e857123ffa02834cfe1a4126099c7486ecc0223251b64c1a9482954`  
		Last Modified: Wed, 18 Nov 2020 10:43:14 GMT  
		Size: 11.2 MB (11244662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ea17e8a560a0e781a182aae71bb98b7d6c0f8b59de48c41ca0ba4f9006097c`  
		Last Modified: Wed, 18 Nov 2020 10:43:10 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40bed2a0ea8bd34e9eb6ad5b1402f0e6b5dabcd0e3072f495a0e122b1c66c9d`  
		Last Modified: Wed, 18 Nov 2020 10:44:28 GMT  
		Size: 21.3 MB (21288399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6f60a2ebf322104e26fa3e867de1c11d5a667874b9e15f5bcf80f453d19f7c`  
		Last Modified: Wed, 18 Nov 2020 10:44:24 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1b179d423b480ed400f3a5bf0acd9ebc766db80e8667e50a39528db66304f4`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ce67aa919a56bf635b903ce59af070282c6c74aa7c0543ee0ca64ce559ee15`  
		Last Modified: Thu, 19 Nov 2020 04:07:04 GMT  
		Size: 91.7 MB (91682420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5772509129feac5e394a21dbbd14667f6ec08af6bb678342213070c0e9a1fc0a`  
		Last Modified: Thu, 19 Nov 2020 04:06:39 GMT  
		Size: 1.3 MB (1302832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee2429d8b0d53adc0e45a1d0453f17cceb2c50c101fdc827aaf85ac96035832`  
		Last Modified: Thu, 19 Nov 2020 04:06:36 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa29860dedc18f73d32ae3fc035269752dc1fd19490ca3eb3f4d619988d659a`  
		Last Modified: Thu, 19 Nov 2020 04:06:37 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a3b3d232fc7ba6b3c5e37d64edfb61d17a7b418d0f247221f1f10335506595`  
		Last Modified: Thu, 19 Nov 2020 04:06:38 GMT  
		Size: 2.7 MB (2739773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39a9061731cfc320d029edf109fdb55b8ae6162bf0b05e13518337ae6ac1fcf`  
		Last Modified: Thu, 19 Nov 2020 04:06:49 GMT  
		Size: 57.2 MB (57218170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe8386baa19d0b373438491ac57dec304b3c833a541f9e1f61e9fe401f11f3d`  
		Last Modified: Thu, 19 Nov 2020 04:06:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:f05ab67f515695946ed6633edf17a3f289dd74a6dd6a9b813b6464087f51f30e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.1 MB (221054301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29f7d45a1cc118f7f17322d9714cfaae3593d51621b667169f65018e62675e16`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:58 GMT
ADD file:b17dfa607fcb298beb9c58bfbb8b9b0743ceb385875776c56269db2506840edf in / 
# Tue, 17 Nov 2020 20:19:58 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 01:50:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 01:50:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 01:50:18 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 02:12:58 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 02:18:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 02:18:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 02:18:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 02:18:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 02:18:11 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 16:28:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 16:28:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 16:29:05 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:29:06 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 16:29:06 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 16:29:06 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 16:29:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 16:29:07 GMT
ENV REDMINE_VERSION=4.1.1
# Wed, 18 Nov 2020 16:29:07 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Wed, 18 Nov 2020 16:29:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 16:31:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 16:31:04 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 16:31:04 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 16:31:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 16:31:04 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 16:31:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e8e82c9fb36b8f3a9b8f18fe1d88e4d425d5c45968e3f2e94cdbb1255feb4878`  
		Last Modified: Tue, 17 Nov 2020 20:26:45 GMT  
		Size: 27.8 MB (27766186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56fbd9e82fd11f8ad081f5e89024c72f30321709805d508e2e07cfa4ec8dc8da`  
		Last Modified: Wed, 18 Nov 2020 02:49:55 GMT  
		Size: 17.2 MB (17207426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f29890b7d3b20bd4d0d4da045c378afaa0ce98710734a94606b4f565594bcb5`  
		Last Modified: Wed, 18 Nov 2020 02:49:47 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95bd96c246e2c6a5f9fd496b0717504aff786edc6b58fb255622543c1af5e99e`  
		Last Modified: Wed, 18 Nov 2020 02:51:17 GMT  
		Size: 20.9 MB (20884752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfcbfc10a807c014f44297d6e929aa7c8c5756dab2f54181c1cddc95403951b2`  
		Last Modified: Wed, 18 Nov 2020 02:51:13 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8897bbac36c81c5ca34cd30285949651ac03b8a6d8d3f4163fb7e80c60692494`  
		Last Modified: Wed, 18 Nov 2020 16:35:20 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f55c47f87eb292476768cb1d6c5c4a9133ba389656f8a8e5d3e451fac2e60f`  
		Last Modified: Wed, 18 Nov 2020 16:35:49 GMT  
		Size: 94.7 MB (94727984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7357ab763d41a2ce00c108910a7eb09d9a52d6d4b49caefa8fde8f4c1b11d48a`  
		Last Modified: Wed, 18 Nov 2020 16:35:19 GMT  
		Size: 1.3 MB (1337919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae1b38b60e40631615232d45aebb7a34a57cb98eeddc2ac7f85de5c5553c8a`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2748ed72d3978b1a3e4898bd4b8c170ac4a31592455f1aaf90e5f70cef1e6b1d`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d1001b3f18050630ba786830c891b880c9faced19fe4a39fcdda8937f88e8e`  
		Last Modified: Wed, 18 Nov 2020 16:35:19 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd148206259b30fbfb7ba54e464954391bce2786b87b584b35352d93a3067f8`  
		Last Modified: Wed, 18 Nov 2020 16:35:32 GMT  
		Size: 56.4 MB (56386149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009c7c03d7e082effcfc58964806b009ab6672b31380597557744e635dcc9f96`  
		Last Modified: Wed, 18 Nov 2020 16:35:17 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; mips64le

```console
$ docker pull redmine@sha256:35eea7d0cb73b9a686ee12c47df5fef0d96183a64061dd0094dcf56f567d6492
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.4 MB (210421080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5279ec7ab65588c4dfb09e9311640a47e602dd589177dcd0a0bd5e9572cdc31c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:30 GMT
ADD file:edb758d587972f30ef28b162dcabf79f61b685afa3c6066cb611c61abea124f3 in / 
# Fri, 11 Dec 2020 02:03:30 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:51:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:51:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 15:51:06 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 16:27:22 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 16:35:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 16:35:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 16:35:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 16:35:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 16:35:52 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:18:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:19:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:20:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:20:14 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:20:14 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:20:15 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:20:16 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:20:17 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 20:20:17 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 20:20:24 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:26:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:26:04 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:26:04 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:26:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:26:05 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:26:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:bed35f8e8e003f268bd91c8bc28d93f0b1463296add14ab3ec84c3d3d30e9025`  
		Last Modified: Fri, 11 Dec 2020 02:10:15 GMT  
		Size: 25.8 MB (25769881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1864c3d7d0761fea04a3b1c6ac70ddd82c27b002138b03d3b89fa7be97abceb7`  
		Last Modified: Fri, 11 Dec 2020 16:54:07 GMT  
		Size: 11.6 MB (11608300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c58bddd16db870da684d956706ac7beb34a9a61a1637993de013305758cf280`  
		Last Modified: Fri, 11 Dec 2020 16:53:56 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724bc21f9dc167d33b39911e02e8ca816132ecbc3747d7f141b95a99de70f36`  
		Last Modified: Fri, 11 Dec 2020 16:56:27 GMT  
		Size: 21.6 MB (21637748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64df4fb893d9e4613191d83d82f0cd2b63f149bbfbfd363deec584d9644f4fa6`  
		Last Modified: Fri, 11 Dec 2020 16:56:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9c186313904d91e281f8e1831122fcccb8ab04d6412b825dc8f7459bcc551fb`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48af7885230e30ca6d0084380ed8e14750622deb4c94bf05befe441f7523835`  
		Last Modified: Fri, 11 Dec 2020 20:37:10 GMT  
		Size: 90.1 MB (90072579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129e6fa772a517fe09bce5f15f1cbb879f1d2d805028d61c1ed129f9dee551b5`  
		Last Modified: Fri, 11 Dec 2020 20:36:01 GMT  
		Size: 1.3 MB (1256645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa8c0a4dd492334ab9acc4b786f85e20ff8e91d8f994a47fd7c534f7fed84ec7`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a93c92ba03861a44a149916f51047a1ad284e34b83aeb90bdd4504238c1c1e2`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413a895834fed7a4125630a5fb75fecc0516bc14c6f5664d4d8882925b7760bf`  
		Last Modified: Fri, 11 Dec 2020 20:36:00 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfc83332192097ee67902d601513d8e50030905b3e5a007ac39165eb400dcad`  
		Last Modified: Fri, 11 Dec 2020 20:36:28 GMT  
		Size: 57.3 MB (57332039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a674d2c8b1e024562180c82c0597eba27e91c07e6c1c06c8903a540e1e0bdd3`  
		Last Modified: Fri, 11 Dec 2020 20:35:56 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:c3ea73afabbf5abdfb628b2873fb45815d1ef4c9b95b572a9a0015e6945eefe6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227408094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3e775c0e85890cfa750dae96663aaa8263ea772923a290760ce0de9b4248dbf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Nov 2020 23:23:06 GMT
ADD file:49cd8b08964980901349e1f3d6cb34abd8145dea6e6d9ab83502452281ac73ca in / 
# Tue, 17 Nov 2020 23:23:11 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 12:26:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 12:26:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 12:27:02 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 12:57:31 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 12:57:42 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 12:57:53 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 13:05:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 13:06:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:13 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 13:06:22 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 13:06:33 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 13:06:40 GMT
CMD ["irb"]
# Wed, 18 Nov 2020 22:56:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Nov 2020 23:16:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 23:23:58 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:24:12 GMT
ENV RAILS_ENV=production
# Wed, 18 Nov 2020 23:24:36 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Nov 2020 23:24:57 GMT
ENV HOME=/home/redmine
# Wed, 18 Nov 2020 23:25:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Nov 2020 23:26:01 GMT
ENV REDMINE_VERSION=4.1.1
# Wed, 18 Nov 2020 23:26:23 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Wed, 18 Nov 2020 23:27:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Nov 2020 23:36:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Nov 2020 23:37:11 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Nov 2020 23:37:14 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Wed, 18 Nov 2020 23:37:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Nov 2020 23:37:26 GMT
EXPOSE 3000
# Wed, 18 Nov 2020 23:37:31 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d79345c10f03543bff3982aedb35a18ba18626c0074014387ff5e1dc14474e2b`  
		Last Modified: Tue, 17 Nov 2020 23:32:54 GMT  
		Size: 30.5 MB (30531702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4324dba4d658f9cef4692709806bbbe7aa3f108b09489d3abadcdd00af26e816`  
		Last Modified: Wed, 18 Nov 2020 13:22:24 GMT  
		Size: 12.7 MB (12687856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f433a44b3fa921ad6d8b09e5619993f6812dfc023bf9c1ef38db8077916dfd3`  
		Last Modified: Wed, 18 Nov 2020 13:22:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6122ffb25e816545dedec8b707cbdea5f9f2b3c7c2a183f9ae488e46c605bb`  
		Last Modified: Wed, 18 Nov 2020 13:24:12 GMT  
		Size: 22.0 MB (21970057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab94d3b1f8973fd676af9a7da7255d83d3fdd27976823cbe4531093d01bb5f37`  
		Last Modified: Wed, 18 Nov 2020 13:24:09 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88001e8a986c6b8ebd7392d6ff4d5086ad80462ed5989827c839d3bfb4a01256`  
		Last Modified: Thu, 19 Nov 2020 00:19:46 GMT  
		Size: 1.8 KB (1761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89539658f86c698aa7459ac0cdc89685e83e9eabb35fda5f82bbafe99f899680`  
		Last Modified: Thu, 19 Nov 2020 00:20:07 GMT  
		Size: 100.3 MB (100343979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c3aa80defc7bbd76afb4c318dc49286936ba18a4e02c316b3fea450caf5727`  
		Last Modified: Thu, 19 Nov 2020 00:19:45 GMT  
		Size: 1.3 MB (1290133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46476067be42396f83b1e0b86411f0ebb193a82c64a8b44cfe7fce12fb68a1fc`  
		Last Modified: Thu, 19 Nov 2020 00:19:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec78f45da7bc16720440b5cfb4662425a82274373104d14c4834ed6185111460`  
		Last Modified: Thu, 19 Nov 2020 00:19:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9d4b0e36b50c79e6977f2e38415655d5822d25f34ecf61019611bf963cbddc`  
		Last Modified: Thu, 19 Nov 2020 00:19:40 GMT  
		Size: 2.7 MB (2739776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b6640a34082c8700a151ec61ee56a940ed83e971f04c234b49da0526ed48ee`  
		Last Modified: Thu, 19 Nov 2020 00:19:48 GMT  
		Size: 57.8 MB (57840073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6b1969b444ef8f9019b929408c483060e510efd0b8db7764de2391927bb84`  
		Last Modified: Thu, 19 Nov 2020 00:19:38 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:5afbbd3ee43a0df0b0e47bdce40339edfe52fdbb7e15f32b7c99dfe13e037d46
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210687321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72abefdbc79df1244ddf76dba03ecf53d87f03826bfee12474c75bdbb7158f8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 11 Dec 2020 02:12:11 GMT
ADD file:db86ce5a1665b6d8ac734c54ac249a811c58484f569b935b14772445962428aa in / 
# Fri, 11 Dec 2020 02:12:15 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 14:05:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 14:06:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 11 Dec 2020 14:06:00 GMT
ENV LANG=C.UTF-8
# Fri, 11 Dec 2020 14:39:41 GMT
ENV RUBY_MAJOR=2.6
# Fri, 11 Dec 2020 14:39:42 GMT
ENV RUBY_VERSION=2.6.6
# Fri, 11 Dec 2020 14:39:43 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Fri, 11 Dec 2020 14:44:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 11 Dec 2020 14:44:04 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 11 Dec 2020 14:44:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 11 Dec 2020 14:44:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 11 Dec 2020 14:44:07 GMT
CMD ["irb"]
# Fri, 11 Dec 2020 20:53:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 11 Dec 2020 20:53:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 20:54:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:54:20 GMT
ENV RAILS_ENV=production
# Fri, 11 Dec 2020 20:54:20 GMT
WORKDIR /usr/src/redmine
# Fri, 11 Dec 2020 20:54:21 GMT
ENV HOME=/home/redmine
# Fri, 11 Dec 2020 20:54:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 11 Dec 2020 20:54:22 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 11 Dec 2020 20:54:23 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 11 Dec 2020 20:54:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 11 Dec 2020 20:56:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 11 Dec 2020 20:56:29 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 11 Dec 2020 20:56:30 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 11 Dec 2020 20:56:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 20:56:30 GMT
EXPOSE 3000
# Fri, 11 Dec 2020 20:56:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f4cf10ca9f31aab0854647d7878dc4db838e93b892b843dde3db24f2e909a106`  
		Last Modified: Fri, 11 Dec 2020 02:17:07 GMT  
		Size: 25.7 MB (25713957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7319ab475e590b72d37f20d16fbbd64f355ac72137f788fba1242aae760a6732`  
		Last Modified: Fri, 11 Dec 2020 14:58:05 GMT  
		Size: 10.8 MB (10796868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81262b7893747b34acbfca1a00cfc0c68a997043db4e4b0ca7c54b95ef42d3`  
		Last Modified: Fri, 11 Dec 2020 14:58:03 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a2d6654f121a57b04ec9b4cd0328c79f7172e853a3c161296394c0a4eff283`  
		Last Modified: Fri, 11 Dec 2020 14:58:43 GMT  
		Size: 21.6 MB (21598273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554cb46f10b3fc8fe21d4894b92fd3a71978d0522f8f8483a20076965f766433`  
		Last Modified: Fri, 11 Dec 2020 14:58:41 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae3b3620abc202ccd0f4255185baf54839bf2b973b6e861c0d152a91932fdd1`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae562a30e04f377136d022a05202c0e304d868faf41178e4d93747f3dcf4e02`  
		Last Modified: Fri, 11 Dec 2020 21:00:52 GMT  
		Size: 90.8 MB (90834404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15cf9abfa62fe46d287e76c82e923fb635c8d76e9daa28663547ae13c6961fde`  
		Last Modified: Fri, 11 Dec 2020 21:00:38 GMT  
		Size: 1.4 MB (1355550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f42b8d97ca9305ed8fee32c1e42ddbe6147d0a1301c149b9465cf97819d559`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9486d1ae34f16fbe53268c5fa17157568a1679208eb74f8046aaf79b5c2ffd4`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a697087fccb24b639a6b93f6da510d3f6ce42ace5d9f9e64cd893108536edf5`  
		Last Modified: Fri, 11 Dec 2020 21:00:37 GMT  
		Size: 2.7 MB (2739767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59bda450facc4353a24f90ffab51457fb80d6fcd340d01cda5540157a21f1c0d`  
		Last Modified: Fri, 11 Dec 2020 21:00:43 GMT  
		Size: 57.6 MB (57643997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5351b41a29cb67f7763dbe84a9ee387f3667913e513212ba1d94d227034010`  
		Last Modified: Fri, 11 Dec 2020 21:00:36 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:passenger`

```console
$ docker pull redmine@sha256:5a4a19b0c0a63edf33e94bfe6c24edf734d7ce5045150a4d1210e334063d44ee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:b0480b6630ec7282e8aa09359a5a1700f668c38d8016438e9101ebeeb7c9252f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.5 MB (240467558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c41cc26645f19911933cc36cb8a8a7c5306e0d826c9bf6fffd44a7407b991fe5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Nov 2020 20:21:17 GMT
ADD file:d2abb0e4e7ac1773741f51f57d3a0b8ffc7907348842d773f8c341ba17f856d5 in / 
# Tue, 17 Nov 2020 20:21:17 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 15:21:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 15:21:23 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 18 Nov 2020 15:21:24 GMT
ENV LANG=C.UTF-8
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_MAJOR=2.6
# Wed, 18 Nov 2020 15:38:59 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 18 Nov 2020 15:39:00 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 18 Nov 2020 15:43:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 18 Nov 2020 15:43:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:02 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 18 Nov 2020 15:43:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 18 Nov 2020 15:43:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 18 Nov 2020 15:43:04 GMT
CMD ["irb"]
# Thu, 19 Nov 2020 05:47:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 19 Nov 2020 05:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 19 Nov 2020 05:47:41 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.19.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:47:41 GMT
ENV RAILS_ENV=production
# Thu, 19 Nov 2020 05:47:41 GMT
WORKDIR /usr/src/redmine
# Thu, 19 Nov 2020 05:47:41 GMT
ENV HOME=/home/redmine
# Thu, 19 Nov 2020 05:47:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 19 Nov 2020 05:47:43 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 19 Nov 2020 05:47:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 19 Nov 2020 05:49:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:20 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 19 Nov 2020 05:49:20 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 19 Nov 2020 05:49:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 19 Nov 2020 05:49:20 GMT
EXPOSE 3000
# Thu, 19 Nov 2020 05:49:20 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Thu, 19 Nov 2020 05:49:39 GMT
ENV PASSENGER_VERSION=6.0.7
# Thu, 19 Nov 2020 05:49:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Nov 2020 05:49:57 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Thu, 19 Nov 2020 05:49:57 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Thu, 19 Nov 2020 05:49:58 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:852e50cd189dfeb54d97680d9fa6bed21a6d7d18cfb56d6abfe2de9d7f173795`  
		Last Modified: Tue, 17 Nov 2020 20:27:25 GMT  
		Size: 27.1 MB (27105484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de4319615e27e1aaaadc89b43db39ea0e118f47eeecfa4c8b910ca2fd810653`  
		Last Modified: Wed, 18 Nov 2020 16:04:22 GMT  
		Size: 12.5 MB (12539406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:150eb06190d1ba56f7b998da25a140c21258bca436d33e2e77df679d77ab364a`  
		Last Modified: Wed, 18 Nov 2020 16:04:19 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9edff165f601a92c37be3301f41c28d3a5cd48ee0f4d6cad492a45cc81353e3`  
		Last Modified: Wed, 18 Nov 2020 16:05:17 GMT  
		Size: 21.5 MB (21450268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f31f949c4a723d3db9f21d3aa1e9523ca6942f6ddd32786d221e9a807bc3f94`  
		Last Modified: Wed, 18 Nov 2020 16:05:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51098d9bfbfa8457f002ed865d93565d3a434cb52cd4e87eb014e5e2c66f186b`  
		Last Modified: Thu, 19 Nov 2020 05:53:49 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ceaf427bdaab140ab3c03e03e397142d0f07a88cdd442cba1826fb438958620`  
		Last Modified: Thu, 19 Nov 2020 05:54:07 GMT  
		Size: 93.1 MB (93104105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6332f2c839082a3548a096495ec34f3bc551c78437af681d10ce1edfb94ee264`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 1.4 MB (1369330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f061509154252c143a6b5680bb73dfa52909d4a8b300d809dd0e1ac53da1f12d`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409c9bd29355b0269a77c26db749c2549cfbfca66ffd7dd6b1f04610b2623019`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a53142f7c27fe4f4a12dfef13f9a10f4613b03ad98babf32482a6c25ff52f13`  
		Last Modified: Thu, 19 Nov 2020 05:53:48 GMT  
		Size: 2.7 MB (2739478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee5b56b6eec16ce4e488515ba41448ea784f5bf5a8fc75c36ce898c6b5a46bb`  
		Last Modified: Thu, 19 Nov 2020 05:53:55 GMT  
		Size: 57.3 MB (57280977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98c5b8b7f7c3b21ee1b9ea7cbae6a70f0a9cfe48646a3c04077b0fe8c8c8d64`  
		Last Modified: Thu, 19 Nov 2020 05:53:47 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe718b527ed48d5acde8b6e369a9906a5742eecf6fb634c03de4658ce359980`  
		Last Modified: Thu, 19 Nov 2020 05:54:18 GMT  
		Size: 20.0 MB (19952149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd401b8b07edacf0f7e26dfa17e1e02a1ff174e3b43f0dacc172b1bcdb18cf6`  
		Last Modified: Thu, 19 Nov 2020 05:54:16 GMT  
		Size: 4.9 MB (4921957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
