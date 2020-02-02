<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `redmine`

-	[`redmine:3`](#redmine3)
-	[`redmine:3.4`](#redmine34)
-	[`redmine:3.4.13`](#redmine3413)
-	[`redmine:3.4.13-alpine`](#redmine3413-alpine)
-	[`redmine:3.4.13-passenger`](#redmine3413-passenger)
-	[`redmine:3.4-alpine`](#redmine34-alpine)
-	[`redmine:3.4-passenger`](#redmine34-passenger)
-	[`redmine:3-alpine`](#redmine3-alpine)
-	[`redmine:3-passenger`](#redmine3-passenger)
-	[`redmine:4`](#redmine4)
-	[`redmine:4.0`](#redmine40)
-	[`redmine:4.0.6`](#redmine406)
-	[`redmine:4.0.6-alpine`](#redmine406-alpine)
-	[`redmine:4.0.6-passenger`](#redmine406-passenger)
-	[`redmine:4.0-alpine`](#redmine40-alpine)
-	[`redmine:4.0-passenger`](#redmine40-passenger)
-	[`redmine:4.1`](#redmine41)
-	[`redmine:4.1.0`](#redmine410)
-	[`redmine:4.1.0-alpine`](#redmine410-alpine)
-	[`redmine:4.1.0-passenger`](#redmine410-passenger)
-	[`redmine:4.1-alpine`](#redmine41-alpine)
-	[`redmine:4.1-passenger`](#redmine41-passenger)
-	[`redmine:4-alpine`](#redmine4-alpine)
-	[`redmine:4-passenger`](#redmine4-passenger)
-	[`redmine:alpine`](#redminealpine)
-	[`redmine:latest`](#redminelatest)
-	[`redmine:passenger`](#redminepassenger)

## `redmine:3`

```console
$ docker pull redmine@sha256:f6559d4aa45c11d241acf5e5c2dd317520e71579a63f85fa89919d57765798eb
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

### `redmine:3` - linux; amd64

```console
$ docker pull redmine@sha256:4beb787321e64d4f9ee0864d211279b3c01ee99e61259529c75f340d012be97d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207502345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91750691100784163b27ba361763857c9b3db45acd8a73cd890fdd3b2becd79`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 15:05:12 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 15:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:09:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:21:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:21:30 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:53:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:53:14 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:53:14 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:53:14 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:53:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 02:53:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:12:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:10 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:12:10 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:12:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:12:11 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:12:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aac5e62bfbec87ca600e8d9ee16832e53efd48c6a1ad8f02c923545e2d32fc4`  
		Last Modified: Sat, 28 Dec 2019 15:19:25 GMT  
		Size: 22.0 MB (22006052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fd0e5c830a620f7adbe8dbf517f558bd629236c05e30a81562e627d41af933`  
		Last Modified: Tue, 07 Jan 2020 02:23:51 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda27aa91ecfc255aa8888f23781a4fd6c446c38b13fcf945d933d697868399d`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3047b43ab05eab0353c1e221caf7d98300915f73d638eeb5fc32c8c542f9f979`  
		Last Modified: Tue, 07 Jan 2020 03:00:49 GMT  
		Size: 80.2 MB (80161214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d379f55b07e46100b9811c56dc34b9488eeb5029cd6d5b5aa1d0d952db4585f4`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.3 MB (1296456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d615b50742767a48c5a2f96cb4848af939353414d875d60e5bfd09828138869`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64db6c7eb6d20bd9906e4c0a451b94d1f042f1e8724e096a58608af75e4570`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26258bfd510bef8a8d430c8304327ee816f16c1d11e96b4e9d3127b00eb7611a`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 2.5 MB (2463473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27b56d37a6fe981e5fa2e124b4c81a2b197c46c74beddca441e70d12b3c0d4`  
		Last Modified: Sat, 25 Jan 2020 03:16:42 GMT  
		Size: 61.9 MB (61938710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a824ae4c58c52b7a5ff3051b2a8f0239a28542e884ed3c3b341d33b56aa4d`  
		Last Modified: Sat, 25 Jan 2020 03:16:33 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3` - linux; arm variant v5

```console
$ docker pull redmine@sha256:c94aeafc4839953ffc6f1d091d0be07f4b08b8798aac09ad6d5553bccf4919f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.3 MB (197297445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22cd43b3d587718da99aba51d70195446f839e60ec885836249565df5fa1e5f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:53:06 GMT
ENV RUBY_MAJOR=2.4
# Sun, 02 Feb 2020 02:53:07 GMT
ENV RUBY_VERSION=2.4.9
# Sun, 02 Feb 2020 02:53:07 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sun, 02 Feb 2020 02:53:08 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sun, 02 Feb 2020 03:00:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 03:00:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 03:00:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 03:00:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 03:00:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 03:00:19 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:58:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 10:00:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 10:00:16 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 10:00:17 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 10:00:18 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 10:00:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 10:00:24 GMT
ENV REDMINE_VERSION=3.4.13
# Sun, 02 Feb 2020 10:00:26 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Sun, 02 Feb 2020 10:00:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 10:06:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 10:06:54 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 10:06:55 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 10:06:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 10:06:56 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 10:06:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d66a1f914bdc48f10a9fb7fa826de1fc4d51127360bfb635de92800427c2c`  
		Last Modified: Sun, 02 Feb 2020 03:18:21 GMT  
		Size: 21.3 MB (21337996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59db49767202ac506ef64e9ad4e78c2222a92d585fc752c47494f69c8d66c40`  
		Last Modified: Sun, 02 Feb 2020 03:18:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb41ba2542818a91d69186164d2baa8245ac6afcfb94f1fcb0d6f6e512d1065`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd4d2b24e257beb61f33391e5e90e9967dc45a757e66afcf682f086ae1db02b`  
		Last Modified: Sun, 02 Feb 2020 10:09:15 GMT  
		Size: 76.0 MB (76036604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774123ad6534a0960d229fc9293ab82687ff0eb673ef39fe99574fdb43fc0300`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 1.3 MB (1254237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba04482a10d8e7ec8a828448873ef5521cb469231897b4757a6e3acb3772cce`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a493edaaf61e6e3d79bca713573cd3eada2ce4a0149ce264e8c82f1a087b407`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943138c7822bb22264d257ee437bf08d764d088aca0a6279ba23f62232241da4`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 2.5 MB (2463871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfefd54730a9b78dff4a21cc9482ecaa0526bbced5ccd32add28fead591f587`  
		Last Modified: Sun, 02 Feb 2020 10:08:55 GMT  
		Size: 61.0 MB (61044490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bbf1e5c954dbffe8437807f7327f66456bb1c60539fbea8fd822d16dcdfb2f`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3` - linux; arm variant v7

```console
$ docker pull redmine@sha256:4c39f48cac800b36598706c649b989d6f5f9205f39ac72b306dacfe85dd38d43
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.8 MB (190775448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3e252e5d8c5e730460892f1a9f42514c647123d5101525d0d055cc902bf803`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:51:26 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 21:51:27 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 21:51:29 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 21:51:29 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 21:57:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:57:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:15:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:15:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:15:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:15:41 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:52:03 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:52:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:53:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:53:17 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:53:18 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:53:18 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:53:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:53:20 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:53:21 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:53:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:23:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:23:58 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:23:59 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:24:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:24:02 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:24:03 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8baf5eda0f1fcf9d63cd20bab0bf046b7fdf99276524015b69f17a54f2d4e5bd`  
		Last Modified: Sat, 28 Dec 2019 22:15:15 GMT  
		Size: 21.3 MB (21261197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799af941ea6a75fd00ff583cd811459d9aa1ebf9bbfe53c690c886f22090c7b`  
		Last Modified: Tue, 07 Jan 2020 03:19:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c215c6dca6c1749986f1b9558c12d97e3b6165c10c6adcd3dcab432b34a1afa`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8f67953faffb1c4e8fffb1caa9217a25357829e1bbc3542405026627994e64`  
		Last Modified: Tue, 07 Jan 2020 04:00:42 GMT  
		Size: 72.4 MB (72370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99638607df68e0caa80b678073b2bc1ab6bed1e6e765fbd58b4988e0a71017b4`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 1.2 MB (1243561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78977b4c3dfedf84fb120dbfa4e54e630246641aa0d57ede77b71d350a609774`  
		Last Modified: Tue, 07 Jan 2020 04:00:18 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0a66cd3e3ab71fca594f8aff62bbba677266975b1a11f481c8ae2965e5ca51`  
		Last Modified: Tue, 07 Jan 2020 04:00:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b76411581c7df4e2b0a02012d441a45291a6285744c35eb2744a942f54b7560`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 2.5 MB (2463868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c00cc8eff10d5bfb13c4eeadb6504d82f498ec7dd94327a00fa9bbbc5c109f`  
		Last Modified: Sat, 25 Jan 2020 02:25:43 GMT  
		Size: 60.9 MB (60884981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec3548c1f4fb71a189745695038f0338727e1807ba1901b255f362827eddc6`  
		Last Modified: Sat, 25 Jan 2020 02:25:30 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:957f9b274b869bd00c1179677cab1163d933e1c615fad331467dab582aed0c17
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203347558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5777787ec04c96709988514a7ead13444e1289631fd8c8e05fb49a69ecae4411`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 23:03:38 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 23:03:39 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 23:03:40 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 23:03:41 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 23:09:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 23:09:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:43:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:43:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:43:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:43:07 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:22:13 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:23:40 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:23:40 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:23:41 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:23:41 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:23:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:23:44 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:23:44 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:23:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:52:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:52:45 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:52:46 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:52:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:52:48 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:52:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5cb0a3803f06119e2e010bac2f8756f225c7aafdb2af8de4eaa2aa2ab7b54b`  
		Last Modified: Sat, 28 Dec 2019 23:25:14 GMT  
		Size: 21.9 MB (21879231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c771ed92dd7985dfe7f891a2a1dcd20a4924b1c897760f5a84805f5996ecfbe4`  
		Last Modified: Tue, 07 Jan 2020 02:46:44 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f143af2012a522002d49c8c5e35ad2f785ea557182fc369a45b1f83f18ed178`  
		Last Modified: Tue, 07 Jan 2020 03:32:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae138bc962325d1988fa72ea2f6ee74ee8549c9a467873a8624a810371df69e`  
		Last Modified: Tue, 07 Jan 2020 03:32:34 GMT  
		Size: 78.8 MB (78782045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8add249b39c3d8ec3f40de3ca3f3fa8c28484688f18f819e44be255a154b9f6`  
		Last Modified: Tue, 07 Jan 2020 03:32:12 GMT  
		Size: 1.2 MB (1228475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7b17f7c48aaa1d7dffac2d6c94b30b55b46051c58d9102d265a3e694d7a736`  
		Last Modified: Tue, 07 Jan 2020 03:32:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e80fe221a061826ce2e5104101ae09f094f093004bc6b7735d85ef712d7781`  
		Last Modified: Tue, 07 Jan 2020 03:32:09 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5178963f7abb7582e65919deb0614e9014cb4d013df72194bb2d91201ceaf8`  
		Last Modified: Tue, 07 Jan 2020 03:32:10 GMT  
		Size: 2.5 MB (2463878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6ead016d43f4981848676dd1d46cd08e0cfc3bf743b2c9d06df8415ad3931e`  
		Last Modified: Sat, 25 Jan 2020 02:54:27 GMT  
		Size: 61.9 MB (61894027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ff648cf1b1bae072e3a39161c9356ff9fd977dd469225a5c5ef215033c04ad`  
		Last Modified: Sat, 25 Jan 2020 02:54:14 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3` - linux; 386

```console
$ docker pull redmine@sha256:9d20bae3dc8a25376db18c0942653aa050d19617f8ed641a89a24852b4699189
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212966720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48cd45f82afe394a48d66b2244501078593165b9b5070f3016083c535401a04e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 16:24:30 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 16:30:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 16:30:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:40:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:40:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:40:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:40:07 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:07:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:08:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:08:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:08:12 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:08:12 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:08:13 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:08:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:08:14 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:08:14 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:08:17 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:55:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:55:06 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:55:07 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:55:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:55:07 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:55:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c021c8bfb2bb7e4f5caefd65e47f63eebb61502811966d3adc3f94ed9971017`  
		Last Modified: Sat, 28 Dec 2019 16:46:27 GMT  
		Size: 21.5 MB (21545961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33387c53c9ce779731032ff2f975ff7bbf0a16cd0551530997c664fec29ffb9a`  
		Last Modified: Tue, 07 Jan 2020 02:42:33 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdbef8b208533e2164c865470a9f1eb7ff708ecf888e79a7a884f20f5d93a45`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab5be34e7c4dc9dacc59a617b7f06eb1eb3ad229c4eb52da844415056b5f70`  
		Last Modified: Tue, 07 Jan 2020 03:12:17 GMT  
		Size: 81.6 MB (81574487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902840c7a384de1512dc1b47ecb4131fd83059a1ec3573014a974cecc6de24dd`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 1.3 MB (1261121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1807d33df93b1be2b8457093bccf02a94b6497f02105ec86c2408ac7cd8feccf`  
		Last Modified: Tue, 07 Jan 2020 03:11:54 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2991d075bf2bd2e85f753f498185dd38bfec5885dc0da5ad01c74c1e0d34ee1e`  
		Last Modified: Tue, 07 Jan 2020 03:11:54 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7f65bcaf193982883ff7c676cf3acd30476b7bf836c6fa410fd0bc7b7f645`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 2.5 MB (2463470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9c6ceadaecf4398689a031439e3820eaa178b90b78d55176bbe3bfb6ba6e9`  
		Last Modified: Sat, 25 Jan 2020 01:56:17 GMT  
		Size: 61.2 MB (61164251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef61387ac2248fbdd6ba623bb119faa53406da27e4e5a8b8de36c60c0124fdb`  
		Last Modified: Sat, 25 Jan 2020 01:56:07 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3` - linux; ppc64le

```console
$ docker pull redmine@sha256:b92641f85841d118e8ce915e66fa19f48099e1c4729c3642a1eb7aed6c933b51
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218738140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f42e869aa800a67426ec040dda456b59adf3e38fd56451ba30a4f5961d05d77`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 05:07:30 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 05:07:32 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 05:07:33 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 05:07:35 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 05:16:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 05:17:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:22:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:22:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:22:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:22:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:16:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:18:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:19:36 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:19:38 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:19:41 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:19:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:19:47 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:19:49 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:19:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:28:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:28:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:28:22 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:28:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:28:29 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:28:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0831251b6fc73f4a098076145b4eedff1f2043b17e07a22a640aac457b19ffab`  
		Last Modified: Sat, 28 Dec 2019 05:31:10 GMT  
		Size: 22.5 MB (22518813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f17dc85665a35195e0378cddb30197da86e7d824c5330302c8b74d2dc7bd254`  
		Last Modified: Tue, 07 Jan 2020 02:30:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ff712870942f8f279111b569dd620512940f713de5a18702909c666b82283d`  
		Last Modified: Tue, 07 Jan 2020 03:31:00 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815827d563f9f23bf0c3e35c713e3b20f90ccdb1d3d9bc9411efe6507d2c229f`  
		Last Modified: Tue, 07 Jan 2020 03:31:24 GMT  
		Size: 86.8 MB (86837755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f077a99d3a54521280a74467d75d74dc098e16cc5401d15524c42adce16819a7`  
		Last Modified: Tue, 07 Jan 2020 03:31:00 GMT  
		Size: 1.2 MB (1218174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0de3d5e5366fabf9fdc6c1f4eb2c2f92afde26d760575faf726ff770be38799`  
		Last Modified: Tue, 07 Jan 2020 03:30:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374d354d8b463223158de295e4a199502ea29b7f1b51c490c7cdd3e01e560cd7`  
		Last Modified: Tue, 07 Jan 2020 03:30:56 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d1fd1f3723fb7145a7656f58f20ae8c7267107e777d38e479d92163e07abd`  
		Last Modified: Tue, 07 Jan 2020 03:30:57 GMT  
		Size: 2.5 MB (2463873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c41537c282aa3c5005eed86f46ed7e478e4d7f43cb38d67c0938a23d0b58f64`  
		Last Modified: Sat, 25 Jan 2020 03:30:16 GMT  
		Size: 62.5 MB (62488597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e8b55367dfb30b9a185fd4565e93a20c53fa0c0a1aa7e4022133c0aab87f8`  
		Last Modified: Sat, 25 Jan 2020 03:30:05 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3` - linux; s390x

```console
$ docker pull redmine@sha256:2370a4642f404adbcdd7c37975e2aa8a4a9c399593cf21b831a7753bf31f1fd2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202577034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:889f0b16b19300fc0a24e1c00746a0ab8ffe37e3001f3e859a8832c7e724ffeb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:48:48 GMT
ENV RUBY_MAJOR=2.4
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 01 Feb 2020 22:51:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:51:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:51:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:51:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:51:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:51:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:31:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:32:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:32:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:32:25 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:32:25 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:32:25 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:32:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:32:26 GMT
ENV REDMINE_VERSION=3.4.13
# Sun, 02 Feb 2020 03:32:26 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Sun, 02 Feb 2020 03:32:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:34:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:34:39 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:34:39 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:34:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:34:39 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:34:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace099387f5254edf276126e046611f26609fd7b03c6eccab25882e8492ab41f`  
		Last Modified: Sat, 01 Feb 2020 22:58:36 GMT  
		Size: 22.2 MB (22151592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b170fa9fa8c788d38c6d6505a94b57d409b33565fd70320c01ce2c1a22977c6`  
		Last Modified: Sat, 01 Feb 2020 22:58:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f8b559eb775e7ef2268ad21235635a36ac961841bf8d21ff310f414a71c80e`  
		Last Modified: Sun, 02 Feb 2020 03:36:10 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeaef2a78b559791011534abf0ee2a723b138776372b00019af6f1bcf1b59da`  
		Last Modified: Sun, 02 Feb 2020 03:36:21 GMT  
		Size: 77.9 MB (77940591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf387e3c6ea73ebb6cd13db382724dff9771329e421c8c4ed454fe11927aea0e`  
		Last Modified: Sun, 02 Feb 2020 03:36:09 GMT  
		Size: 1.3 MB (1283198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662f8c8a715db4b4d679682f19697f18f3d11ce144ca00a77c43d87f8251198e`  
		Last Modified: Sun, 02 Feb 2020 03:36:08 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58d75b229dcd884bd3aa4e230e09890af1beccdf1e73b531fdfef09787a956f`  
		Last Modified: Sun, 02 Feb 2020 03:36:07 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e04af6349cfcff77309336b34350e8fd67956803fe9408f9ff99f121eb6f15`  
		Last Modified: Sun, 02 Feb 2020 03:36:09 GMT  
		Size: 2.5 MB (2463866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babe457f5e43177a09c215741217f93c7a724ca2a67b1bbd2b2ae33bc8e96108`  
		Last Modified: Sun, 02 Feb 2020 03:36:29 GMT  
		Size: 62.2 MB (62231901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9a86c32d5039b929295c3d0162a1177253345f3654fb1e75ddba4477957176`  
		Last Modified: Sun, 02 Feb 2020 03:36:39 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:3.4`

```console
$ docker pull redmine@sha256:f6559d4aa45c11d241acf5e5c2dd317520e71579a63f85fa89919d57765798eb
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

### `redmine:3.4` - linux; amd64

```console
$ docker pull redmine@sha256:4beb787321e64d4f9ee0864d211279b3c01ee99e61259529c75f340d012be97d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207502345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91750691100784163b27ba361763857c9b3db45acd8a73cd890fdd3b2becd79`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 15:05:12 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 15:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:09:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:21:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:21:30 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:53:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:53:14 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:53:14 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:53:14 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:53:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 02:53:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:12:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:10 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:12:10 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:12:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:12:11 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:12:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aac5e62bfbec87ca600e8d9ee16832e53efd48c6a1ad8f02c923545e2d32fc4`  
		Last Modified: Sat, 28 Dec 2019 15:19:25 GMT  
		Size: 22.0 MB (22006052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fd0e5c830a620f7adbe8dbf517f558bd629236c05e30a81562e627d41af933`  
		Last Modified: Tue, 07 Jan 2020 02:23:51 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda27aa91ecfc255aa8888f23781a4fd6c446c38b13fcf945d933d697868399d`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3047b43ab05eab0353c1e221caf7d98300915f73d638eeb5fc32c8c542f9f979`  
		Last Modified: Tue, 07 Jan 2020 03:00:49 GMT  
		Size: 80.2 MB (80161214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d379f55b07e46100b9811c56dc34b9488eeb5029cd6d5b5aa1d0d952db4585f4`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.3 MB (1296456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d615b50742767a48c5a2f96cb4848af939353414d875d60e5bfd09828138869`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64db6c7eb6d20bd9906e4c0a451b94d1f042f1e8724e096a58608af75e4570`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26258bfd510bef8a8d430c8304327ee816f16c1d11e96b4e9d3127b00eb7611a`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 2.5 MB (2463473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27b56d37a6fe981e5fa2e124b4c81a2b197c46c74beddca441e70d12b3c0d4`  
		Last Modified: Sat, 25 Jan 2020 03:16:42 GMT  
		Size: 61.9 MB (61938710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a824ae4c58c52b7a5ff3051b2a8f0239a28542e884ed3c3b341d33b56aa4d`  
		Last Modified: Sat, 25 Jan 2020 03:16:33 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:c94aeafc4839953ffc6f1d091d0be07f4b08b8798aac09ad6d5553bccf4919f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.3 MB (197297445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22cd43b3d587718da99aba51d70195446f839e60ec885836249565df5fa1e5f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:53:06 GMT
ENV RUBY_MAJOR=2.4
# Sun, 02 Feb 2020 02:53:07 GMT
ENV RUBY_VERSION=2.4.9
# Sun, 02 Feb 2020 02:53:07 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sun, 02 Feb 2020 02:53:08 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sun, 02 Feb 2020 03:00:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 03:00:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 03:00:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 03:00:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 03:00:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 03:00:19 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:58:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 10:00:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 10:00:16 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 10:00:17 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 10:00:18 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 10:00:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 10:00:24 GMT
ENV REDMINE_VERSION=3.4.13
# Sun, 02 Feb 2020 10:00:26 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Sun, 02 Feb 2020 10:00:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 10:06:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 10:06:54 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 10:06:55 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 10:06:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 10:06:56 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 10:06:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d66a1f914bdc48f10a9fb7fa826de1fc4d51127360bfb635de92800427c2c`  
		Last Modified: Sun, 02 Feb 2020 03:18:21 GMT  
		Size: 21.3 MB (21337996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59db49767202ac506ef64e9ad4e78c2222a92d585fc752c47494f69c8d66c40`  
		Last Modified: Sun, 02 Feb 2020 03:18:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb41ba2542818a91d69186164d2baa8245ac6afcfb94f1fcb0d6f6e512d1065`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd4d2b24e257beb61f33391e5e90e9967dc45a757e66afcf682f086ae1db02b`  
		Last Modified: Sun, 02 Feb 2020 10:09:15 GMT  
		Size: 76.0 MB (76036604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774123ad6534a0960d229fc9293ab82687ff0eb673ef39fe99574fdb43fc0300`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 1.3 MB (1254237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba04482a10d8e7ec8a828448873ef5521cb469231897b4757a6e3acb3772cce`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a493edaaf61e6e3d79bca713573cd3eada2ce4a0149ce264e8c82f1a087b407`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943138c7822bb22264d257ee437bf08d764d088aca0a6279ba23f62232241da4`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 2.5 MB (2463871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfefd54730a9b78dff4a21cc9482ecaa0526bbced5ccd32add28fead591f587`  
		Last Modified: Sun, 02 Feb 2020 10:08:55 GMT  
		Size: 61.0 MB (61044490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bbf1e5c954dbffe8437807f7327f66456bb1c60539fbea8fd822d16dcdfb2f`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:4c39f48cac800b36598706c649b989d6f5f9205f39ac72b306dacfe85dd38d43
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.8 MB (190775448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3e252e5d8c5e730460892f1a9f42514c647123d5101525d0d055cc902bf803`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:51:26 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 21:51:27 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 21:51:29 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 21:51:29 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 21:57:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:57:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:15:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:15:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:15:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:15:41 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:52:03 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:52:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:53:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:53:17 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:53:18 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:53:18 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:53:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:53:20 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:53:21 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:53:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:23:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:23:58 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:23:59 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:24:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:24:02 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:24:03 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8baf5eda0f1fcf9d63cd20bab0bf046b7fdf99276524015b69f17a54f2d4e5bd`  
		Last Modified: Sat, 28 Dec 2019 22:15:15 GMT  
		Size: 21.3 MB (21261197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799af941ea6a75fd00ff583cd811459d9aa1ebf9bbfe53c690c886f22090c7b`  
		Last Modified: Tue, 07 Jan 2020 03:19:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c215c6dca6c1749986f1b9558c12d97e3b6165c10c6adcd3dcab432b34a1afa`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8f67953faffb1c4e8fffb1caa9217a25357829e1bbc3542405026627994e64`  
		Last Modified: Tue, 07 Jan 2020 04:00:42 GMT  
		Size: 72.4 MB (72370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99638607df68e0caa80b678073b2bc1ab6bed1e6e765fbd58b4988e0a71017b4`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 1.2 MB (1243561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78977b4c3dfedf84fb120dbfa4e54e630246641aa0d57ede77b71d350a609774`  
		Last Modified: Tue, 07 Jan 2020 04:00:18 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0a66cd3e3ab71fca594f8aff62bbba677266975b1a11f481c8ae2965e5ca51`  
		Last Modified: Tue, 07 Jan 2020 04:00:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b76411581c7df4e2b0a02012d441a45291a6285744c35eb2744a942f54b7560`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 2.5 MB (2463868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c00cc8eff10d5bfb13c4eeadb6504d82f498ec7dd94327a00fa9bbbc5c109f`  
		Last Modified: Sat, 25 Jan 2020 02:25:43 GMT  
		Size: 60.9 MB (60884981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec3548c1f4fb71a189745695038f0338727e1807ba1901b255f362827eddc6`  
		Last Modified: Sat, 25 Jan 2020 02:25:30 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:957f9b274b869bd00c1179677cab1163d933e1c615fad331467dab582aed0c17
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203347558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5777787ec04c96709988514a7ead13444e1289631fd8c8e05fb49a69ecae4411`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 23:03:38 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 23:03:39 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 23:03:40 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 23:03:41 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 23:09:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 23:09:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:43:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:43:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:43:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:43:07 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:22:13 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:23:40 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:23:40 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:23:41 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:23:41 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:23:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:23:44 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:23:44 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:23:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:52:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:52:45 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:52:46 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:52:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:52:48 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:52:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5cb0a3803f06119e2e010bac2f8756f225c7aafdb2af8de4eaa2aa2ab7b54b`  
		Last Modified: Sat, 28 Dec 2019 23:25:14 GMT  
		Size: 21.9 MB (21879231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c771ed92dd7985dfe7f891a2a1dcd20a4924b1c897760f5a84805f5996ecfbe4`  
		Last Modified: Tue, 07 Jan 2020 02:46:44 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f143af2012a522002d49c8c5e35ad2f785ea557182fc369a45b1f83f18ed178`  
		Last Modified: Tue, 07 Jan 2020 03:32:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae138bc962325d1988fa72ea2f6ee74ee8549c9a467873a8624a810371df69e`  
		Last Modified: Tue, 07 Jan 2020 03:32:34 GMT  
		Size: 78.8 MB (78782045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8add249b39c3d8ec3f40de3ca3f3fa8c28484688f18f819e44be255a154b9f6`  
		Last Modified: Tue, 07 Jan 2020 03:32:12 GMT  
		Size: 1.2 MB (1228475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7b17f7c48aaa1d7dffac2d6c94b30b55b46051c58d9102d265a3e694d7a736`  
		Last Modified: Tue, 07 Jan 2020 03:32:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e80fe221a061826ce2e5104101ae09f094f093004bc6b7735d85ef712d7781`  
		Last Modified: Tue, 07 Jan 2020 03:32:09 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5178963f7abb7582e65919deb0614e9014cb4d013df72194bb2d91201ceaf8`  
		Last Modified: Tue, 07 Jan 2020 03:32:10 GMT  
		Size: 2.5 MB (2463878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6ead016d43f4981848676dd1d46cd08e0cfc3bf743b2c9d06df8415ad3931e`  
		Last Modified: Sat, 25 Jan 2020 02:54:27 GMT  
		Size: 61.9 MB (61894027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ff648cf1b1bae072e3a39161c9356ff9fd977dd469225a5c5ef215033c04ad`  
		Last Modified: Sat, 25 Jan 2020 02:54:14 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4` - linux; 386

```console
$ docker pull redmine@sha256:9d20bae3dc8a25376db18c0942653aa050d19617f8ed641a89a24852b4699189
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212966720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48cd45f82afe394a48d66b2244501078593165b9b5070f3016083c535401a04e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 16:24:30 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 16:30:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 16:30:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:40:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:40:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:40:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:40:07 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:07:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:08:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:08:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:08:12 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:08:12 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:08:13 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:08:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:08:14 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:08:14 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:08:17 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:55:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:55:06 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:55:07 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:55:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:55:07 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:55:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c021c8bfb2bb7e4f5caefd65e47f63eebb61502811966d3adc3f94ed9971017`  
		Last Modified: Sat, 28 Dec 2019 16:46:27 GMT  
		Size: 21.5 MB (21545961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33387c53c9ce779731032ff2f975ff7bbf0a16cd0551530997c664fec29ffb9a`  
		Last Modified: Tue, 07 Jan 2020 02:42:33 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdbef8b208533e2164c865470a9f1eb7ff708ecf888e79a7a884f20f5d93a45`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab5be34e7c4dc9dacc59a617b7f06eb1eb3ad229c4eb52da844415056b5f70`  
		Last Modified: Tue, 07 Jan 2020 03:12:17 GMT  
		Size: 81.6 MB (81574487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902840c7a384de1512dc1b47ecb4131fd83059a1ec3573014a974cecc6de24dd`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 1.3 MB (1261121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1807d33df93b1be2b8457093bccf02a94b6497f02105ec86c2408ac7cd8feccf`  
		Last Modified: Tue, 07 Jan 2020 03:11:54 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2991d075bf2bd2e85f753f498185dd38bfec5885dc0da5ad01c74c1e0d34ee1e`  
		Last Modified: Tue, 07 Jan 2020 03:11:54 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7f65bcaf193982883ff7c676cf3acd30476b7bf836c6fa410fd0bc7b7f645`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 2.5 MB (2463470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9c6ceadaecf4398689a031439e3820eaa178b90b78d55176bbe3bfb6ba6e9`  
		Last Modified: Sat, 25 Jan 2020 01:56:17 GMT  
		Size: 61.2 MB (61164251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef61387ac2248fbdd6ba623bb119faa53406da27e4e5a8b8de36c60c0124fdb`  
		Last Modified: Sat, 25 Jan 2020 01:56:07 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4` - linux; ppc64le

```console
$ docker pull redmine@sha256:b92641f85841d118e8ce915e66fa19f48099e1c4729c3642a1eb7aed6c933b51
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218738140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f42e869aa800a67426ec040dda456b59adf3e38fd56451ba30a4f5961d05d77`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 05:07:30 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 05:07:32 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 05:07:33 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 05:07:35 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 05:16:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 05:17:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:22:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:22:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:22:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:22:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:16:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:18:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:19:36 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:19:38 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:19:41 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:19:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:19:47 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:19:49 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:19:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:28:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:28:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:28:22 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:28:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:28:29 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:28:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0831251b6fc73f4a098076145b4eedff1f2043b17e07a22a640aac457b19ffab`  
		Last Modified: Sat, 28 Dec 2019 05:31:10 GMT  
		Size: 22.5 MB (22518813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f17dc85665a35195e0378cddb30197da86e7d824c5330302c8b74d2dc7bd254`  
		Last Modified: Tue, 07 Jan 2020 02:30:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ff712870942f8f279111b569dd620512940f713de5a18702909c666b82283d`  
		Last Modified: Tue, 07 Jan 2020 03:31:00 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815827d563f9f23bf0c3e35c713e3b20f90ccdb1d3d9bc9411efe6507d2c229f`  
		Last Modified: Tue, 07 Jan 2020 03:31:24 GMT  
		Size: 86.8 MB (86837755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f077a99d3a54521280a74467d75d74dc098e16cc5401d15524c42adce16819a7`  
		Last Modified: Tue, 07 Jan 2020 03:31:00 GMT  
		Size: 1.2 MB (1218174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0de3d5e5366fabf9fdc6c1f4eb2c2f92afde26d760575faf726ff770be38799`  
		Last Modified: Tue, 07 Jan 2020 03:30:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374d354d8b463223158de295e4a199502ea29b7f1b51c490c7cdd3e01e560cd7`  
		Last Modified: Tue, 07 Jan 2020 03:30:56 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d1fd1f3723fb7145a7656f58f20ae8c7267107e777d38e479d92163e07abd`  
		Last Modified: Tue, 07 Jan 2020 03:30:57 GMT  
		Size: 2.5 MB (2463873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c41537c282aa3c5005eed86f46ed7e478e4d7f43cb38d67c0938a23d0b58f64`  
		Last Modified: Sat, 25 Jan 2020 03:30:16 GMT  
		Size: 62.5 MB (62488597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e8b55367dfb30b9a185fd4565e93a20c53fa0c0a1aa7e4022133c0aab87f8`  
		Last Modified: Sat, 25 Jan 2020 03:30:05 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4` - linux; s390x

```console
$ docker pull redmine@sha256:2370a4642f404adbcdd7c37975e2aa8a4a9c399593cf21b831a7753bf31f1fd2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202577034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:889f0b16b19300fc0a24e1c00746a0ab8ffe37e3001f3e859a8832c7e724ffeb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:48:48 GMT
ENV RUBY_MAJOR=2.4
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 01 Feb 2020 22:51:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:51:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:51:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:51:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:51:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:51:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:31:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:32:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:32:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:32:25 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:32:25 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:32:25 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:32:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:32:26 GMT
ENV REDMINE_VERSION=3.4.13
# Sun, 02 Feb 2020 03:32:26 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Sun, 02 Feb 2020 03:32:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:34:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:34:39 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:34:39 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:34:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:34:39 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:34:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace099387f5254edf276126e046611f26609fd7b03c6eccab25882e8492ab41f`  
		Last Modified: Sat, 01 Feb 2020 22:58:36 GMT  
		Size: 22.2 MB (22151592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b170fa9fa8c788d38c6d6505a94b57d409b33565fd70320c01ce2c1a22977c6`  
		Last Modified: Sat, 01 Feb 2020 22:58:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f8b559eb775e7ef2268ad21235635a36ac961841bf8d21ff310f414a71c80e`  
		Last Modified: Sun, 02 Feb 2020 03:36:10 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeaef2a78b559791011534abf0ee2a723b138776372b00019af6f1bcf1b59da`  
		Last Modified: Sun, 02 Feb 2020 03:36:21 GMT  
		Size: 77.9 MB (77940591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf387e3c6ea73ebb6cd13db382724dff9771329e421c8c4ed454fe11927aea0e`  
		Last Modified: Sun, 02 Feb 2020 03:36:09 GMT  
		Size: 1.3 MB (1283198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662f8c8a715db4b4d679682f19697f18f3d11ce144ca00a77c43d87f8251198e`  
		Last Modified: Sun, 02 Feb 2020 03:36:08 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58d75b229dcd884bd3aa4e230e09890af1beccdf1e73b531fdfef09787a956f`  
		Last Modified: Sun, 02 Feb 2020 03:36:07 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e04af6349cfcff77309336b34350e8fd67956803fe9408f9ff99f121eb6f15`  
		Last Modified: Sun, 02 Feb 2020 03:36:09 GMT  
		Size: 2.5 MB (2463866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babe457f5e43177a09c215741217f93c7a724ca2a67b1bbd2b2ae33bc8e96108`  
		Last Modified: Sun, 02 Feb 2020 03:36:29 GMT  
		Size: 62.2 MB (62231901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9a86c32d5039b929295c3d0162a1177253345f3654fb1e75ddba4477957176`  
		Last Modified: Sun, 02 Feb 2020 03:36:39 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:3.4.13`

```console
$ docker pull redmine@sha256:f6559d4aa45c11d241acf5e5c2dd317520e71579a63f85fa89919d57765798eb
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

### `redmine:3.4.13` - linux; amd64

```console
$ docker pull redmine@sha256:4beb787321e64d4f9ee0864d211279b3c01ee99e61259529c75f340d012be97d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.5 MB (207502345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91750691100784163b27ba361763857c9b3db45acd8a73cd890fdd3b2becd79`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 15:05:12 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 15:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:09:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:21:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:21:30 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:53:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:53:14 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:53:14 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:53:14 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:53:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 02:53:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:12:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:10 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:12:10 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:12:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:12:11 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:12:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aac5e62bfbec87ca600e8d9ee16832e53efd48c6a1ad8f02c923545e2d32fc4`  
		Last Modified: Sat, 28 Dec 2019 15:19:25 GMT  
		Size: 22.0 MB (22006052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fd0e5c830a620f7adbe8dbf517f558bd629236c05e30a81562e627d41af933`  
		Last Modified: Tue, 07 Jan 2020 02:23:51 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda27aa91ecfc255aa8888f23781a4fd6c446c38b13fcf945d933d697868399d`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3047b43ab05eab0353c1e221caf7d98300915f73d638eeb5fc32c8c542f9f979`  
		Last Modified: Tue, 07 Jan 2020 03:00:49 GMT  
		Size: 80.2 MB (80161214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d379f55b07e46100b9811c56dc34b9488eeb5029cd6d5b5aa1d0d952db4585f4`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.3 MB (1296456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d615b50742767a48c5a2f96cb4848af939353414d875d60e5bfd09828138869`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64db6c7eb6d20bd9906e4c0a451b94d1f042f1e8724e096a58608af75e4570`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26258bfd510bef8a8d430c8304327ee816f16c1d11e96b4e9d3127b00eb7611a`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 2.5 MB (2463473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27b56d37a6fe981e5fa2e124b4c81a2b197c46c74beddca441e70d12b3c0d4`  
		Last Modified: Sat, 25 Jan 2020 03:16:42 GMT  
		Size: 61.9 MB (61938710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a824ae4c58c52b7a5ff3051b2a8f0239a28542e884ed3c3b341d33b56aa4d`  
		Last Modified: Sat, 25 Jan 2020 03:16:33 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4.13` - linux; arm variant v5

```console
$ docker pull redmine@sha256:c94aeafc4839953ffc6f1d091d0be07f4b08b8798aac09ad6d5553bccf4919f1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.3 MB (197297445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22cd43b3d587718da99aba51d70195446f839e60ec885836249565df5fa1e5f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:53:06 GMT
ENV RUBY_MAJOR=2.4
# Sun, 02 Feb 2020 02:53:07 GMT
ENV RUBY_VERSION=2.4.9
# Sun, 02 Feb 2020 02:53:07 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sun, 02 Feb 2020 02:53:08 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sun, 02 Feb 2020 03:00:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 03:00:15 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 03:00:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 03:00:16 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 03:00:18 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 03:00:19 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:58:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:59:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 10:00:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 10:00:16 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 10:00:17 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 10:00:18 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 10:00:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 10:00:24 GMT
ENV REDMINE_VERSION=3.4.13
# Sun, 02 Feb 2020 10:00:26 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Sun, 02 Feb 2020 10:00:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 10:06:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 10:06:54 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 10:06:55 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 10:06:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 10:06:56 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 10:06:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d66a1f914bdc48f10a9fb7fa826de1fc4d51127360bfb635de92800427c2c`  
		Last Modified: Sun, 02 Feb 2020 03:18:21 GMT  
		Size: 21.3 MB (21337996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59db49767202ac506ef64e9ad4e78c2222a92d585fc752c47494f69c8d66c40`  
		Last Modified: Sun, 02 Feb 2020 03:18:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb41ba2542818a91d69186164d2baa8245ac6afcfb94f1fcb0d6f6e512d1065`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd4d2b24e257beb61f33391e5e90e9967dc45a757e66afcf682f086ae1db02b`  
		Last Modified: Sun, 02 Feb 2020 10:09:15 GMT  
		Size: 76.0 MB (76036604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774123ad6534a0960d229fc9293ab82687ff0eb673ef39fe99574fdb43fc0300`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 1.3 MB (1254237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba04482a10d8e7ec8a828448873ef5521cb469231897b4757a6e3acb3772cce`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a493edaaf61e6e3d79bca713573cd3eada2ce4a0149ce264e8c82f1a087b407`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943138c7822bb22264d257ee437bf08d764d088aca0a6279ba23f62232241da4`  
		Last Modified: Sun, 02 Feb 2020 10:08:39 GMT  
		Size: 2.5 MB (2463871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bfefd54730a9b78dff4a21cc9482ecaa0526bbced5ccd32add28fead591f587`  
		Last Modified: Sun, 02 Feb 2020 10:08:55 GMT  
		Size: 61.0 MB (61044490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bbf1e5c954dbffe8437807f7327f66456bb1c60539fbea8fd822d16dcdfb2f`  
		Last Modified: Sun, 02 Feb 2020 10:08:37 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4.13` - linux; arm variant v7

```console
$ docker pull redmine@sha256:4c39f48cac800b36598706c649b989d6f5f9205f39ac72b306dacfe85dd38d43
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.8 MB (190775448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b3e252e5d8c5e730460892f1a9f42514c647123d5101525d0d055cc902bf803`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:51:26 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 21:51:27 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 21:51:29 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 21:51:29 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 21:57:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:57:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:15:36 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:15:37 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:15:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:15:41 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:52:03 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:52:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:53:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:53:17 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:53:18 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:53:18 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:53:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:53:20 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:53:21 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:53:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:23:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:23:58 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:23:59 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:24:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:24:02 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:24:03 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8baf5eda0f1fcf9d63cd20bab0bf046b7fdf99276524015b69f17a54f2d4e5bd`  
		Last Modified: Sat, 28 Dec 2019 22:15:15 GMT  
		Size: 21.3 MB (21261197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7799af941ea6a75fd00ff583cd811459d9aa1ebf9bbfe53c690c886f22090c7b`  
		Last Modified: Tue, 07 Jan 2020 03:19:29 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c215c6dca6c1749986f1b9558c12d97e3b6165c10c6adcd3dcab432b34a1afa`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8f67953faffb1c4e8fffb1caa9217a25357829e1bbc3542405026627994e64`  
		Last Modified: Tue, 07 Jan 2020 04:00:42 GMT  
		Size: 72.4 MB (72370843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99638607df68e0caa80b678073b2bc1ab6bed1e6e765fbd58b4988e0a71017b4`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 1.2 MB (1243561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78977b4c3dfedf84fb120dbfa4e54e630246641aa0d57ede77b71d350a609774`  
		Last Modified: Tue, 07 Jan 2020 04:00:18 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0a66cd3e3ab71fca594f8aff62bbba677266975b1a11f481c8ae2965e5ca51`  
		Last Modified: Tue, 07 Jan 2020 04:00:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b76411581c7df4e2b0a02012d441a45291a6285744c35eb2744a942f54b7560`  
		Last Modified: Tue, 07 Jan 2020 04:00:20 GMT  
		Size: 2.5 MB (2463868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c00cc8eff10d5bfb13c4eeadb6504d82f498ec7dd94327a00fa9bbbc5c109f`  
		Last Modified: Sat, 25 Jan 2020 02:25:43 GMT  
		Size: 60.9 MB (60884981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ec3548c1f4fb71a189745695038f0338727e1807ba1901b255f362827eddc6`  
		Last Modified: Sat, 25 Jan 2020 02:25:30 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4.13` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:957f9b274b869bd00c1179677cab1163d933e1c615fad331467dab582aed0c17
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.3 MB (203347558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5777787ec04c96709988514a7ead13444e1289631fd8c8e05fb49a69ecae4411`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 23:03:38 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 23:03:39 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 23:03:40 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 23:03:41 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 23:09:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 23:09:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:43:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:43:05 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:43:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:43:07 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:22:13 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:23:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:23:40 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:23:40 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:23:41 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:23:41 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:23:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:23:44 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:23:44 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:23:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:52:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:52:45 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:52:46 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:52:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:52:48 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:52:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5cb0a3803f06119e2e010bac2f8756f225c7aafdb2af8de4eaa2aa2ab7b54b`  
		Last Modified: Sat, 28 Dec 2019 23:25:14 GMT  
		Size: 21.9 MB (21879231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c771ed92dd7985dfe7f891a2a1dcd20a4924b1c897760f5a84805f5996ecfbe4`  
		Last Modified: Tue, 07 Jan 2020 02:46:44 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f143af2012a522002d49c8c5e35ad2f785ea557182fc369a45b1f83f18ed178`  
		Last Modified: Tue, 07 Jan 2020 03:32:12 GMT  
		Size: 1.8 KB (1752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae138bc962325d1988fa72ea2f6ee74ee8549c9a467873a8624a810371df69e`  
		Last Modified: Tue, 07 Jan 2020 03:32:34 GMT  
		Size: 78.8 MB (78782045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8add249b39c3d8ec3f40de3ca3f3fa8c28484688f18f819e44be255a154b9f6`  
		Last Modified: Tue, 07 Jan 2020 03:32:12 GMT  
		Size: 1.2 MB (1228475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7b17f7c48aaa1d7dffac2d6c94b30b55b46051c58d9102d265a3e694d7a736`  
		Last Modified: Tue, 07 Jan 2020 03:32:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e80fe221a061826ce2e5104101ae09f094f093004bc6b7735d85ef712d7781`  
		Last Modified: Tue, 07 Jan 2020 03:32:09 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c5178963f7abb7582e65919deb0614e9014cb4d013df72194bb2d91201ceaf8`  
		Last Modified: Tue, 07 Jan 2020 03:32:10 GMT  
		Size: 2.5 MB (2463878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa6ead016d43f4981848676dd1d46cd08e0cfc3bf743b2c9d06df8415ad3931e`  
		Last Modified: Sat, 25 Jan 2020 02:54:27 GMT  
		Size: 61.9 MB (61894027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ff648cf1b1bae072e3a39161c9356ff9fd977dd469225a5c5ef215033c04ad`  
		Last Modified: Sat, 25 Jan 2020 02:54:14 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4.13` - linux; 386

```console
$ docker pull redmine@sha256:9d20bae3dc8a25376db18c0942653aa050d19617f8ed641a89a24852b4699189
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (212966720 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48cd45f82afe394a48d66b2244501078593165b9b5070f3016083c535401a04e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 16:24:30 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 16:24:31 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 16:30:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 16:30:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:40:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:40:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:40:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:40:07 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:07:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:08:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:08:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:08:12 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:08:12 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:08:13 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:08:13 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:08:14 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:08:14 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:08:17 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:55:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:55:06 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:55:07 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:55:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:55:07 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:55:07 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c021c8bfb2bb7e4f5caefd65e47f63eebb61502811966d3adc3f94ed9971017`  
		Last Modified: Sat, 28 Dec 2019 16:46:27 GMT  
		Size: 21.5 MB (21545961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33387c53c9ce779731032ff2f975ff7bbf0a16cd0551530997c664fec29ffb9a`  
		Last Modified: Tue, 07 Jan 2020 02:42:33 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdbef8b208533e2164c865470a9f1eb7ff708ecf888e79a7a884f20f5d93a45`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab5be34e7c4dc9dacc59a617b7f06eb1eb3ad229c4eb52da844415056b5f70`  
		Last Modified: Tue, 07 Jan 2020 03:12:17 GMT  
		Size: 81.6 MB (81574487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902840c7a384de1512dc1b47ecb4131fd83059a1ec3573014a974cecc6de24dd`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 1.3 MB (1261121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1807d33df93b1be2b8457093bccf02a94b6497f02105ec86c2408ac7cd8feccf`  
		Last Modified: Tue, 07 Jan 2020 03:11:54 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2991d075bf2bd2e85f753f498185dd38bfec5885dc0da5ad01c74c1e0d34ee1e`  
		Last Modified: Tue, 07 Jan 2020 03:11:54 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7f65bcaf193982883ff7c676cf3acd30476b7bf836c6fa410fd0bc7b7f645`  
		Last Modified: Tue, 07 Jan 2020 03:11:56 GMT  
		Size: 2.5 MB (2463470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9c6ceadaecf4398689a031439e3820eaa178b90b78d55176bbe3bfb6ba6e9`  
		Last Modified: Sat, 25 Jan 2020 01:56:17 GMT  
		Size: 61.2 MB (61164251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef61387ac2248fbdd6ba623bb119faa53406da27e4e5a8b8de36c60c0124fdb`  
		Last Modified: Sat, 25 Jan 2020 01:56:07 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4.13` - linux; ppc64le

```console
$ docker pull redmine@sha256:b92641f85841d118e8ce915e66fa19f48099e1c4729c3642a1eb7aed6c933b51
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.7 MB (218738140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f42e869aa800a67426ec040dda456b59adf3e38fd56451ba30a4f5961d05d77`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 05:07:30 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 05:07:32 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 05:07:33 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 05:07:35 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 05:16:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 05:17:01 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:22:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:22:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:22:55 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:22:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:16:32 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:18:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:19:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:19:36 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:19:38 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:19:41 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:19:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:19:47 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 03:19:49 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 03:19:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:28:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:28:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:28:22 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:28:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:28:29 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:28:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0831251b6fc73f4a098076145b4eedff1f2043b17e07a22a640aac457b19ffab`  
		Last Modified: Sat, 28 Dec 2019 05:31:10 GMT  
		Size: 22.5 MB (22518813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f17dc85665a35195e0378cddb30197da86e7d824c5330302c8b74d2dc7bd254`  
		Last Modified: Tue, 07 Jan 2020 02:30:07 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ff712870942f8f279111b569dd620512940f713de5a18702909c666b82283d`  
		Last Modified: Tue, 07 Jan 2020 03:31:00 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:815827d563f9f23bf0c3e35c713e3b20f90ccdb1d3d9bc9411efe6507d2c229f`  
		Last Modified: Tue, 07 Jan 2020 03:31:24 GMT  
		Size: 86.8 MB (86837755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f077a99d3a54521280a74467d75d74dc098e16cc5401d15524c42adce16819a7`  
		Last Modified: Tue, 07 Jan 2020 03:31:00 GMT  
		Size: 1.2 MB (1218174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0de3d5e5366fabf9fdc6c1f4eb2c2f92afde26d760575faf726ff770be38799`  
		Last Modified: Tue, 07 Jan 2020 03:30:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374d354d8b463223158de295e4a199502ea29b7f1b51c490c7cdd3e01e560cd7`  
		Last Modified: Tue, 07 Jan 2020 03:30:56 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931d1fd1f3723fb7145a7656f58f20ae8c7267107e777d38e479d92163e07abd`  
		Last Modified: Tue, 07 Jan 2020 03:30:57 GMT  
		Size: 2.5 MB (2463873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c41537c282aa3c5005eed86f46ed7e478e4d7f43cb38d67c0938a23d0b58f64`  
		Last Modified: Sat, 25 Jan 2020 03:30:16 GMT  
		Size: 62.5 MB (62488597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b29e8b55367dfb30b9a185fd4565e93a20c53fa0c0a1aa7e4022133c0aab87f8`  
		Last Modified: Sat, 25 Jan 2020 03:30:05 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:3.4.13` - linux; s390x

```console
$ docker pull redmine@sha256:2370a4642f404adbcdd7c37975e2aa8a4a9c399593cf21b831a7753bf31f1fd2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202577034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:889f0b16b19300fc0a24e1c00746a0ab8ffe37e3001f3e859a8832c7e724ffeb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:48:48 GMT
ENV RUBY_MAJOR=2.4
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 01 Feb 2020 22:48:49 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 01 Feb 2020 22:51:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:51:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:51:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:51:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:51:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:51:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:31:52 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:32:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:32:25 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:32:25 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:32:25 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:32:25 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:32:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:32:26 GMT
ENV REDMINE_VERSION=3.4.13
# Sun, 02 Feb 2020 03:32:26 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Sun, 02 Feb 2020 03:32:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:34:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:34:39 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:34:39 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:34:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:34:39 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:34:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ace099387f5254edf276126e046611f26609fd7b03c6eccab25882e8492ab41f`  
		Last Modified: Sat, 01 Feb 2020 22:58:36 GMT  
		Size: 22.2 MB (22151592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b170fa9fa8c788d38c6d6505a94b57d409b33565fd70320c01ce2c1a22977c6`  
		Last Modified: Sat, 01 Feb 2020 22:58:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f8b559eb775e7ef2268ad21235635a36ac961841bf8d21ff310f414a71c80e`  
		Last Modified: Sun, 02 Feb 2020 03:36:10 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aeaef2a78b559791011534abf0ee2a723b138776372b00019af6f1bcf1b59da`  
		Last Modified: Sun, 02 Feb 2020 03:36:21 GMT  
		Size: 77.9 MB (77940591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf387e3c6ea73ebb6cd13db382724dff9771329e421c8c4ed454fe11927aea0e`  
		Last Modified: Sun, 02 Feb 2020 03:36:09 GMT  
		Size: 1.3 MB (1283198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662f8c8a715db4b4d679682f19697f18f3d11ce144ca00a77c43d87f8251198e`  
		Last Modified: Sun, 02 Feb 2020 03:36:08 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58d75b229dcd884bd3aa4e230e09890af1beccdf1e73b531fdfef09787a956f`  
		Last Modified: Sun, 02 Feb 2020 03:36:07 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e04af6349cfcff77309336b34350e8fd67956803fe9408f9ff99f121eb6f15`  
		Last Modified: Sun, 02 Feb 2020 03:36:09 GMT  
		Size: 2.5 MB (2463866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:babe457f5e43177a09c215741217f93c7a724ca2a67b1bbd2b2ae33bc8e96108`  
		Last Modified: Sun, 02 Feb 2020 03:36:29 GMT  
		Size: 62.2 MB (62231901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9a86c32d5039b929295c3d0162a1177253345f3654fb1e75ddba4477957176`  
		Last Modified: Sun, 02 Feb 2020 03:36:39 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:3.4.13-alpine`

```console
$ docker pull redmine@sha256:8cfd3510d6764d58ce5e117fc1f858d98a5956d836dda57626bc9a9606c7323f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:3.4.13-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:a7fa111e00068a60a15eacaf9ad11ca8db4b7929469cd49f85714a218a76ce56
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156153745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8259090d178e8fb12df9f3d4e431bd79e8270029500b7797ee8cfc1d018a660`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_MAJOR=2.4
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_VERSION=2.4.9
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Thu, 23 Jan 2020 23:00:16 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Thu, 23 Jan 2020 23:06:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 23:06:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 23:06:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 23:06:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 23:06:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 23:06:30 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:24:44 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 24 Jan 2020 15:24:52 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Fri, 24 Jan 2020 15:24:53 GMT
ENV RAILS_ENV=production
# Fri, 24 Jan 2020 15:24:53 GMT
WORKDIR /usr/src/redmine
# Fri, 24 Jan 2020 15:24:53 GMT
ENV HOME=/home/redmine
# Fri, 24 Jan 2020 15:24:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 24 Jan 2020 15:24:54 GMT
ENV REDMINE_VERSION=3.4.13
# Fri, 24 Jan 2020 15:24:54 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Fri, 24 Jan 2020 15:24:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:14:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:14:36 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:14:36 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:14:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:14:36 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:14:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cfcf9ea42c9ec1b11a4ff2b7d27b908592b82b7e0f30a65325c27366087d9c`  
		Last Modified: Thu, 23 Jan 2020 23:08:27 GMT  
		Size: 22.8 MB (22821242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05133739e27c89886d8326fab4637b17f5be9ba6911377081d055c17802a7cb`  
		Last Modified: Thu, 23 Jan 2020 23:08:22 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb3b93c12687c41298f346a387962f3814e677aeb84f1b30feb98d66a26c729`  
		Last Modified: Fri, 24 Jan 2020 15:28:15 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b05c8061524c573766c6947d511203084e274f98e5e5139bfc48640f414437c`  
		Last Modified: Fri, 24 Jan 2020 15:28:51 GMT  
		Size: 65.7 MB (65727265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaaf598f37860e727a62490f2f41bc6c1b0ebd0ceea3d847fb6bd37eb3deb8f`  
		Last Modified: Fri, 24 Jan 2020 15:28:14 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a34d3df39933babed2228a5ba0cf7c208dc606e14b42dafb9b1eab9a8f3973c`  
		Last Modified: Fri, 24 Jan 2020 15:28:14 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c99b56a190ee237d0173d3850c2a76784f7e6171f58eb209d73c0b8a3c6f26`  
		Last Modified: Fri, 24 Jan 2020 15:28:15 GMT  
		Size: 2.5 MB (2464289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0533af3382a728453efbf76861619d015c43eb1005bcb41b3cd9f8380d8b5ff`  
		Last Modified: Sat, 25 Jan 2020 03:17:04 GMT  
		Size: 61.3 MB (61319827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00547284caab370d894d098a856a792d1b5992fbbde4361c5855c222e6999f3b`  
		Last Modified: Sat, 25 Jan 2020 03:16:56 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:3.4.13-passenger`

```console
$ docker pull redmine@sha256:d7e84ee9915b17b4a78b104db8f0333ae89b28759934fd00594bf730a713240d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:3.4.13-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:a59f8054b8f74ce957eca255b93211ef4b8374d04245da03a85cfed1e27a9231
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232357569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a779098a33b5db5a6e904c218a8192f662b12eeeb7c814baf25bf0b900f48f84`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 15:05:12 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 15:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:09:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:21:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:21:30 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:53:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:53:14 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:53:14 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:53:14 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:53:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 02:53:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:12:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:10 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:12:10 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:12:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:12:11 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:12:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:12:23 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:12:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:42 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:12:42 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:12:42 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aac5e62bfbec87ca600e8d9ee16832e53efd48c6a1ad8f02c923545e2d32fc4`  
		Last Modified: Sat, 28 Dec 2019 15:19:25 GMT  
		Size: 22.0 MB (22006052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fd0e5c830a620f7adbe8dbf517f558bd629236c05e30a81562e627d41af933`  
		Last Modified: Tue, 07 Jan 2020 02:23:51 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda27aa91ecfc255aa8888f23781a4fd6c446c38b13fcf945d933d697868399d`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3047b43ab05eab0353c1e221caf7d98300915f73d638eeb5fc32c8c542f9f979`  
		Last Modified: Tue, 07 Jan 2020 03:00:49 GMT  
		Size: 80.2 MB (80161214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d379f55b07e46100b9811c56dc34b9488eeb5029cd6d5b5aa1d0d952db4585f4`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.3 MB (1296456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d615b50742767a48c5a2f96cb4848af939353414d875d60e5bfd09828138869`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64db6c7eb6d20bd9906e4c0a451b94d1f042f1e8724e096a58608af75e4570`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26258bfd510bef8a8d430c8304327ee816f16c1d11e96b4e9d3127b00eb7611a`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 2.5 MB (2463473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27b56d37a6fe981e5fa2e124b4c81a2b197c46c74beddca441e70d12b3c0d4`  
		Last Modified: Sat, 25 Jan 2020 03:16:42 GMT  
		Size: 61.9 MB (61938710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a824ae4c58c52b7a5ff3051b2a8f0239a28542e884ed3c3b341d33b56aa4d`  
		Last Modified: Sat, 25 Jan 2020 03:16:33 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b54765efc339f1a67765dcc94c9981dc71b2496471cf211176ac1370a8cd8b`  
		Last Modified: Sat, 25 Jan 2020 03:16:51 GMT  
		Size: 19.9 MB (19937379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3896276a138101c67c7d1dcec7c270f7a56d34f5aad54f8e4c92d8ff41536081`  
		Last Modified: Sat, 25 Jan 2020 03:16:48 GMT  
		Size: 4.9 MB (4917845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:3.4-alpine`

```console
$ docker pull redmine@sha256:8cfd3510d6764d58ce5e117fc1f858d98a5956d836dda57626bc9a9606c7323f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:3.4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:a7fa111e00068a60a15eacaf9ad11ca8db4b7929469cd49f85714a218a76ce56
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156153745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8259090d178e8fb12df9f3d4e431bd79e8270029500b7797ee8cfc1d018a660`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_MAJOR=2.4
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_VERSION=2.4.9
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Thu, 23 Jan 2020 23:00:16 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Thu, 23 Jan 2020 23:06:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 23:06:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 23:06:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 23:06:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 23:06:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 23:06:30 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:24:44 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 24 Jan 2020 15:24:52 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Fri, 24 Jan 2020 15:24:53 GMT
ENV RAILS_ENV=production
# Fri, 24 Jan 2020 15:24:53 GMT
WORKDIR /usr/src/redmine
# Fri, 24 Jan 2020 15:24:53 GMT
ENV HOME=/home/redmine
# Fri, 24 Jan 2020 15:24:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 24 Jan 2020 15:24:54 GMT
ENV REDMINE_VERSION=3.4.13
# Fri, 24 Jan 2020 15:24:54 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Fri, 24 Jan 2020 15:24:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:14:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:14:36 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:14:36 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:14:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:14:36 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:14:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cfcf9ea42c9ec1b11a4ff2b7d27b908592b82b7e0f30a65325c27366087d9c`  
		Last Modified: Thu, 23 Jan 2020 23:08:27 GMT  
		Size: 22.8 MB (22821242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05133739e27c89886d8326fab4637b17f5be9ba6911377081d055c17802a7cb`  
		Last Modified: Thu, 23 Jan 2020 23:08:22 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb3b93c12687c41298f346a387962f3814e677aeb84f1b30feb98d66a26c729`  
		Last Modified: Fri, 24 Jan 2020 15:28:15 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b05c8061524c573766c6947d511203084e274f98e5e5139bfc48640f414437c`  
		Last Modified: Fri, 24 Jan 2020 15:28:51 GMT  
		Size: 65.7 MB (65727265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaaf598f37860e727a62490f2f41bc6c1b0ebd0ceea3d847fb6bd37eb3deb8f`  
		Last Modified: Fri, 24 Jan 2020 15:28:14 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a34d3df39933babed2228a5ba0cf7c208dc606e14b42dafb9b1eab9a8f3973c`  
		Last Modified: Fri, 24 Jan 2020 15:28:14 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c99b56a190ee237d0173d3850c2a76784f7e6171f58eb209d73c0b8a3c6f26`  
		Last Modified: Fri, 24 Jan 2020 15:28:15 GMT  
		Size: 2.5 MB (2464289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0533af3382a728453efbf76861619d015c43eb1005bcb41b3cd9f8380d8b5ff`  
		Last Modified: Sat, 25 Jan 2020 03:17:04 GMT  
		Size: 61.3 MB (61319827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00547284caab370d894d098a856a792d1b5992fbbde4361c5855c222e6999f3b`  
		Last Modified: Sat, 25 Jan 2020 03:16:56 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:3.4-passenger`

```console
$ docker pull redmine@sha256:d7e84ee9915b17b4a78b104db8f0333ae89b28759934fd00594bf730a713240d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:3.4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:a59f8054b8f74ce957eca255b93211ef4b8374d04245da03a85cfed1e27a9231
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232357569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a779098a33b5db5a6e904c218a8192f662b12eeeb7c814baf25bf0b900f48f84`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 15:05:12 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 15:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:09:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:21:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:21:30 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:53:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:53:14 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:53:14 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:53:14 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:53:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 02:53:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:12:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:10 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:12:10 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:12:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:12:11 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:12:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:12:23 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:12:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:42 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:12:42 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:12:42 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aac5e62bfbec87ca600e8d9ee16832e53efd48c6a1ad8f02c923545e2d32fc4`  
		Last Modified: Sat, 28 Dec 2019 15:19:25 GMT  
		Size: 22.0 MB (22006052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fd0e5c830a620f7adbe8dbf517f558bd629236c05e30a81562e627d41af933`  
		Last Modified: Tue, 07 Jan 2020 02:23:51 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda27aa91ecfc255aa8888f23781a4fd6c446c38b13fcf945d933d697868399d`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3047b43ab05eab0353c1e221caf7d98300915f73d638eeb5fc32c8c542f9f979`  
		Last Modified: Tue, 07 Jan 2020 03:00:49 GMT  
		Size: 80.2 MB (80161214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d379f55b07e46100b9811c56dc34b9488eeb5029cd6d5b5aa1d0d952db4585f4`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.3 MB (1296456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d615b50742767a48c5a2f96cb4848af939353414d875d60e5bfd09828138869`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64db6c7eb6d20bd9906e4c0a451b94d1f042f1e8724e096a58608af75e4570`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26258bfd510bef8a8d430c8304327ee816f16c1d11e96b4e9d3127b00eb7611a`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 2.5 MB (2463473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27b56d37a6fe981e5fa2e124b4c81a2b197c46c74beddca441e70d12b3c0d4`  
		Last Modified: Sat, 25 Jan 2020 03:16:42 GMT  
		Size: 61.9 MB (61938710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a824ae4c58c52b7a5ff3051b2a8f0239a28542e884ed3c3b341d33b56aa4d`  
		Last Modified: Sat, 25 Jan 2020 03:16:33 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b54765efc339f1a67765dcc94c9981dc71b2496471cf211176ac1370a8cd8b`  
		Last Modified: Sat, 25 Jan 2020 03:16:51 GMT  
		Size: 19.9 MB (19937379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3896276a138101c67c7d1dcec7c270f7a56d34f5aad54f8e4c92d8ff41536081`  
		Last Modified: Sat, 25 Jan 2020 03:16:48 GMT  
		Size: 4.9 MB (4917845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:3-alpine`

```console
$ docker pull redmine@sha256:8cfd3510d6764d58ce5e117fc1f858d98a5956d836dda57626bc9a9606c7323f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:3-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:a7fa111e00068a60a15eacaf9ad11ca8db4b7929469cd49f85714a218a76ce56
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.2 MB (156153745 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8259090d178e8fb12df9f3d4e431bd79e8270029500b7797ee8cfc1d018a660`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_MAJOR=2.4
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_VERSION=2.4.9
# Thu, 23 Jan 2020 23:00:15 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Thu, 23 Jan 2020 23:00:16 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Thu, 23 Jan 2020 23:06:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 23:06:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 23:06:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 23:06:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 23:06:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 23:06:30 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:24:44 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 24 Jan 2020 15:24:52 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Fri, 24 Jan 2020 15:24:53 GMT
ENV RAILS_ENV=production
# Fri, 24 Jan 2020 15:24:53 GMT
WORKDIR /usr/src/redmine
# Fri, 24 Jan 2020 15:24:53 GMT
ENV HOME=/home/redmine
# Fri, 24 Jan 2020 15:24:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 24 Jan 2020 15:24:54 GMT
ENV REDMINE_VERSION=3.4.13
# Fri, 24 Jan 2020 15:24:54 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Fri, 24 Jan 2020 15:24:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:14:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:14:36 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:14:36 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:14:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:14:36 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:14:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cfcf9ea42c9ec1b11a4ff2b7d27b908592b82b7e0f30a65325c27366087d9c`  
		Last Modified: Thu, 23 Jan 2020 23:08:27 GMT  
		Size: 22.8 MB (22821242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05133739e27c89886d8326fab4637b17f5be9ba6911377081d055c17802a7cb`  
		Last Modified: Thu, 23 Jan 2020 23:08:22 GMT  
		Size: 140.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb3b93c12687c41298f346a387962f3814e677aeb84f1b30feb98d66a26c729`  
		Last Modified: Fri, 24 Jan 2020 15:28:15 GMT  
		Size: 1.2 KB (1219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b05c8061524c573766c6947d511203084e274f98e5e5139bfc48640f414437c`  
		Last Modified: Fri, 24 Jan 2020 15:28:51 GMT  
		Size: 65.7 MB (65727265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaaf598f37860e727a62490f2f41bc6c1b0ebd0ceea3d847fb6bd37eb3deb8f`  
		Last Modified: Fri, 24 Jan 2020 15:28:14 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a34d3df39933babed2228a5ba0cf7c208dc606e14b42dafb9b1eab9a8f3973c`  
		Last Modified: Fri, 24 Jan 2020 15:28:14 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98c99b56a190ee237d0173d3850c2a76784f7e6171f58eb209d73c0b8a3c6f26`  
		Last Modified: Fri, 24 Jan 2020 15:28:15 GMT  
		Size: 2.5 MB (2464289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0533af3382a728453efbf76861619d015c43eb1005bcb41b3cd9f8380d8b5ff`  
		Last Modified: Sat, 25 Jan 2020 03:17:04 GMT  
		Size: 61.3 MB (61319827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00547284caab370d894d098a856a792d1b5992fbbde4361c5855c222e6999f3b`  
		Last Modified: Sat, 25 Jan 2020 03:16:56 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:3-passenger`

```console
$ docker pull redmine@sha256:d7e84ee9915b17b4a78b104db8f0333ae89b28759934fd00594bf730a713240d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:3-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:a59f8054b8f74ce957eca255b93211ef4b8374d04245da03a85cfed1e27a9231
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232357569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a779098a33b5db5a6e904c218a8192f662b12eeeb7c814baf25bf0b900f48f84`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_MAJOR=2.4
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 28 Dec 2019 15:05:11 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 28 Dec 2019 15:05:12 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 28 Dec 2019 15:09:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:09:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:21:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:21:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:21:30 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:53:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:53:14 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:53:14 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:53:14 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:53:14 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:53:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_VERSION=3.4.13
# Tue, 07 Jan 2020 02:53:15 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Tue, 07 Jan 2020 02:53:21 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:12:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:10 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:12:10 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:12:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:12:11 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:12:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:12:23 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:12:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:12:42 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:12:42 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:12:42 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aac5e62bfbec87ca600e8d9ee16832e53efd48c6a1ad8f02c923545e2d32fc4`  
		Last Modified: Sat, 28 Dec 2019 15:19:25 GMT  
		Size: 22.0 MB (22006052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60fd0e5c830a620f7adbe8dbf517f558bd629236c05e30a81562e627d41af933`  
		Last Modified: Tue, 07 Jan 2020 02:23:51 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda27aa91ecfc255aa8888f23781a4fd6c446c38b13fcf945d933d697868399d`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3047b43ab05eab0353c1e221caf7d98300915f73d638eeb5fc32c8c542f9f979`  
		Last Modified: Tue, 07 Jan 2020 03:00:49 GMT  
		Size: 80.2 MB (80161214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d379f55b07e46100b9811c56dc34b9488eeb5029cd6d5b5aa1d0d952db4585f4`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 1.3 MB (1296456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d615b50742767a48c5a2f96cb4848af939353414d875d60e5bfd09828138869`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb64db6c7eb6d20bd9906e4c0a451b94d1f042f1e8724e096a58608af75e4570`  
		Last Modified: Tue, 07 Jan 2020 03:00:28 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26258bfd510bef8a8d430c8304327ee816f16c1d11e96b4e9d3127b00eb7611a`  
		Last Modified: Tue, 07 Jan 2020 03:00:29 GMT  
		Size: 2.5 MB (2463473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc27b56d37a6fe981e5fa2e124b4c81a2b197c46c74beddca441e70d12b3c0d4`  
		Last Modified: Sat, 25 Jan 2020 03:16:42 GMT  
		Size: 61.9 MB (61938710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270a824ae4c58c52b7a5ff3051b2a8f0239a28542e884ed3c3b341d33b56aa4d`  
		Last Modified: Sat, 25 Jan 2020 03:16:33 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33b54765efc339f1a67765dcc94c9981dc71b2496471cf211176ac1370a8cd8b`  
		Last Modified: Sat, 25 Jan 2020 03:16:51 GMT  
		Size: 19.9 MB (19937379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3896276a138101c67c7d1dcec7c270f7a56d34f5aad54f8e4c92d8ff41536081`  
		Last Modified: Sat, 25 Jan 2020 03:16:48 GMT  
		Size: 4.9 MB (4917845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4`

```console
$ docker pull redmine@sha256:31dc2573b1c77945e98ad71e3ba671f787b3f402abf9d00af0b5062d3e0176bb
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
$ docker pull redmine@sha256:b020b824c4bc29851cb807d079249567fba38953a183e5c6c156843fe044fd5e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.4 MB (215374935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe885543d5387f35a4aa3a2a65968c4ace488cb67a6c40677407a4aec17c9ed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:59:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:59:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:59:53 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:59:53 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:59:53 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:59:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:59:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:01:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:01:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:01:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:01:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:01:50 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:01:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20875f0e3d3802e64f74c9b1930e47473aa008ac1e3e2f5449ad290a85ab57`  
		Last Modified: Sat, 25 Jan 2020 03:15:23 GMT  
		Size: 93.1 MB (93059371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309a0bcae95c3ed0d1e34a294ec279f52939042fe32ae9ce3795d64ac30b93b`  
		Last Modified: Sat, 25 Jan 2020 03:15:04 GMT  
		Size: 1.3 MB (1307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce465b077ee104502ac0d3bb56ee609f8466b52df3019fc8e0eb9910c16c2475`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fd3dbd195628a62fb6e32bdc5cb84a1ad44500433876fab465c8e8d1d23c9`  
		Last Modified: Sat, 25 Jan 2020 03:15:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc96f26d91b45b07346a0a2064741540002911ab51b1c01a69d794eb672085c`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.7 MB (2735388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d61a0e145c858537c040f69d6811589e5d6e96ac59368d19b40ec966610ba7`  
		Last Modified: Sat, 25 Jan 2020 03:15:11 GMT  
		Size: 57.2 MB (57190428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5794504759a01ead1a31eb3f4b6799addca73aaca089b237498d8b773f0400f4`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:d81487b3c1ad872dcf937922c70e1b33aa56ba4ce5190286fa2d86d8adeedc35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204856480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb08d7d0f07498236e41fdcf83db177fea39c1c452b01cf798acd1a6878621b8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:16:09 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 02:16:12 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 02:16:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 02:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 02:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 02:19:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 02:20:03 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:44:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:46:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:46:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:46:22 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 09:46:22 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 09:46:23 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 09:46:25 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 09:46:25 GMT
ENV REDMINE_VERSION=4.1.0
# Sun, 02 Feb 2020 09:46:26 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sun, 02 Feb 2020 09:46:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 09:50:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:50:23 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 09:50:23 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 09:50:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:50:25 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 09:50:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd05ffdd7888092a6ef03be377963c297edec0344ce762bb6b3e1e2f114b94`  
		Last Modified: Sun, 02 Feb 2020 03:16:40 GMT  
		Size: 20.7 MB (20712712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e99c39d252f8cf22fae4749b2764aec83374848c63b8546989494f7f7a1cd2`  
		Last Modified: Sun, 02 Feb 2020 03:16:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff532b6c7852f386bab467c7b3f4b83b928ea314de236796805380d538c9717`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2386bd4b4f50f1d8f93b32303170d0866887841332213e58a371ca1bb7a20589`  
		Last Modified: Sun, 02 Feb 2020 10:07:52 GMT  
		Size: 88.7 MB (88656018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3116bbee905e3f17958856da579a4d33255abeddc081a9673f7e7751b098ebe`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.3 MB (1265374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a450151953d1dd4bd9521617998e60400bbde5af211dc4477b78be4b3f12675b`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98603c054417f4f97943b58f87a4064bff0a6fdcc842f801c987da619b29ff3b`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23326958468d4e64c292656ee80e58902c0ffdb4d9dd0ebe0f3ab5264ce8d22`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 2.7 MB (2735847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdb53308614fca2cb01c7b7851bffaab106d45dee36ec93f25b881241ff56a0`  
		Last Modified: Sun, 02 Feb 2020 10:07:31 GMT  
		Size: 56.3 MB (56326279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2affc3b6a6c7eac6ca68be7e12a92c5998344deee6abc0a859b5698bb25dfdcc`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:fd859aecbff1334ede20c1579bbabb5bd45bf7594547561cdc1d27758507b025
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197890698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5ca2f6d8a5214b523a543ba010bc02d222e1415eb4513f339f22da0cb06cba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 21:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 21:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:22:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:12:51 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:39:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:06:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:07:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:07:02 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:07:03 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:07:04 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:07:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:07:07 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:07:08 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:07:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:10:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:10:55 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:10:56 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:10:58 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:10:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4c32e3c622deadf3234025d30c88895c18ae7eac94288d4e42f903c4a72f5`  
		Last Modified: Sat, 28 Dec 2019 22:13:25 GMT  
		Size: 20.6 MB (20620161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe49bcffa8c82983470bbf0074d2412dacbf1f325bcc2ffb85fddcbda7c7da8`  
		Last Modified: Tue, 07 Jan 2020 03:17:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67711a5ad765c81e93b31a6b9e1b763d7d8448315399ea1765bf97971567bfcb`  
		Last Modified: Tue, 07 Jan 2020 03:59:01 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22df051691cc30d921b9d70b85efd5cd46a51c055fb7a885fe2ae9ef34f1965`  
		Last Modified: Sat, 25 Jan 2020 02:24:54 GMT  
		Size: 84.7 MB (84708006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d2540796d803b25bed6e74b93432545aae43cc0a48e7fbf6093c5e6823b0a4`  
		Last Modified: Sat, 25 Jan 2020 02:24:26 GMT  
		Size: 1.3 MB (1258219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a8c6a15e107f7bf7271010e2bdf9b48e58f6598901bd1971275252da7f8ae`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7837a0650c1e2b2d0636d7b4235bda5767e5c67ef97f5a6747edd98b03f63c7`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d2ce28f760155459539026440cf179c5489575000c97eae858f42d01c9568c`  
		Last Modified: Sat, 25 Jan 2020 02:24:25 GMT  
		Size: 2.7 MB (2735850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646d541d0d57a917412aac2e133006b795fac0f438acd943f02709948cba90e6`  
		Last Modified: Sat, 25 Jan 2020 02:24:38 GMT  
		Size: 56.0 MB (56017460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714489a49c6e19537c912f14ef35b3218572e68b1c1f851192d706acad806bed`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:58f2624f1a316fd842c70194c733401281f3850fa6fa8f1340c7d2b9198cfb57
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.1 MB (211120176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1aa59e95791a967e02ca12ecfd915f8009cbca478126af0f52e55f8759923c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 22:28:49 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 22:28:50 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 22:28:51 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 22:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 22:32:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:41:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:41:14 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:06:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:34:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:35:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:35:13 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:35:15 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:35:15 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:35:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:35:18 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:35:20 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:35:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:40:02 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:40:03 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:40:12 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:40:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc7342d754a238156ddfd7ee18001a3862d29761cdf787ceb41e05bfde38061`  
		Last Modified: Sat, 28 Dec 2019 23:23:41 GMT  
		Size: 21.3 MB (21281931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1828050bdff9d08ad357e12a1bd0639c7818f955a59966e76a48d90c55ccc2`  
		Last Modified: Tue, 07 Jan 2020 02:45:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec8c6749d85258e801554c4c6b4d94f96e6ca4909194be6fc4aa78f0ba7caf`  
		Last Modified: Tue, 07 Jan 2020 03:31:11 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79ff809afa32d5baba46f2f7bde80a0ab57dc15374657c246cdb0db778b6c4d`  
		Last Modified: Sat, 25 Jan 2020 02:53:40 GMT  
		Size: 91.6 MB (91645815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee31ede564e2642f141b9f0353eb8a17b5738e42230d2666c77f0057e3c71ed`  
		Last Modified: Sat, 25 Jan 2020 02:53:12 GMT  
		Size: 1.2 MB (1242951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538e9d155ef665df153038fe494404878b140304e7a7358d79c50f3c06cdd0f1`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24c8d492a9f691c39c85e79b35ccf567e2430697d78dabeb9149cb9789d5d1a`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20410b8776eb35b945d7702f61a7e2c0d2f768b9d7e3919c8153e5f1f45b0370`  
		Last Modified: Sat, 25 Jan 2020 02:53:11 GMT  
		Size: 2.7 MB (2735848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17724b15809fcdf62e3624dc2b6d2500d0531bf9fa6a801f1dad1ad4a5e70b87`  
		Last Modified: Sat, 25 Jan 2020 02:53:23 GMT  
		Size: 57.1 MB (57113718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8820389aab406aeaa971c6a195fb163be61f4b7d5b3ff008a5f4f41897e285`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; 386

```console
$ docker pull redmine@sha256:f700874a4b5a04b0de5054424a487980540e0cbc11dd8880c89437153e718aba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.8 MB (220831119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13bb3cef0fc5bee43a02ef2d01a7bc6cc73c13e1ecb2668ea53c6064fce16f77`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 15:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 15:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:48:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:39:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:39:08 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:00:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 01:47:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 01:47:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:47:29 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 01:47:29 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 01:47:29 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 01:47:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 01:47:30 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 01:47:31 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 01:47:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:49:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:49:23 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:49:23 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:49:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:49:24 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:49:24 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b12042d352b3390a1d5c085213ccee7f26bee56d8a1a3fb0a76e80159a411c`  
		Last Modified: Sat, 28 Dec 2019 16:44:44 GMT  
		Size: 20.9 MB (20885521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c53ce40fd432336a5365d519861a9d64c7cf858412dd402f939e5f6cb0ed3f`  
		Last Modified: Tue, 07 Jan 2020 02:41:40 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b71e9da85871d84768b7e4ee95650087a03f4db095955f62e526335b0c09aa4`  
		Last Modified: Tue, 07 Jan 2020 03:11:10 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5f640023220debb54aa59008a23084703fc0537fc624f8ceab4d90009b5f0a`  
		Last Modified: Sat, 25 Jan 2020 01:55:48 GMT  
		Size: 94.7 MB (94693229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c958a54bf64e77189cf05b4486d2756c03a8c3d2dfaa0623e2a09c1a5109e0b`  
		Last Modified: Sat, 25 Jan 2020 01:55:24 GMT  
		Size: 1.3 MB (1275383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00731a6396a0f584e04f340d4a49c149951c796ca229ed740930499b1a882c`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a2a82b5a98ff43706a5284dab0afd502f20a49c7a2a08ed51f40683ac458d`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d5165755570cce25c28f06dd103a1d73386b43cf12f92cd6ca898131ae5663`  
		Last Modified: Sat, 25 Jan 2020 01:55:24 GMT  
		Size: 2.7 MB (2735383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe1b8246e4d2cefa8623bb1ec59f0b3ab47bb321632de09d3ea2b875a984bc8`  
		Last Modified: Sat, 25 Jan 2020 01:55:33 GMT  
		Size: 56.3 MB (56284173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a398c5eaf1193a79396d5800707f6528d558924b2c597e2767da34ae511bb6`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; ppc64le

```console
$ docker pull redmine@sha256:f08f037717dc3721e961cb0907ae97ac8328ba24fe1bfa1b059ed270e9cfe715
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227173333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2bb12560bf4f88050034a40821bb893c2d88a2a3c4abd85702087a17761c09`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 04:44:05 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 04:44:07 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 04:44:10 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 04:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 04:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:18:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:18:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 03:06:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:06:20 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 03:06:23 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 03:06:27 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 03:06:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 03:06:35 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 03:06:37 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 03:06:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:10:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:10:41 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:10:42 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:10:47 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:10:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8219d68aec763d8d91942869b8dd9ef7233da0ba814028c00dce26b61b1ec`  
		Last Modified: Sat, 28 Dec 2019 05:29:59 GMT  
		Size: 22.0 MB (21968340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88418e7313544081130ec82f1125b007f6673672ed6fe3f2815a8bc0836d834d`  
		Last Modified: Tue, 07 Jan 2020 02:27:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811e39d17ef5178d803832537e4b94505620908b40d2ece5c639ebc74bb249c`  
		Last Modified: Tue, 07 Jan 2020 03:29:32 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fdc2fee5bcdaa20790472eb3b3e6a238cee4c14ea8503eaf556e87582caf2b`  
		Last Modified: Sat, 25 Jan 2020 03:29:20 GMT  
		Size: 100.3 MB (100282383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37063699c1769c556fcd7e961dae12c108451947f10a4381c9312fb86a65bb6b`  
		Last Modified: Sat, 25 Jan 2020 03:28:58 GMT  
		Size: 1.2 MB (1232203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77c914aba14ea81411aae5a9d0b596dbebda443ecb800ce8e717f0c782a367b`  
		Last Modified: Sat, 25 Jan 2020 03:28:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b47a8358f9f444669f85d1a5f3690a1d8e37b0c91e7a827ceb0b4937b251c5`  
		Last Modified: Sat, 25 Jan 2020 03:28:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b553f520f8f427b541d300f1b7cd485adf7ee67d7046a370c78d993aaebff1a7`  
		Last Modified: Sat, 25 Jan 2020 03:28:56 GMT  
		Size: 2.7 MB (2735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1492d8aabeb5a9c29d1c9c848723748f59b53365c4e70c0d9c897c329ca329`  
		Last Modified: Sat, 25 Jan 2020 03:29:06 GMT  
		Size: 57.7 MB (57743620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556573964a0bd208b3e595f68ab9d500f1405000b822b06641efaa11e9820c7b`  
		Last Modified: Sat, 25 Jan 2020 03:28:54 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; s390x

```console
$ docker pull redmine@sha256:ab1568d6b226e18d614f69224ab5082f76ab6c3c459575b451c0b43a044e4c88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210607230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e81bbd4d53db9fe58b1f99028cbe990f74848ac4052582c07576953e60742dc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_MAJOR=2.6
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 01 Feb 2020 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:36:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:36:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:36:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:24:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:25:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:25:35 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:25:36 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:25:36 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:25:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:25:37 GMT
ENV REDMINE_VERSION=4.1.0
# Sun, 02 Feb 2020 03:25:37 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sun, 02 Feb 2020 03:25:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:28:15 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:28:15 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:28:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:28:16 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:28:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f50ba1593f8ab66d1deaf12e190c35ecfea96815beda37efe10f1246f342b`  
		Last Modified: Sat, 01 Feb 2020 22:57:18 GMT  
		Size: 21.6 MB (21592569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8a5d1fd225888733445fbc5a03464b232ab7c659a3bf619e93c5670a0ca594`  
		Last Modified: Sat, 01 Feb 2020 22:57:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6b52758f305e2a6eca340f3801ffcd699d9f9863ebfe870573fbea05f125b`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c2d954e677f77134627d444d4526d3dd757e20731a3db791ee045bd3ff5`  
		Last Modified: Sun, 02 Feb 2020 03:35:13 GMT  
		Size: 90.8 MB (90810821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4b03bbe680823684e8167d23322040275fc82bb40b38251bd1aca1d9759997`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.3 MB (1297549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6a56833da980d550b03c0656e63d42b60190fa8f5b743d0efd1679e03cb5ea`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6743cd35c07b27ae19792d6c94243798a11247fa7a5f0fd8d63ec5fec7f8c8`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0844cdbf926f537d20bc1295376495cb2b126746d549e3cc88402e855e2f92`  
		Last Modified: Sun, 02 Feb 2020 03:34:58 GMT  
		Size: 2.7 MB (2735858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a0c8052dd4f2d2e8e61136ca875e5667f9fdd869156f21339a352533be465b`  
		Last Modified: Sun, 02 Feb 2020 03:35:25 GMT  
		Size: 57.7 MB (57664549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b47a626d921e859c5def90095c9624aa612e063bcacdce5bb5485574308e28`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0`

```console
$ docker pull redmine@sha256:2cbe178da1bc5ab4da1b7ec5b69ba5f55367dbc3cdfdb85a8144d76b356312c5
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
$ docker pull redmine@sha256:69a57b170618bc5ea16a564655faa4a675f8f3c13e37bc875efd8c01e146d120
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.1 MB (206096278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fe698f6b99ddbae61bb0bb6332fc61814fe13a0bb00652cc461ead815a8659`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:42:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:42:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:42:40 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:42:40 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:42:40 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:42:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:47:32 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 02:47:32 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 02:47:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:07:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:07:05 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:07:05 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:07:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:07:05 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:07:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c8c66f527fafb06b837048b77a717c5c453f36789591051417d3730279253a`  
		Last Modified: Tue, 07 Jan 2020 02:59:05 GMT  
		Size: 80.2 MB (80161685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e48374f11ea16d535dab197d7559592d994ed6d63b0ad3369f9e3bc9f03bc6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.3 MB (1296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ef176d155013b441d3aa61066b961412df315989dafee3b72f9ba5dd31538`  
		Last Modified: Tue, 07 Jan 2020 02:58:44 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcc35189da5025b89745e7680b1bcdb34cdf9f51d54e3e0b46fff097d0b34ae`  
		Last Modified: Tue, 07 Jan 2020 02:58:45 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afc1770bdcd5ce4d9bdd3587987b09053f042cd48c8f5810cfcaa87a16b5a9`  
		Last Modified: Tue, 07 Jan 2020 02:59:47 GMT  
		Size: 2.5 MB (2534060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0666fa958bfd6c9ef2328395485e37db84aacc6ecd4d17e31a1d295896b57de4`  
		Last Modified: Sat, 25 Jan 2020 03:16:08 GMT  
		Size: 61.0 MB (61021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c3832c067fe681b3dcf02c0178bc3bcb49bb7a656323c54de44664d81ecc3`  
		Last Modified: Sat, 25 Jan 2020 03:16:00 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:6c2dea6b181f65d669cd93ed3528823ad6e7c0c2140ff489ea485ad4339bc3b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195708230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca154e81c746b1401a3a68110b0600c1c2948a0bcbf4064ca3ccf6d17f645b0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:16:09 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 02:16:12 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 02:16:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 02:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 02:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 02:19:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 02:20:03 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:44:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:51:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:52:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:52:01 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 09:52:02 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 09:52:02 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 09:52:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 09:52:05 GMT
ENV REDMINE_VERSION=4.0.6
# Sun, 02 Feb 2020 09:52:06 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Sun, 02 Feb 2020 09:52:10 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 09:58:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:58:22 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 09:58:22 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 09:58:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:58:25 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 09:58:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd05ffdd7888092a6ef03be377963c297edec0344ce762bb6b3e1e2f114b94`  
		Last Modified: Sun, 02 Feb 2020 03:16:40 GMT  
		Size: 20.7 MB (20712712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e99c39d252f8cf22fae4749b2764aec83374848c63b8546989494f7f7a1cd2`  
		Last Modified: Sun, 02 Feb 2020 03:16:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff532b6c7852f386bab467c7b3f4b83b928ea314de236796805380d538c9717`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0debc39d343e6e3774b7272d41bc3baba5a731a248e516631a84c1a159f8e92`  
		Last Modified: Sun, 02 Feb 2020 10:08:31 GMT  
		Size: 76.0 MB (76036784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad080b035428964df5b926dd10100e90e780aba975a158a431d3981e83c258b8`  
		Last Modified: Sun, 02 Feb 2020 10:08:04 GMT  
		Size: 1.3 MB (1254160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9727bc7a8173e4995f60fae2c0648c1cb27901cb17032ad9158742d2802b6515`  
		Last Modified: Sun, 02 Feb 2020 10:08:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd97e49c236fbff5f8e9ddea74499d2220bd7243c51337af425617f8a7dd7ae`  
		Last Modified: Sun, 02 Feb 2020 10:08:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea72640d58690c2a87f00a90e7227a898f083e23da7c935365625fed397ce753`  
		Last Modified: Sun, 02 Feb 2020 10:08:03 GMT  
		Size: 2.5 MB (2534555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7020374fdf35ade6f5496677da7317db93a9a3e8c281ee32fecbbc5655f43a1`  
		Last Modified: Sun, 02 Feb 2020 10:08:20 GMT  
		Size: 60.0 MB (60009770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bf767d92dd343de578ca08df993171a406b4a73d327094036a50f3bcb4d694`  
		Last Modified: Sun, 02 Feb 2020 10:08:01 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:84e0082a8946b18b8a34f107cfe5db7e46786d57088f43e6ebcb81481d9c3105
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.1 MB (189145233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff12a514617deb29d9b7894230353c672a0d2618e104c13611f6749a6ebedc3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 21:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 21:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:22:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:12:51 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:39:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:40:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:40:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:41:00 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:41:01 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:41:02 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:41:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:46:42 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 03:46:43 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 03:46:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:17:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:17:26 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:17:28 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:17:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:17:31 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:17:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4c32e3c622deadf3234025d30c88895c18ae7eac94288d4e42f903c4a72f5`  
		Last Modified: Sat, 28 Dec 2019 22:13:25 GMT  
		Size: 20.6 MB (20620161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe49bcffa8c82983470bbf0074d2412dacbf1f325bcc2ffb85fddcbda7c7da8`  
		Last Modified: Tue, 07 Jan 2020 03:17:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67711a5ad765c81e93b31a6b9e1b763d7d8448315399ea1765bf97971567bfcb`  
		Last Modified: Tue, 07 Jan 2020 03:59:01 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d74eecc06d13134c138c9df69b88fae2a875703f36a0fb2fd26e740242128b`  
		Last Modified: Tue, 07 Jan 2020 03:59:24 GMT  
		Size: 72.4 MB (72371109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13558994cbeb5acd84e3d5cbd289b63aa49eb00c519c44df85c8eb739e1aecdc`  
		Last Modified: Tue, 07 Jan 2020 03:59:01 GMT  
		Size: 1.2 MB (1243608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0071ee240d8a61e07f23310aaa0abd958805870c68cc9a980486c0af09abd8de`  
		Last Modified: Tue, 07 Jan 2020 03:58:59 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4a08ec220f99917007502db7459ff7d23e8e699418f7728948b9785f8ad389`  
		Last Modified: Tue, 07 Jan 2020 03:58:59 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7e0dc0053822770819d959cac7513a859d9618ae56b44f8d33b3f5b2df4f1`  
		Last Modified: Tue, 07 Jan 2020 03:59:37 GMT  
		Size: 2.5 MB (2534562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56bea2c3f7dc0f05c65f36eb41cc724793bb19fcbfd13f4de34e0d35fd2b79a`  
		Last Modified: Sat, 25 Jan 2020 02:25:20 GMT  
		Size: 59.8 MB (59824791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266253a21b99fe0d3d23e179e7ddfec3b95b8dda403ed1eac5f0097285f07018`  
		Last Modified: Sat, 25 Jan 2020 02:25:07 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:29805161783705424b4dcab0ae5edc8ac7ab0b3059cfbad706fcfa364bfa76d0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201862015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e04f14bc7141eef4cef7a4f285b7c6b0b2fc0d371b55afc8003b19e8d3aed50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 22:28:49 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 22:28:50 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 22:28:51 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 22:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 22:32:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:41:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:41:14 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:06:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:07:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:08:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:08:35 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:08:38 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:08:40 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:08:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:16:20 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 03:16:21 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 03:16:28 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:47:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:47:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:47:22 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:47:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:47:25 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:47:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc7342d754a238156ddfd7ee18001a3862d29761cdf787ceb41e05bfde38061`  
		Last Modified: Sat, 28 Dec 2019 23:23:41 GMT  
		Size: 21.3 MB (21281931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1828050bdff9d08ad357e12a1bd0639c7818f955a59966e76a48d90c55ccc2`  
		Last Modified: Tue, 07 Jan 2020 02:45:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec8c6749d85258e801554c4c6b4d94f96e6ca4909194be6fc4aa78f0ba7caf`  
		Last Modified: Tue, 07 Jan 2020 03:31:11 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7616f60ca94ba9dd9d5ec4a4672df90a8f21683b3f5e363ecbb6c56cd57b34f`  
		Last Modified: Tue, 07 Jan 2020 03:31:38 GMT  
		Size: 78.8 MB (78781946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed90e7447acdd79b625fff5e37d6b9567b24b0ec16826357c12a1f1047c0e96a`  
		Last Modified: Tue, 07 Jan 2020 03:31:11 GMT  
		Size: 1.2 MB (1228684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9cb5aa81f92922c768a7f7f77d66adc87edf01e2ce3986835401c20d683c11`  
		Last Modified: Tue, 07 Jan 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe15bb660b67ad397ff5dced96f6c5a667bc63dd0d23a82b5d30347018e9c15f`  
		Last Modified: Tue, 07 Jan 2020 03:31:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb9da5aaab24a2becc2b052f105f1d4d9a237cab2fb743aa0b7f9e9a711b15f`  
		Last Modified: Tue, 07 Jan 2020 03:31:50 GMT  
		Size: 2.5 MB (2534554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4362f4a0f03489b544ce29238d811dcc3801bd192f83b6c88957bfeecbd606d`  
		Last Modified: Sat, 25 Jan 2020 02:54:06 GMT  
		Size: 60.9 MB (60934991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ccd781ca61cb091446e9a63bfbb137fd3c4660bddc3c34723fdbb9b5293660`  
		Last Modified: Sat, 25 Jan 2020 02:53:55 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; 386

```console
$ docker pull redmine@sha256:61632704ec4195eb295f59e96babd0c6c68bf01e92ba9b7464dff117bf0ef920
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.4 MB (211364575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:455db6c7f5a95dd44f30ed172088458b04e5e071a0d9889a4152c4664be2aecb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 15:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 15:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:48:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:39:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:39:08 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:00:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:01:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:01:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:01:34 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:01:34 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:01:34 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:01:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:04:48 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 03:04:49 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 03:04:52 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:52:19 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:52:19 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:52:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:52:19 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:52:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b12042d352b3390a1d5c085213ccee7f26bee56d8a1a3fb0a76e80159a411c`  
		Last Modified: Sat, 28 Dec 2019 16:44:44 GMT  
		Size: 20.9 MB (20885521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c53ce40fd432336a5365d519861a9d64c7cf858412dd402f939e5f6cb0ed3f`  
		Last Modified: Tue, 07 Jan 2020 02:41:40 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b71e9da85871d84768b7e4ee95650087a03f4db095955f62e526335b0c09aa4`  
		Last Modified: Tue, 07 Jan 2020 03:11:10 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3ccb3b9a12325f66d08313505167fa8d7a46ab42c2e89625e485c5ac43ca78`  
		Last Modified: Tue, 07 Jan 2020 03:11:33 GMT  
		Size: 81.6 MB (81574872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8085aa370c294355492d62d20997a91dce32290fb39f7ff46d2ea9f79c9cac7`  
		Last Modified: Tue, 07 Jan 2020 03:11:09 GMT  
		Size: 1.3 MB (1261083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca155252736682989c07106e5bb0eeaaf8b2372c1366aa1cdc83c0575ff1a54`  
		Last Modified: Tue, 07 Jan 2020 03:11:08 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b530bf833967827e0f2848925236be5bb8b6284da960ded962768f10853d79`  
		Last Modified: Tue, 07 Jan 2020 03:11:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2d9c5e5ea62422bf45c92473bc5a3da00f61b8c50620eb2d3498e6b0a3b55a`  
		Last Modified: Tue, 07 Jan 2020 03:11:41 GMT  
		Size: 2.5 MB (2534064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb2e3e0905f7e8ac5605108b481bd97079ff392563587780f2b52e1ee08db8`  
		Last Modified: Sat, 25 Jan 2020 01:56:04 GMT  
		Size: 60.2 MB (60151606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22292d58b737b0eb389913964b4c87c79b5626b5e3c2a012159294905266bb2d`  
		Last Modified: Sat, 25 Jan 2020 01:55:54 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:26abf6cd909df7ba26291cf53721ebcdf21bd2cbebfef007d60416f72aea39fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.4 MB (217435396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbca00bfdb96a5cb5bf0820448072a00e862a95d159bf4617d63d45b216eddcf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 04:44:05 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 04:44:07 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 04:44:10 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 04:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 04:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:18:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:18:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:56:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:57:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:57:19 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:57:25 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:57:31 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:57:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:08:01 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 03:08:03 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 03:08:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:19:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:19:10 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:19:13 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:19:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:19:17 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8219d68aec763d8d91942869b8dd9ef7233da0ba814028c00dce26b61b1ec`  
		Last Modified: Sat, 28 Dec 2019 05:29:59 GMT  
		Size: 22.0 MB (21968340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88418e7313544081130ec82f1125b007f6673672ed6fe3f2815a8bc0836d834d`  
		Last Modified: Tue, 07 Jan 2020 02:27:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811e39d17ef5178d803832537e4b94505620908b40d2ece5c639ebc74bb249c`  
		Last Modified: Tue, 07 Jan 2020 03:29:32 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759f2cb97aba0fe1a2f1053949514cc564ab7e2cfc06feb29ff83f1a25204a75`  
		Last Modified: Tue, 07 Jan 2020 03:30:06 GMT  
		Size: 86.8 MB (86837114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6f7850a6e18d809176a36601f044b1e81f00e83669c91e047608f68e15fe76`  
		Last Modified: Tue, 07 Jan 2020 03:29:32 GMT  
		Size: 1.2 MB (1218315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6322666aa095fbbcc93f7c9b4120792fc53d3d10e016d2f5b886ebaf9a71dd`  
		Last Modified: Tue, 07 Jan 2020 03:29:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff21de5e70292bac1732e4d68af3d870e59b1973fe11a6f7f5f8e2584d35433`  
		Last Modified: Tue, 07 Jan 2020 03:29:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633b566a1dbe8eeef0d0b5c4732d6ac66eda4587e3b21599312cd29761361e8b`  
		Last Modified: Tue, 07 Jan 2020 03:30:31 GMT  
		Size: 2.5 MB (2534555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bd43dd78125c27b355d6ef5106766f825e7aaaa21c17785fa492a92fb73ea2`  
		Last Modified: Sat, 25 Jan 2020 03:29:50 GMT  
		Size: 61.7 MB (61666141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186806885b22dcb37bee5f4ea9dc9520e06f18b227f801f7db8c50e51febd58b`  
		Last Modified: Sat, 25 Jan 2020 03:29:40 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; s390x

```console
$ docker pull redmine@sha256:cbf070b34f864e9c96515dfa45421eaa20238ef10162705f9822d124da8cd1f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.2 MB (201200831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b645759a5ba2c2f260e05766ef5dcd1734dcf2951d74bed1cbaa1bab9997ff66`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_MAJOR=2.6
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 01 Feb 2020 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:36:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:36:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:36:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:24:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:28:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:29:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:29:08 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:29:08 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:29:08 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:29:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:29:09 GMT
ENV REDMINE_VERSION=4.0.6
# Sun, 02 Feb 2020 03:29:09 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Sun, 02 Feb 2020 03:29:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:31:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:31:46 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:31:47 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:31:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:31:47 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:31:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f50ba1593f8ab66d1deaf12e190c35ecfea96815beda37efe10f1246f342b`  
		Last Modified: Sat, 01 Feb 2020 22:57:18 GMT  
		Size: 21.6 MB (21592569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8a5d1fd225888733445fbc5a03464b232ab7c659a3bf619e93c5670a0ca594`  
		Last Modified: Sat, 01 Feb 2020 22:57:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6b52758f305e2a6eca340f3801ffcd699d9f9863ebfe870573fbea05f125b`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1fac4ff5cafcd8c72e5f5c2b0ad9b65c0da0b68abc477c04f5a694df30d7c3`  
		Last Modified: Sun, 02 Feb 2020 03:35:46 GMT  
		Size: 77.9 MB (77938026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff38b0dcb3bbc5f2f4a3d6db1ff6ae6e4fec958a96bed443120d073beeb3cca`  
		Last Modified: Sun, 02 Feb 2020 03:35:34 GMT  
		Size: 1.3 MB (1283142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfc8a9f51c523c1393ad678485fc7c27af0973daadb7a4b898403c00a470c1c`  
		Last Modified: Sun, 02 Feb 2020 03:35:32 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48652af6bf6cc23d74f44d8dac9310630f1e54ce1970a50e76b9b08e969d36e3`  
		Last Modified: Sun, 02 Feb 2020 03:35:48 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e7113be31cd9d1c3b63a00e3042d6f6990a6f7abfd9153a63665f70c0f57f6`  
		Last Modified: Sun, 02 Feb 2020 03:35:48 GMT  
		Size: 2.5 MB (2534555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1af23fc8a237407ee124dbcb2eb6f80a2c91d2a5940c439c678cdfef1dbd90`  
		Last Modified: Sun, 02 Feb 2020 03:35:39 GMT  
		Size: 61.3 MB (61346659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388d58b291fa3d29f6414a4697d6ff544204e41efc77488f71a129e007e9c1f0`  
		Last Modified: Sun, 02 Feb 2020 03:36:03 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.6`

```console
$ docker pull redmine@sha256:2cbe178da1bc5ab4da1b7ec5b69ba5f55367dbc3cdfdb85a8144d76b356312c5
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

### `redmine:4.0.6` - linux; amd64

```console
$ docker pull redmine@sha256:69a57b170618bc5ea16a564655faa4a675f8f3c13e37bc875efd8c01e146d120
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.1 MB (206096278 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1fe698f6b99ddbae61bb0bb6332fc61814fe13a0bb00652cc461ead815a8659`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:42:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:42:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:42:40 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:42:40 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:42:40 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:42:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:47:32 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 02:47:32 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 02:47:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:07:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:07:05 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:07:05 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:07:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:07:05 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:07:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c8c66f527fafb06b837048b77a717c5c453f36789591051417d3730279253a`  
		Last Modified: Tue, 07 Jan 2020 02:59:05 GMT  
		Size: 80.2 MB (80161685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e48374f11ea16d535dab197d7559592d994ed6d63b0ad3369f9e3bc9f03bc6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.3 MB (1296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ef176d155013b441d3aa61066b961412df315989dafee3b72f9ba5dd31538`  
		Last Modified: Tue, 07 Jan 2020 02:58:44 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcc35189da5025b89745e7680b1bcdb34cdf9f51d54e3e0b46fff097d0b34ae`  
		Last Modified: Tue, 07 Jan 2020 02:58:45 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afc1770bdcd5ce4d9bdd3587987b09053f042cd48c8f5810cfcaa87a16b5a9`  
		Last Modified: Tue, 07 Jan 2020 02:59:47 GMT  
		Size: 2.5 MB (2534060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0666fa958bfd6c9ef2328395485e37db84aacc6ecd4d17e31a1d295896b57de4`  
		Last Modified: Sat, 25 Jan 2020 03:16:08 GMT  
		Size: 61.0 MB (61021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c3832c067fe681b3dcf02c0178bc3bcb49bb7a656323c54de44664d81ecc3`  
		Last Modified: Sat, 25 Jan 2020 03:16:00 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.6` - linux; arm variant v5

```console
$ docker pull redmine@sha256:6c2dea6b181f65d669cd93ed3528823ad6e7c0c2140ff489ea485ad4339bc3b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195708230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bca154e81c746b1401a3a68110b0600c1c2948a0bcbf4064ca3ccf6d17f645b0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:16:09 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 02:16:12 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 02:16:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 02:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 02:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 02:19:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 02:20:03 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:44:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:51:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:52:00 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:52:01 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 09:52:02 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 09:52:02 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 09:52:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 09:52:05 GMT
ENV REDMINE_VERSION=4.0.6
# Sun, 02 Feb 2020 09:52:06 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Sun, 02 Feb 2020 09:52:10 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 09:58:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:58:22 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 09:58:22 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 09:58:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:58:25 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 09:58:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd05ffdd7888092a6ef03be377963c297edec0344ce762bb6b3e1e2f114b94`  
		Last Modified: Sun, 02 Feb 2020 03:16:40 GMT  
		Size: 20.7 MB (20712712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e99c39d252f8cf22fae4749b2764aec83374848c63b8546989494f7f7a1cd2`  
		Last Modified: Sun, 02 Feb 2020 03:16:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff532b6c7852f386bab467c7b3f4b83b928ea314de236796805380d538c9717`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0debc39d343e6e3774b7272d41bc3baba5a731a248e516631a84c1a159f8e92`  
		Last Modified: Sun, 02 Feb 2020 10:08:31 GMT  
		Size: 76.0 MB (76036784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad080b035428964df5b926dd10100e90e780aba975a158a431d3981e83c258b8`  
		Last Modified: Sun, 02 Feb 2020 10:08:04 GMT  
		Size: 1.3 MB (1254160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9727bc7a8173e4995f60fae2c0648c1cb27901cb17032ad9158742d2802b6515`  
		Last Modified: Sun, 02 Feb 2020 10:08:02 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd97e49c236fbff5f8e9ddea74499d2220bd7243c51337af425617f8a7dd7ae`  
		Last Modified: Sun, 02 Feb 2020 10:08:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea72640d58690c2a87f00a90e7227a898f083e23da7c935365625fed397ce753`  
		Last Modified: Sun, 02 Feb 2020 10:08:03 GMT  
		Size: 2.5 MB (2534555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7020374fdf35ade6f5496677da7317db93a9a3e8c281ee32fecbbc5655f43a1`  
		Last Modified: Sun, 02 Feb 2020 10:08:20 GMT  
		Size: 60.0 MB (60009770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bf767d92dd343de578ca08df993171a406b4a73d327094036a50f3bcb4d694`  
		Last Modified: Sun, 02 Feb 2020 10:08:01 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.6` - linux; arm variant v7

```console
$ docker pull redmine@sha256:84e0082a8946b18b8a34f107cfe5db7e46786d57088f43e6ebcb81481d9c3105
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.1 MB (189145233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff12a514617deb29d9b7894230353c672a0d2618e104c13611f6749a6ebedc3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 21:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 21:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:22:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:12:51 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:39:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:40:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:40:59 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:41:00 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:41:01 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:41:02 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:41:04 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:46:42 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 03:46:43 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 03:46:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:17:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:17:26 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:17:28 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:17:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:17:31 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:17:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4c32e3c622deadf3234025d30c88895c18ae7eac94288d4e42f903c4a72f5`  
		Last Modified: Sat, 28 Dec 2019 22:13:25 GMT  
		Size: 20.6 MB (20620161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe49bcffa8c82983470bbf0074d2412dacbf1f325bcc2ffb85fddcbda7c7da8`  
		Last Modified: Tue, 07 Jan 2020 03:17:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67711a5ad765c81e93b31a6b9e1b763d7d8448315399ea1765bf97971567bfcb`  
		Last Modified: Tue, 07 Jan 2020 03:59:01 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d74eecc06d13134c138c9df69b88fae2a875703f36a0fb2fd26e740242128b`  
		Last Modified: Tue, 07 Jan 2020 03:59:24 GMT  
		Size: 72.4 MB (72371109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13558994cbeb5acd84e3d5cbd289b63aa49eb00c519c44df85c8eb739e1aecdc`  
		Last Modified: Tue, 07 Jan 2020 03:59:01 GMT  
		Size: 1.2 MB (1243608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0071ee240d8a61e07f23310aaa0abd958805870c68cc9a980486c0af09abd8de`  
		Last Modified: Tue, 07 Jan 2020 03:58:59 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4a08ec220f99917007502db7459ff7d23e8e699418f7728948b9785f8ad389`  
		Last Modified: Tue, 07 Jan 2020 03:58:59 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7e0dc0053822770819d959cac7513a859d9618ae56b44f8d33b3f5b2df4f1`  
		Last Modified: Tue, 07 Jan 2020 03:59:37 GMT  
		Size: 2.5 MB (2534562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56bea2c3f7dc0f05c65f36eb41cc724793bb19fcbfd13f4de34e0d35fd2b79a`  
		Last Modified: Sat, 25 Jan 2020 02:25:20 GMT  
		Size: 59.8 MB (59824791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266253a21b99fe0d3d23e179e7ddfec3b95b8dda403ed1eac5f0097285f07018`  
		Last Modified: Sat, 25 Jan 2020 02:25:07 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.6` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:29805161783705424b4dcab0ae5edc8ac7ab0b3059cfbad706fcfa364bfa76d0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.9 MB (201862015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e04f14bc7141eef4cef7a4f285b7c6b0b2fc0d371b55afc8003b19e8d3aed50`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 22:28:49 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 22:28:50 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 22:28:51 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 22:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 22:32:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:41:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:41:14 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:06:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:07:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:08:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:08:35 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:08:38 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:08:40 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:08:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:16:20 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 03:16:21 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 03:16:28 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:47:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:47:21 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:47:22 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:47:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:47:25 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:47:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc7342d754a238156ddfd7ee18001a3862d29761cdf787ceb41e05bfde38061`  
		Last Modified: Sat, 28 Dec 2019 23:23:41 GMT  
		Size: 21.3 MB (21281931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1828050bdff9d08ad357e12a1bd0639c7818f955a59966e76a48d90c55ccc2`  
		Last Modified: Tue, 07 Jan 2020 02:45:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec8c6749d85258e801554c4c6b4d94f96e6ca4909194be6fc4aa78f0ba7caf`  
		Last Modified: Tue, 07 Jan 2020 03:31:11 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7616f60ca94ba9dd9d5ec4a4672df90a8f21683b3f5e363ecbb6c56cd57b34f`  
		Last Modified: Tue, 07 Jan 2020 03:31:38 GMT  
		Size: 78.8 MB (78781946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed90e7447acdd79b625fff5e37d6b9567b24b0ec16826357c12a1f1047c0e96a`  
		Last Modified: Tue, 07 Jan 2020 03:31:11 GMT  
		Size: 1.2 MB (1228684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9cb5aa81f92922c768a7f7f77d66adc87edf01e2ce3986835401c20d683c11`  
		Last Modified: Tue, 07 Jan 2020 03:31:08 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe15bb660b67ad397ff5dced96f6c5a667bc63dd0d23a82b5d30347018e9c15f`  
		Last Modified: Tue, 07 Jan 2020 03:31:08 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb9da5aaab24a2becc2b052f105f1d4d9a237cab2fb743aa0b7f9e9a711b15f`  
		Last Modified: Tue, 07 Jan 2020 03:31:50 GMT  
		Size: 2.5 MB (2534554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4362f4a0f03489b544ce29238d811dcc3801bd192f83b6c88957bfeecbd606d`  
		Last Modified: Sat, 25 Jan 2020 02:54:06 GMT  
		Size: 60.9 MB (60934991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ccd781ca61cb091446e9a63bfbb137fd3c4660bddc3c34723fdbb9b5293660`  
		Last Modified: Sat, 25 Jan 2020 02:53:55 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.6` - linux; 386

```console
$ docker pull redmine@sha256:61632704ec4195eb295f59e96babd0c6c68bf01e92ba9b7464dff117bf0ef920
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.4 MB (211364575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:455db6c7f5a95dd44f30ed172088458b04e5e071a0d9889a4152c4664be2aecb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 15:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 15:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:48:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:39:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:39:08 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:00:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 03:01:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 03:01:34 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 03:01:34 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 03:01:34 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 03:01:34 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 03:01:35 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:04:48 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 03:04:49 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 03:04:52 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:52:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:52:19 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:52:19 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:52:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:52:19 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:52:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b12042d352b3390a1d5c085213ccee7f26bee56d8a1a3fb0a76e80159a411c`  
		Last Modified: Sat, 28 Dec 2019 16:44:44 GMT  
		Size: 20.9 MB (20885521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c53ce40fd432336a5365d519861a9d64c7cf858412dd402f939e5f6cb0ed3f`  
		Last Modified: Tue, 07 Jan 2020 02:41:40 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b71e9da85871d84768b7e4ee95650087a03f4db095955f62e526335b0c09aa4`  
		Last Modified: Tue, 07 Jan 2020 03:11:10 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3ccb3b9a12325f66d08313505167fa8d7a46ab42c2e89625e485c5ac43ca78`  
		Last Modified: Tue, 07 Jan 2020 03:11:33 GMT  
		Size: 81.6 MB (81574872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8085aa370c294355492d62d20997a91dce32290fb39f7ff46d2ea9f79c9cac7`  
		Last Modified: Tue, 07 Jan 2020 03:11:09 GMT  
		Size: 1.3 MB (1261083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca155252736682989c07106e5bb0eeaaf8b2372c1366aa1cdc83c0575ff1a54`  
		Last Modified: Tue, 07 Jan 2020 03:11:08 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b530bf833967827e0f2848925236be5bb8b6284da960ded962768f10853d79`  
		Last Modified: Tue, 07 Jan 2020 03:11:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2d9c5e5ea62422bf45c92473bc5a3da00f61b8c50620eb2d3498e6b0a3b55a`  
		Last Modified: Tue, 07 Jan 2020 03:11:41 GMT  
		Size: 2.5 MB (2534064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdb2e3e0905f7e8ac5605108b481bd97079ff392563587780f2b52e1ee08db8`  
		Last Modified: Sat, 25 Jan 2020 01:56:04 GMT  
		Size: 60.2 MB (60151606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22292d58b737b0eb389913964b4c87c79b5626b5e3c2a012159294905266bb2d`  
		Last Modified: Sat, 25 Jan 2020 01:55:54 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.6` - linux; ppc64le

```console
$ docker pull redmine@sha256:26abf6cd909df7ba26291cf53721ebcdf21bd2cbebfef007d60416f72aea39fa
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.4 MB (217435396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbca00bfdb96a5cb5bf0820448072a00e862a95d159bf4617d63d45b216eddcf`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 04:44:05 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 04:44:07 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 04:44:10 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 04:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 04:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:18:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:18:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:56:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:57:12 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:57:19 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:57:25 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:57:31 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:57:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 03:08:01 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 03:08:03 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 03:08:11 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:19:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:19:10 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:19:13 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:19:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:19:17 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:19:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8219d68aec763d8d91942869b8dd9ef7233da0ba814028c00dce26b61b1ec`  
		Last Modified: Sat, 28 Dec 2019 05:29:59 GMT  
		Size: 22.0 MB (21968340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88418e7313544081130ec82f1125b007f6673672ed6fe3f2815a8bc0836d834d`  
		Last Modified: Tue, 07 Jan 2020 02:27:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811e39d17ef5178d803832537e4b94505620908b40d2ece5c639ebc74bb249c`  
		Last Modified: Tue, 07 Jan 2020 03:29:32 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759f2cb97aba0fe1a2f1053949514cc564ab7e2cfc06feb29ff83f1a25204a75`  
		Last Modified: Tue, 07 Jan 2020 03:30:06 GMT  
		Size: 86.8 MB (86837114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6f7850a6e18d809176a36601f044b1e81f00e83669c91e047608f68e15fe76`  
		Last Modified: Tue, 07 Jan 2020 03:29:32 GMT  
		Size: 1.2 MB (1218315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6322666aa095fbbcc93f7c9b4120792fc53d3d10e016d2f5b886ebaf9a71dd`  
		Last Modified: Tue, 07 Jan 2020 03:29:26 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff21de5e70292bac1732e4d68af3d870e59b1973fe11a6f7f5f8e2584d35433`  
		Last Modified: Tue, 07 Jan 2020 03:29:26 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633b566a1dbe8eeef0d0b5c4732d6ac66eda4587e3b21599312cd29761361e8b`  
		Last Modified: Tue, 07 Jan 2020 03:30:31 GMT  
		Size: 2.5 MB (2534555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44bd43dd78125c27b355d6ef5106766f825e7aaaa21c17785fa492a92fb73ea2`  
		Last Modified: Sat, 25 Jan 2020 03:29:50 GMT  
		Size: 61.7 MB (61666141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186806885b22dcb37bee5f4ea9dc9520e06f18b227f801f7db8c50e51febd58b`  
		Last Modified: Sat, 25 Jan 2020 03:29:40 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.6` - linux; s390x

```console
$ docker pull redmine@sha256:cbf070b34f864e9c96515dfa45421eaa20238ef10162705f9822d124da8cd1f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **201.2 MB (201200831 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b645759a5ba2c2f260e05766ef5dcd1734dcf2951d74bed1cbaa1bab9997ff66`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_MAJOR=2.6
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 01 Feb 2020 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:36:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:36:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:36:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:24:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:28:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:29:08 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:29:08 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:29:08 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:29:08 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:29:09 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:29:09 GMT
ENV REDMINE_VERSION=4.0.6
# Sun, 02 Feb 2020 03:29:09 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Sun, 02 Feb 2020 03:29:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:31:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:31:46 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:31:47 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:31:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:31:47 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:31:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f50ba1593f8ab66d1deaf12e190c35ecfea96815beda37efe10f1246f342b`  
		Last Modified: Sat, 01 Feb 2020 22:57:18 GMT  
		Size: 21.6 MB (21592569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8a5d1fd225888733445fbc5a03464b232ab7c659a3bf619e93c5670a0ca594`  
		Last Modified: Sat, 01 Feb 2020 22:57:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6b52758f305e2a6eca340f3801ffcd699d9f9863ebfe870573fbea05f125b`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1fac4ff5cafcd8c72e5f5c2b0ad9b65c0da0b68abc477c04f5a694df30d7c3`  
		Last Modified: Sun, 02 Feb 2020 03:35:46 GMT  
		Size: 77.9 MB (77938026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff38b0dcb3bbc5f2f4a3d6db1ff6ae6e4fec958a96bed443120d073beeb3cca`  
		Last Modified: Sun, 02 Feb 2020 03:35:34 GMT  
		Size: 1.3 MB (1283142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfc8a9f51c523c1393ad678485fc7c27af0973daadb7a4b898403c00a470c1c`  
		Last Modified: Sun, 02 Feb 2020 03:35:32 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48652af6bf6cc23d74f44d8dac9310630f1e54ce1970a50e76b9b08e969d36e3`  
		Last Modified: Sun, 02 Feb 2020 03:35:48 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36e7113be31cd9d1c3b63a00e3042d6f6990a6f7abfd9153a63665f70c0f57f6`  
		Last Modified: Sun, 02 Feb 2020 03:35:48 GMT  
		Size: 2.5 MB (2534555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a1af23fc8a237407ee124dbcb2eb6f80a2c91d2a5940c439c678cdfef1dbd90`  
		Last Modified: Sun, 02 Feb 2020 03:35:39 GMT  
		Size: 61.3 MB (61346659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388d58b291fa3d29f6414a4697d6ff544204e41efc77488f71a129e007e9c1f0`  
		Last Modified: Sun, 02 Feb 2020 03:36:03 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.6-alpine`

```console
$ docker pull redmine@sha256:a979e29cbfde5de17798d4e9b91d5a2a77bc84a9b9c3f4e4835b7c963166cff0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0.6-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:8f90d09cf079ff5be64d694722794ab5df0c046e03fffa3af8c832bb6cbf8245
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.1 MB (154087478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcdba488d0c766cd6832878ee15e5c07d7b7d5df81f499df81bcf689c2e9cf4d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_MAJOR=2.6
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_VERSION=2.6.5
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Thu, 23 Jan 2020 22:54:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 22:54:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 22:55:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 22:55:00 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:20:34 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 24 Jan 2020 15:20:41 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Fri, 24 Jan 2020 15:20:41 GMT
ENV RAILS_ENV=production
# Fri, 24 Jan 2020 15:20:42 GMT
WORKDIR /usr/src/redmine
# Fri, 24 Jan 2020 15:20:42 GMT
ENV HOME=/home/redmine
# Fri, 24 Jan 2020 15:20:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 24 Jan 2020 15:22:38 GMT
ENV REDMINE_VERSION=4.0.6
# Fri, 24 Jan 2020 15:22:38 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Fri, 24 Jan 2020 15:22:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:09:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:09:32 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:09:32 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:09:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:09:32 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:09:33 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058dc40fe23d25b2a6b8b9a31a6064c2eac5b373f52d5acb6d9219394f18a6c`  
		Last Modified: Thu, 23 Jan 2020 23:08:01 GMT  
		Size: 22.1 MB (22078401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabe7657d0e85ffedf267cb47d1b5a01f8da1f182f429defe848b0cdb2233ab1`  
		Last Modified: Thu, 23 Jan 2020 23:07:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a8cf67746eef043d81238dcc09e82c7404ac11ded1b543a0d44ef4b43b1f6f`  
		Last Modified: Fri, 24 Jan 2020 15:26:52 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec375945f2a0726e842b7cbcd0e44f464791dd670c87ba5c94886a64624e61f7`  
		Last Modified: Fri, 24 Jan 2020 15:27:14 GMT  
		Size: 65.7 MB (65727287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fc0e569dec0c9540830c542087692271d164dda41eb6fd4236c8214f080eb2`  
		Last Modified: Fri, 24 Jan 2020 15:26:51 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ae2ddcba63d2890fcefdbbd31d9646ee5e5428bb2c37578422be8f60b9363f`  
		Last Modified: Fri, 24 Jan 2020 15:26:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5298d654e31d6672b6f7171281f78f6536b027b9dc7e209b2d0f3589d8cbda2`  
		Last Modified: Fri, 24 Jan 2020 15:27:23 GMT  
		Size: 2.5 MB (2535813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841e92874997bbd5b01af23711a5d3dfc55accce652163e641d73a8647f36be7`  
		Last Modified: Sat, 25 Jan 2020 03:16:29 GMT  
		Size: 59.9 MB (59924857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2825ca0d048103b819a2f778649e5c4592cfc7f7030da727b2249617a19b0b0`  
		Last Modified: Sat, 25 Jan 2020 03:16:20 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.6-passenger`

```console
$ docker pull redmine@sha256:ae58f02e9ffc7d8b55e18c123671c04951a42698ac44c0c557c81a39bbc048f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0.6-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:86e01bcde8e88bc380069f044106df6fe3b1b002e29813e3380a7560830ee8a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230954117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0f54d730d080c9abc92f61978646f59a4bec8fb5ad4e03f6cfebb48bfacde1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:42:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:42:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:42:40 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:42:40 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:42:40 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:42:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:47:32 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 02:47:32 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 02:47:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:07:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:07:05 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:07:05 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:07:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:07:05 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:07:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:07:16 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:07:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:07:35 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:07:35 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:07:35 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c8c66f527fafb06b837048b77a717c5c453f36789591051417d3730279253a`  
		Last Modified: Tue, 07 Jan 2020 02:59:05 GMT  
		Size: 80.2 MB (80161685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e48374f11ea16d535dab197d7559592d994ed6d63b0ad3369f9e3bc9f03bc6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.3 MB (1296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ef176d155013b441d3aa61066b961412df315989dafee3b72f9ba5dd31538`  
		Last Modified: Tue, 07 Jan 2020 02:58:44 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcc35189da5025b89745e7680b1bcdb34cdf9f51d54e3e0b46fff097d0b34ae`  
		Last Modified: Tue, 07 Jan 2020 02:58:45 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afc1770bdcd5ce4d9bdd3587987b09053f042cd48c8f5810cfcaa87a16b5a9`  
		Last Modified: Tue, 07 Jan 2020 02:59:47 GMT  
		Size: 2.5 MB (2534060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0666fa958bfd6c9ef2328395485e37db84aacc6ecd4d17e31a1d295896b57de4`  
		Last Modified: Sat, 25 Jan 2020 03:16:08 GMT  
		Size: 61.0 MB (61021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c3832c067fe681b3dcf02c0178bc3bcb49bb7a656323c54de44664d81ecc3`  
		Last Modified: Sat, 25 Jan 2020 03:16:00 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929314698c561d64e84c74c8f52d07293f04cfb11f839998ff6b19e37acf1d8e`  
		Last Modified: Sat, 25 Jan 2020 03:16:15 GMT  
		Size: 19.9 MB (19939988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6331d530dd0b73f990a9f02e9df6246e4341fd2ed8b650ae18010ca57ab1c`  
		Last Modified: Sat, 25 Jan 2020 03:16:13 GMT  
		Size: 4.9 MB (4917851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-alpine`

```console
$ docker pull redmine@sha256:a979e29cbfde5de17798d4e9b91d5a2a77bc84a9b9c3f4e4835b7c963166cff0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:8f90d09cf079ff5be64d694722794ab5df0c046e03fffa3af8c832bb6cbf8245
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.1 MB (154087478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcdba488d0c766cd6832878ee15e5c07d7b7d5df81f499df81bcf689c2e9cf4d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_MAJOR=2.6
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_VERSION=2.6.5
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Thu, 23 Jan 2020 22:54:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 22:54:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 22:55:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 22:55:00 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:20:34 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Fri, 24 Jan 2020 15:20:41 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Fri, 24 Jan 2020 15:20:41 GMT
ENV RAILS_ENV=production
# Fri, 24 Jan 2020 15:20:42 GMT
WORKDIR /usr/src/redmine
# Fri, 24 Jan 2020 15:20:42 GMT
ENV HOME=/home/redmine
# Fri, 24 Jan 2020 15:20:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 24 Jan 2020 15:22:38 GMT
ENV REDMINE_VERSION=4.0.6
# Fri, 24 Jan 2020 15:22:38 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Fri, 24 Jan 2020 15:22:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:09:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:09:32 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:09:32 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:09:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:09:32 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:09:33 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058dc40fe23d25b2a6b8b9a31a6064c2eac5b373f52d5acb6d9219394f18a6c`  
		Last Modified: Thu, 23 Jan 2020 23:08:01 GMT  
		Size: 22.1 MB (22078401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabe7657d0e85ffedf267cb47d1b5a01f8da1f182f429defe848b0cdb2233ab1`  
		Last Modified: Thu, 23 Jan 2020 23:07:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a8cf67746eef043d81238dcc09e82c7404ac11ded1b543a0d44ef4b43b1f6f`  
		Last Modified: Fri, 24 Jan 2020 15:26:52 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec375945f2a0726e842b7cbcd0e44f464791dd670c87ba5c94886a64624e61f7`  
		Last Modified: Fri, 24 Jan 2020 15:27:14 GMT  
		Size: 65.7 MB (65727287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37fc0e569dec0c9540830c542087692271d164dda41eb6fd4236c8214f080eb2`  
		Last Modified: Fri, 24 Jan 2020 15:26:51 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ae2ddcba63d2890fcefdbbd31d9646ee5e5428bb2c37578422be8f60b9363f`  
		Last Modified: Fri, 24 Jan 2020 15:26:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5298d654e31d6672b6f7171281f78f6536b027b9dc7e209b2d0f3589d8cbda2`  
		Last Modified: Fri, 24 Jan 2020 15:27:23 GMT  
		Size: 2.5 MB (2535813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841e92874997bbd5b01af23711a5d3dfc55accce652163e641d73a8647f36be7`  
		Last Modified: Sat, 25 Jan 2020 03:16:29 GMT  
		Size: 59.9 MB (59924857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2825ca0d048103b819a2f778649e5c4592cfc7f7030da727b2249617a19b0b0`  
		Last Modified: Sat, 25 Jan 2020 03:16:20 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-passenger`

```console
$ docker pull redmine@sha256:ae58f02e9ffc7d8b55e18c123671c04951a42698ac44c0c557c81a39bbc048f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:86e01bcde8e88bc380069f044106df6fe3b1b002e29813e3380a7560830ee8a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230954117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a0f54d730d080c9abc92f61978646f59a4bec8fb5ad4e03f6cfebb48bfacde1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 07 Jan 2020 02:42:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jan 2020 02:42:39 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 07 Jan 2020 02:42:40 GMT
ENV RAILS_ENV=production
# Tue, 07 Jan 2020 02:42:40 GMT
WORKDIR /usr/src/redmine
# Tue, 07 Jan 2020 02:42:40 GMT
ENV HOME=/home/redmine
# Tue, 07 Jan 2020 02:42:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 07 Jan 2020 02:47:32 GMT
ENV REDMINE_VERSION=4.0.6
# Tue, 07 Jan 2020 02:47:32 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Tue, 07 Jan 2020 02:47:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:07:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:07:05 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:07:05 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:07:05 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:07:05 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:07:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:07:16 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:07:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:07:35 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:07:35 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:07:35 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c8c66f527fafb06b837048b77a717c5c453f36789591051417d3730279253a`  
		Last Modified: Tue, 07 Jan 2020 02:59:05 GMT  
		Size: 80.2 MB (80161685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0e48374f11ea16d535dab197d7559592d994ed6d63b0ad3369f9e3bc9f03bc6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.3 MB (1296495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030ef176d155013b441d3aa61066b961412df315989dafee3b72f9ba5dd31538`  
		Last Modified: Tue, 07 Jan 2020 02:58:44 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfcc35189da5025b89745e7680b1bcdb34cdf9f51d54e3e0b46fff097d0b34ae`  
		Last Modified: Tue, 07 Jan 2020 02:58:45 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4afc1770bdcd5ce4d9bdd3587987b09053f042cd48c8f5810cfcaa87a16b5a9`  
		Last Modified: Tue, 07 Jan 2020 02:59:47 GMT  
		Size: 2.5 MB (2534060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0666fa958bfd6c9ef2328395485e37db84aacc6ecd4d17e31a1d295896b57de4`  
		Last Modified: Sat, 25 Jan 2020 03:16:08 GMT  
		Size: 61.0 MB (61021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1c3832c067fe681b3dcf02c0178bc3bcb49bb7a656323c54de44664d81ecc3`  
		Last Modified: Sat, 25 Jan 2020 03:16:00 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929314698c561d64e84c74c8f52d07293f04cfb11f839998ff6b19e37acf1d8e`  
		Last Modified: Sat, 25 Jan 2020 03:16:15 GMT  
		Size: 19.9 MB (19939988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb6331d530dd0b73f990a9f02e9df6246e4341fd2ed8b650ae18010ca57ab1c`  
		Last Modified: Sat, 25 Jan 2020 03:16:13 GMT  
		Size: 4.9 MB (4917851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1`

```console
$ docker pull redmine@sha256:31dc2573b1c77945e98ad71e3ba671f787b3f402abf9d00af0b5062d3e0176bb
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
$ docker pull redmine@sha256:b020b824c4bc29851cb807d079249567fba38953a183e5c6c156843fe044fd5e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.4 MB (215374935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe885543d5387f35a4aa3a2a65968c4ace488cb67a6c40677407a4aec17c9ed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:59:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:59:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:59:53 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:59:53 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:59:53 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:59:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:59:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:01:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:01:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:01:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:01:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:01:50 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:01:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20875f0e3d3802e64f74c9b1930e47473aa008ac1e3e2f5449ad290a85ab57`  
		Last Modified: Sat, 25 Jan 2020 03:15:23 GMT  
		Size: 93.1 MB (93059371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309a0bcae95c3ed0d1e34a294ec279f52939042fe32ae9ce3795d64ac30b93b`  
		Last Modified: Sat, 25 Jan 2020 03:15:04 GMT  
		Size: 1.3 MB (1307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce465b077ee104502ac0d3bb56ee609f8466b52df3019fc8e0eb9910c16c2475`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fd3dbd195628a62fb6e32bdc5cb84a1ad44500433876fab465c8e8d1d23c9`  
		Last Modified: Sat, 25 Jan 2020 03:15:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc96f26d91b45b07346a0a2064741540002911ab51b1c01a69d794eb672085c`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.7 MB (2735388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d61a0e145c858537c040f69d6811589e5d6e96ac59368d19b40ec966610ba7`  
		Last Modified: Sat, 25 Jan 2020 03:15:11 GMT  
		Size: 57.2 MB (57190428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5794504759a01ead1a31eb3f4b6799addca73aaca089b237498d8b773f0400f4`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:d81487b3c1ad872dcf937922c70e1b33aa56ba4ce5190286fa2d86d8adeedc35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204856480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb08d7d0f07498236e41fdcf83db177fea39c1c452b01cf798acd1a6878621b8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:16:09 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 02:16:12 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 02:16:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 02:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 02:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 02:19:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 02:20:03 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:44:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:46:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:46:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:46:22 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 09:46:22 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 09:46:23 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 09:46:25 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 09:46:25 GMT
ENV REDMINE_VERSION=4.1.0
# Sun, 02 Feb 2020 09:46:26 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sun, 02 Feb 2020 09:46:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 09:50:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:50:23 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 09:50:23 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 09:50:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:50:25 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 09:50:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd05ffdd7888092a6ef03be377963c297edec0344ce762bb6b3e1e2f114b94`  
		Last Modified: Sun, 02 Feb 2020 03:16:40 GMT  
		Size: 20.7 MB (20712712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e99c39d252f8cf22fae4749b2764aec83374848c63b8546989494f7f7a1cd2`  
		Last Modified: Sun, 02 Feb 2020 03:16:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff532b6c7852f386bab467c7b3f4b83b928ea314de236796805380d538c9717`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2386bd4b4f50f1d8f93b32303170d0866887841332213e58a371ca1bb7a20589`  
		Last Modified: Sun, 02 Feb 2020 10:07:52 GMT  
		Size: 88.7 MB (88656018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3116bbee905e3f17958856da579a4d33255abeddc081a9673f7e7751b098ebe`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.3 MB (1265374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a450151953d1dd4bd9521617998e60400bbde5af211dc4477b78be4b3f12675b`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98603c054417f4f97943b58f87a4064bff0a6fdcc842f801c987da619b29ff3b`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23326958468d4e64c292656ee80e58902c0ffdb4d9dd0ebe0f3ab5264ce8d22`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 2.7 MB (2735847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdb53308614fca2cb01c7b7851bffaab106d45dee36ec93f25b881241ff56a0`  
		Last Modified: Sun, 02 Feb 2020 10:07:31 GMT  
		Size: 56.3 MB (56326279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2affc3b6a6c7eac6ca68be7e12a92c5998344deee6abc0a859b5698bb25dfdcc`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:fd859aecbff1334ede20c1579bbabb5bd45bf7594547561cdc1d27758507b025
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197890698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5ca2f6d8a5214b523a543ba010bc02d222e1415eb4513f339f22da0cb06cba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 21:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 21:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:22:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:12:51 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:39:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:06:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:07:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:07:02 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:07:03 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:07:04 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:07:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:07:07 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:07:08 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:07:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:10:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:10:55 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:10:56 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:10:58 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:10:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4c32e3c622deadf3234025d30c88895c18ae7eac94288d4e42f903c4a72f5`  
		Last Modified: Sat, 28 Dec 2019 22:13:25 GMT  
		Size: 20.6 MB (20620161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe49bcffa8c82983470bbf0074d2412dacbf1f325bcc2ffb85fddcbda7c7da8`  
		Last Modified: Tue, 07 Jan 2020 03:17:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67711a5ad765c81e93b31a6b9e1b763d7d8448315399ea1765bf97971567bfcb`  
		Last Modified: Tue, 07 Jan 2020 03:59:01 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22df051691cc30d921b9d70b85efd5cd46a51c055fb7a885fe2ae9ef34f1965`  
		Last Modified: Sat, 25 Jan 2020 02:24:54 GMT  
		Size: 84.7 MB (84708006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d2540796d803b25bed6e74b93432545aae43cc0a48e7fbf6093c5e6823b0a4`  
		Last Modified: Sat, 25 Jan 2020 02:24:26 GMT  
		Size: 1.3 MB (1258219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a8c6a15e107f7bf7271010e2bdf9b48e58f6598901bd1971275252da7f8ae`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7837a0650c1e2b2d0636d7b4235bda5767e5c67ef97f5a6747edd98b03f63c7`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d2ce28f760155459539026440cf179c5489575000c97eae858f42d01c9568c`  
		Last Modified: Sat, 25 Jan 2020 02:24:25 GMT  
		Size: 2.7 MB (2735850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646d541d0d57a917412aac2e133006b795fac0f438acd943f02709948cba90e6`  
		Last Modified: Sat, 25 Jan 2020 02:24:38 GMT  
		Size: 56.0 MB (56017460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714489a49c6e19537c912f14ef35b3218572e68b1c1f851192d706acad806bed`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:58f2624f1a316fd842c70194c733401281f3850fa6fa8f1340c7d2b9198cfb57
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.1 MB (211120176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1aa59e95791a967e02ca12ecfd915f8009cbca478126af0f52e55f8759923c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 22:28:49 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 22:28:50 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 22:28:51 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 22:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 22:32:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:41:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:41:14 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:06:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:34:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:35:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:35:13 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:35:15 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:35:15 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:35:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:35:18 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:35:20 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:35:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:40:02 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:40:03 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:40:12 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:40:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc7342d754a238156ddfd7ee18001a3862d29761cdf787ceb41e05bfde38061`  
		Last Modified: Sat, 28 Dec 2019 23:23:41 GMT  
		Size: 21.3 MB (21281931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1828050bdff9d08ad357e12a1bd0639c7818f955a59966e76a48d90c55ccc2`  
		Last Modified: Tue, 07 Jan 2020 02:45:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec8c6749d85258e801554c4c6b4d94f96e6ca4909194be6fc4aa78f0ba7caf`  
		Last Modified: Tue, 07 Jan 2020 03:31:11 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79ff809afa32d5baba46f2f7bde80a0ab57dc15374657c246cdb0db778b6c4d`  
		Last Modified: Sat, 25 Jan 2020 02:53:40 GMT  
		Size: 91.6 MB (91645815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee31ede564e2642f141b9f0353eb8a17b5738e42230d2666c77f0057e3c71ed`  
		Last Modified: Sat, 25 Jan 2020 02:53:12 GMT  
		Size: 1.2 MB (1242951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538e9d155ef665df153038fe494404878b140304e7a7358d79c50f3c06cdd0f1`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24c8d492a9f691c39c85e79b35ccf567e2430697d78dabeb9149cb9789d5d1a`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20410b8776eb35b945d7702f61a7e2c0d2f768b9d7e3919c8153e5f1f45b0370`  
		Last Modified: Sat, 25 Jan 2020 02:53:11 GMT  
		Size: 2.7 MB (2735848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17724b15809fcdf62e3624dc2b6d2500d0531bf9fa6a801f1dad1ad4a5e70b87`  
		Last Modified: Sat, 25 Jan 2020 02:53:23 GMT  
		Size: 57.1 MB (57113718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8820389aab406aeaa971c6a195fb163be61f4b7d5b3ff008a5f4f41897e285`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; 386

```console
$ docker pull redmine@sha256:f700874a4b5a04b0de5054424a487980540e0cbc11dd8880c89437153e718aba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.8 MB (220831119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13bb3cef0fc5bee43a02ef2d01a7bc6cc73c13e1ecb2668ea53c6064fce16f77`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 15:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 15:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:48:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:39:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:39:08 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:00:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 01:47:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 01:47:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:47:29 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 01:47:29 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 01:47:29 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 01:47:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 01:47:30 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 01:47:31 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 01:47:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:49:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:49:23 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:49:23 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:49:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:49:24 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:49:24 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b12042d352b3390a1d5c085213ccee7f26bee56d8a1a3fb0a76e80159a411c`  
		Last Modified: Sat, 28 Dec 2019 16:44:44 GMT  
		Size: 20.9 MB (20885521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c53ce40fd432336a5365d519861a9d64c7cf858412dd402f939e5f6cb0ed3f`  
		Last Modified: Tue, 07 Jan 2020 02:41:40 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b71e9da85871d84768b7e4ee95650087a03f4db095955f62e526335b0c09aa4`  
		Last Modified: Tue, 07 Jan 2020 03:11:10 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5f640023220debb54aa59008a23084703fc0537fc624f8ceab4d90009b5f0a`  
		Last Modified: Sat, 25 Jan 2020 01:55:48 GMT  
		Size: 94.7 MB (94693229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c958a54bf64e77189cf05b4486d2756c03a8c3d2dfaa0623e2a09c1a5109e0b`  
		Last Modified: Sat, 25 Jan 2020 01:55:24 GMT  
		Size: 1.3 MB (1275383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00731a6396a0f584e04f340d4a49c149951c796ca229ed740930499b1a882c`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a2a82b5a98ff43706a5284dab0afd502f20a49c7a2a08ed51f40683ac458d`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d5165755570cce25c28f06dd103a1d73386b43cf12f92cd6ca898131ae5663`  
		Last Modified: Sat, 25 Jan 2020 01:55:24 GMT  
		Size: 2.7 MB (2735383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe1b8246e4d2cefa8623bb1ec59f0b3ab47bb321632de09d3ea2b875a984bc8`  
		Last Modified: Sat, 25 Jan 2020 01:55:33 GMT  
		Size: 56.3 MB (56284173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a398c5eaf1193a79396d5800707f6528d558924b2c597e2767da34ae511bb6`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:f08f037717dc3721e961cb0907ae97ac8328ba24fe1bfa1b059ed270e9cfe715
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227173333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2bb12560bf4f88050034a40821bb893c2d88a2a3c4abd85702087a17761c09`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 04:44:05 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 04:44:07 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 04:44:10 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 04:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 04:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:18:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:18:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 03:06:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:06:20 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 03:06:23 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 03:06:27 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 03:06:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 03:06:35 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 03:06:37 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 03:06:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:10:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:10:41 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:10:42 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:10:47 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:10:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8219d68aec763d8d91942869b8dd9ef7233da0ba814028c00dce26b61b1ec`  
		Last Modified: Sat, 28 Dec 2019 05:29:59 GMT  
		Size: 22.0 MB (21968340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88418e7313544081130ec82f1125b007f6673672ed6fe3f2815a8bc0836d834d`  
		Last Modified: Tue, 07 Jan 2020 02:27:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811e39d17ef5178d803832537e4b94505620908b40d2ece5c639ebc74bb249c`  
		Last Modified: Tue, 07 Jan 2020 03:29:32 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fdc2fee5bcdaa20790472eb3b3e6a238cee4c14ea8503eaf556e87582caf2b`  
		Last Modified: Sat, 25 Jan 2020 03:29:20 GMT  
		Size: 100.3 MB (100282383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37063699c1769c556fcd7e961dae12c108451947f10a4381c9312fb86a65bb6b`  
		Last Modified: Sat, 25 Jan 2020 03:28:58 GMT  
		Size: 1.2 MB (1232203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77c914aba14ea81411aae5a9d0b596dbebda443ecb800ce8e717f0c782a367b`  
		Last Modified: Sat, 25 Jan 2020 03:28:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b47a8358f9f444669f85d1a5f3690a1d8e37b0c91e7a827ceb0b4937b251c5`  
		Last Modified: Sat, 25 Jan 2020 03:28:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b553f520f8f427b541d300f1b7cd485adf7ee67d7046a370c78d993aaebff1a7`  
		Last Modified: Sat, 25 Jan 2020 03:28:56 GMT  
		Size: 2.7 MB (2735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1492d8aabeb5a9c29d1c9c848723748f59b53365c4e70c0d9c897c329ca329`  
		Last Modified: Sat, 25 Jan 2020 03:29:06 GMT  
		Size: 57.7 MB (57743620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556573964a0bd208b3e595f68ab9d500f1405000b822b06641efaa11e9820c7b`  
		Last Modified: Sat, 25 Jan 2020 03:28:54 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; s390x

```console
$ docker pull redmine@sha256:ab1568d6b226e18d614f69224ab5082f76ab6c3c459575b451c0b43a044e4c88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210607230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e81bbd4d53db9fe58b1f99028cbe990f74848ac4052582c07576953e60742dc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_MAJOR=2.6
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 01 Feb 2020 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:36:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:36:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:36:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:24:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:25:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:25:35 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:25:36 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:25:36 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:25:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:25:37 GMT
ENV REDMINE_VERSION=4.1.0
# Sun, 02 Feb 2020 03:25:37 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sun, 02 Feb 2020 03:25:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:28:15 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:28:15 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:28:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:28:16 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:28:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f50ba1593f8ab66d1deaf12e190c35ecfea96815beda37efe10f1246f342b`  
		Last Modified: Sat, 01 Feb 2020 22:57:18 GMT  
		Size: 21.6 MB (21592569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8a5d1fd225888733445fbc5a03464b232ab7c659a3bf619e93c5670a0ca594`  
		Last Modified: Sat, 01 Feb 2020 22:57:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6b52758f305e2a6eca340f3801ffcd699d9f9863ebfe870573fbea05f125b`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c2d954e677f77134627d444d4526d3dd757e20731a3db791ee045bd3ff5`  
		Last Modified: Sun, 02 Feb 2020 03:35:13 GMT  
		Size: 90.8 MB (90810821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4b03bbe680823684e8167d23322040275fc82bb40b38251bd1aca1d9759997`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.3 MB (1297549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6a56833da980d550b03c0656e63d42b60190fa8f5b743d0efd1679e03cb5ea`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6743cd35c07b27ae19792d6c94243798a11247fa7a5f0fd8d63ec5fec7f8c8`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0844cdbf926f537d20bc1295376495cb2b126746d549e3cc88402e855e2f92`  
		Last Modified: Sun, 02 Feb 2020 03:34:58 GMT  
		Size: 2.7 MB (2735858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a0c8052dd4f2d2e8e61136ca875e5667f9fdd869156f21339a352533be465b`  
		Last Modified: Sun, 02 Feb 2020 03:35:25 GMT  
		Size: 57.7 MB (57664549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b47a626d921e859c5def90095c9624aa612e063bcacdce5bb5485574308e28`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.0`

```console
$ docker pull redmine@sha256:31dc2573b1c77945e98ad71e3ba671f787b3f402abf9d00af0b5062d3e0176bb
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

### `redmine:4.1.0` - linux; amd64

```console
$ docker pull redmine@sha256:b020b824c4bc29851cb807d079249567fba38953a183e5c6c156843fe044fd5e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.4 MB (215374935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe885543d5387f35a4aa3a2a65968c4ace488cb67a6c40677407a4aec17c9ed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:59:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:59:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:59:53 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:59:53 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:59:53 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:59:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:59:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:01:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:01:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:01:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:01:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:01:50 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:01:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20875f0e3d3802e64f74c9b1930e47473aa008ac1e3e2f5449ad290a85ab57`  
		Last Modified: Sat, 25 Jan 2020 03:15:23 GMT  
		Size: 93.1 MB (93059371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309a0bcae95c3ed0d1e34a294ec279f52939042fe32ae9ce3795d64ac30b93b`  
		Last Modified: Sat, 25 Jan 2020 03:15:04 GMT  
		Size: 1.3 MB (1307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce465b077ee104502ac0d3bb56ee609f8466b52df3019fc8e0eb9910c16c2475`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fd3dbd195628a62fb6e32bdc5cb84a1ad44500433876fab465c8e8d1d23c9`  
		Last Modified: Sat, 25 Jan 2020 03:15:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc96f26d91b45b07346a0a2064741540002911ab51b1c01a69d794eb672085c`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.7 MB (2735388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d61a0e145c858537c040f69d6811589e5d6e96ac59368d19b40ec966610ba7`  
		Last Modified: Sat, 25 Jan 2020 03:15:11 GMT  
		Size: 57.2 MB (57190428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5794504759a01ead1a31eb3f4b6799addca73aaca089b237498d8b773f0400f4`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:d81487b3c1ad872dcf937922c70e1b33aa56ba4ce5190286fa2d86d8adeedc35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204856480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb08d7d0f07498236e41fdcf83db177fea39c1c452b01cf798acd1a6878621b8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:16:09 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 02:16:12 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 02:16:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 02:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 02:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 02:19:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 02:20:03 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:44:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:46:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:46:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:46:22 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 09:46:22 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 09:46:23 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 09:46:25 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 09:46:25 GMT
ENV REDMINE_VERSION=4.1.0
# Sun, 02 Feb 2020 09:46:26 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sun, 02 Feb 2020 09:46:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 09:50:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:50:23 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 09:50:23 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 09:50:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:50:25 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 09:50:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd05ffdd7888092a6ef03be377963c297edec0344ce762bb6b3e1e2f114b94`  
		Last Modified: Sun, 02 Feb 2020 03:16:40 GMT  
		Size: 20.7 MB (20712712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e99c39d252f8cf22fae4749b2764aec83374848c63b8546989494f7f7a1cd2`  
		Last Modified: Sun, 02 Feb 2020 03:16:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff532b6c7852f386bab467c7b3f4b83b928ea314de236796805380d538c9717`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2386bd4b4f50f1d8f93b32303170d0866887841332213e58a371ca1bb7a20589`  
		Last Modified: Sun, 02 Feb 2020 10:07:52 GMT  
		Size: 88.7 MB (88656018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3116bbee905e3f17958856da579a4d33255abeddc081a9673f7e7751b098ebe`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.3 MB (1265374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a450151953d1dd4bd9521617998e60400bbde5af211dc4477b78be4b3f12675b`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98603c054417f4f97943b58f87a4064bff0a6fdcc842f801c987da619b29ff3b`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23326958468d4e64c292656ee80e58902c0ffdb4d9dd0ebe0f3ab5264ce8d22`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 2.7 MB (2735847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdb53308614fca2cb01c7b7851bffaab106d45dee36ec93f25b881241ff56a0`  
		Last Modified: Sun, 02 Feb 2020 10:07:31 GMT  
		Size: 56.3 MB (56326279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2affc3b6a6c7eac6ca68be7e12a92c5998344deee6abc0a859b5698bb25dfdcc`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:fd859aecbff1334ede20c1579bbabb5bd45bf7594547561cdc1d27758507b025
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197890698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5ca2f6d8a5214b523a543ba010bc02d222e1415eb4513f339f22da0cb06cba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 21:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 21:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:22:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:12:51 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:39:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:06:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:07:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:07:02 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:07:03 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:07:04 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:07:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:07:07 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:07:08 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:07:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:10:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:10:55 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:10:56 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:10:58 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:10:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4c32e3c622deadf3234025d30c88895c18ae7eac94288d4e42f903c4a72f5`  
		Last Modified: Sat, 28 Dec 2019 22:13:25 GMT  
		Size: 20.6 MB (20620161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe49bcffa8c82983470bbf0074d2412dacbf1f325bcc2ffb85fddcbda7c7da8`  
		Last Modified: Tue, 07 Jan 2020 03:17:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67711a5ad765c81e93b31a6b9e1b763d7d8448315399ea1765bf97971567bfcb`  
		Last Modified: Tue, 07 Jan 2020 03:59:01 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22df051691cc30d921b9d70b85efd5cd46a51c055fb7a885fe2ae9ef34f1965`  
		Last Modified: Sat, 25 Jan 2020 02:24:54 GMT  
		Size: 84.7 MB (84708006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d2540796d803b25bed6e74b93432545aae43cc0a48e7fbf6093c5e6823b0a4`  
		Last Modified: Sat, 25 Jan 2020 02:24:26 GMT  
		Size: 1.3 MB (1258219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a8c6a15e107f7bf7271010e2bdf9b48e58f6598901bd1971275252da7f8ae`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7837a0650c1e2b2d0636d7b4235bda5767e5c67ef97f5a6747edd98b03f63c7`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d2ce28f760155459539026440cf179c5489575000c97eae858f42d01c9568c`  
		Last Modified: Sat, 25 Jan 2020 02:24:25 GMT  
		Size: 2.7 MB (2735850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646d541d0d57a917412aac2e133006b795fac0f438acd943f02709948cba90e6`  
		Last Modified: Sat, 25 Jan 2020 02:24:38 GMT  
		Size: 56.0 MB (56017460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714489a49c6e19537c912f14ef35b3218572e68b1c1f851192d706acad806bed`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:58f2624f1a316fd842c70194c733401281f3850fa6fa8f1340c7d2b9198cfb57
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.1 MB (211120176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1aa59e95791a967e02ca12ecfd915f8009cbca478126af0f52e55f8759923c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 22:28:49 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 22:28:50 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 22:28:51 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 22:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 22:32:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:41:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:41:14 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:06:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:34:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:35:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:35:13 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:35:15 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:35:15 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:35:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:35:18 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:35:20 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:35:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:40:02 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:40:03 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:40:12 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:40:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc7342d754a238156ddfd7ee18001a3862d29761cdf787ceb41e05bfde38061`  
		Last Modified: Sat, 28 Dec 2019 23:23:41 GMT  
		Size: 21.3 MB (21281931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1828050bdff9d08ad357e12a1bd0639c7818f955a59966e76a48d90c55ccc2`  
		Last Modified: Tue, 07 Jan 2020 02:45:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec8c6749d85258e801554c4c6b4d94f96e6ca4909194be6fc4aa78f0ba7caf`  
		Last Modified: Tue, 07 Jan 2020 03:31:11 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79ff809afa32d5baba46f2f7bde80a0ab57dc15374657c246cdb0db778b6c4d`  
		Last Modified: Sat, 25 Jan 2020 02:53:40 GMT  
		Size: 91.6 MB (91645815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee31ede564e2642f141b9f0353eb8a17b5738e42230d2666c77f0057e3c71ed`  
		Last Modified: Sat, 25 Jan 2020 02:53:12 GMT  
		Size: 1.2 MB (1242951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538e9d155ef665df153038fe494404878b140304e7a7358d79c50f3c06cdd0f1`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24c8d492a9f691c39c85e79b35ccf567e2430697d78dabeb9149cb9789d5d1a`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20410b8776eb35b945d7702f61a7e2c0d2f768b9d7e3919c8153e5f1f45b0370`  
		Last Modified: Sat, 25 Jan 2020 02:53:11 GMT  
		Size: 2.7 MB (2735848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17724b15809fcdf62e3624dc2b6d2500d0531bf9fa6a801f1dad1ad4a5e70b87`  
		Last Modified: Sat, 25 Jan 2020 02:53:23 GMT  
		Size: 57.1 MB (57113718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8820389aab406aeaa971c6a195fb163be61f4b7d5b3ff008a5f4f41897e285`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.0` - linux; 386

```console
$ docker pull redmine@sha256:f700874a4b5a04b0de5054424a487980540e0cbc11dd8880c89437153e718aba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.8 MB (220831119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13bb3cef0fc5bee43a02ef2d01a7bc6cc73c13e1ecb2668ea53c6064fce16f77`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 15:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 15:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:48:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:39:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:39:08 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:00:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 01:47:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 01:47:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:47:29 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 01:47:29 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 01:47:29 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 01:47:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 01:47:30 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 01:47:31 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 01:47:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:49:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:49:23 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:49:23 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:49:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:49:24 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:49:24 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b12042d352b3390a1d5c085213ccee7f26bee56d8a1a3fb0a76e80159a411c`  
		Last Modified: Sat, 28 Dec 2019 16:44:44 GMT  
		Size: 20.9 MB (20885521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c53ce40fd432336a5365d519861a9d64c7cf858412dd402f939e5f6cb0ed3f`  
		Last Modified: Tue, 07 Jan 2020 02:41:40 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b71e9da85871d84768b7e4ee95650087a03f4db095955f62e526335b0c09aa4`  
		Last Modified: Tue, 07 Jan 2020 03:11:10 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5f640023220debb54aa59008a23084703fc0537fc624f8ceab4d90009b5f0a`  
		Last Modified: Sat, 25 Jan 2020 01:55:48 GMT  
		Size: 94.7 MB (94693229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c958a54bf64e77189cf05b4486d2756c03a8c3d2dfaa0623e2a09c1a5109e0b`  
		Last Modified: Sat, 25 Jan 2020 01:55:24 GMT  
		Size: 1.3 MB (1275383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00731a6396a0f584e04f340d4a49c149951c796ca229ed740930499b1a882c`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a2a82b5a98ff43706a5284dab0afd502f20a49c7a2a08ed51f40683ac458d`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d5165755570cce25c28f06dd103a1d73386b43cf12f92cd6ca898131ae5663`  
		Last Modified: Sat, 25 Jan 2020 01:55:24 GMT  
		Size: 2.7 MB (2735383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe1b8246e4d2cefa8623bb1ec59f0b3ab47bb321632de09d3ea2b875a984bc8`  
		Last Modified: Sat, 25 Jan 2020 01:55:33 GMT  
		Size: 56.3 MB (56284173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a398c5eaf1193a79396d5800707f6528d558924b2c597e2767da34ae511bb6`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:f08f037717dc3721e961cb0907ae97ac8328ba24fe1bfa1b059ed270e9cfe715
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227173333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2bb12560bf4f88050034a40821bb893c2d88a2a3c4abd85702087a17761c09`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 04:44:05 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 04:44:07 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 04:44:10 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 04:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 04:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:18:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:18:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 03:06:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:06:20 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 03:06:23 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 03:06:27 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 03:06:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 03:06:35 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 03:06:37 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 03:06:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:10:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:10:41 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:10:42 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:10:47 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:10:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8219d68aec763d8d91942869b8dd9ef7233da0ba814028c00dce26b61b1ec`  
		Last Modified: Sat, 28 Dec 2019 05:29:59 GMT  
		Size: 22.0 MB (21968340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88418e7313544081130ec82f1125b007f6673672ed6fe3f2815a8bc0836d834d`  
		Last Modified: Tue, 07 Jan 2020 02:27:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811e39d17ef5178d803832537e4b94505620908b40d2ece5c639ebc74bb249c`  
		Last Modified: Tue, 07 Jan 2020 03:29:32 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fdc2fee5bcdaa20790472eb3b3e6a238cee4c14ea8503eaf556e87582caf2b`  
		Last Modified: Sat, 25 Jan 2020 03:29:20 GMT  
		Size: 100.3 MB (100282383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37063699c1769c556fcd7e961dae12c108451947f10a4381c9312fb86a65bb6b`  
		Last Modified: Sat, 25 Jan 2020 03:28:58 GMT  
		Size: 1.2 MB (1232203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77c914aba14ea81411aae5a9d0b596dbebda443ecb800ce8e717f0c782a367b`  
		Last Modified: Sat, 25 Jan 2020 03:28:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b47a8358f9f444669f85d1a5f3690a1d8e37b0c91e7a827ceb0b4937b251c5`  
		Last Modified: Sat, 25 Jan 2020 03:28:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b553f520f8f427b541d300f1b7cd485adf7ee67d7046a370c78d993aaebff1a7`  
		Last Modified: Sat, 25 Jan 2020 03:28:56 GMT  
		Size: 2.7 MB (2735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1492d8aabeb5a9c29d1c9c848723748f59b53365c4e70c0d9c897c329ca329`  
		Last Modified: Sat, 25 Jan 2020 03:29:06 GMT  
		Size: 57.7 MB (57743620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556573964a0bd208b3e595f68ab9d500f1405000b822b06641efaa11e9820c7b`  
		Last Modified: Sat, 25 Jan 2020 03:28:54 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.0` - linux; s390x

```console
$ docker pull redmine@sha256:ab1568d6b226e18d614f69224ab5082f76ab6c3c459575b451c0b43a044e4c88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210607230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e81bbd4d53db9fe58b1f99028cbe990f74848ac4052582c07576953e60742dc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_MAJOR=2.6
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 01 Feb 2020 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:36:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:36:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:36:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:24:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:25:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:25:35 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:25:36 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:25:36 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:25:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:25:37 GMT
ENV REDMINE_VERSION=4.1.0
# Sun, 02 Feb 2020 03:25:37 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sun, 02 Feb 2020 03:25:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:28:15 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:28:15 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:28:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:28:16 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:28:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f50ba1593f8ab66d1deaf12e190c35ecfea96815beda37efe10f1246f342b`  
		Last Modified: Sat, 01 Feb 2020 22:57:18 GMT  
		Size: 21.6 MB (21592569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8a5d1fd225888733445fbc5a03464b232ab7c659a3bf619e93c5670a0ca594`  
		Last Modified: Sat, 01 Feb 2020 22:57:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6b52758f305e2a6eca340f3801ffcd699d9f9863ebfe870573fbea05f125b`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c2d954e677f77134627d444d4526d3dd757e20731a3db791ee045bd3ff5`  
		Last Modified: Sun, 02 Feb 2020 03:35:13 GMT  
		Size: 90.8 MB (90810821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4b03bbe680823684e8167d23322040275fc82bb40b38251bd1aca1d9759997`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.3 MB (1297549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6a56833da980d550b03c0656e63d42b60190fa8f5b743d0efd1679e03cb5ea`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6743cd35c07b27ae19792d6c94243798a11247fa7a5f0fd8d63ec5fec7f8c8`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0844cdbf926f537d20bc1295376495cb2b126746d549e3cc88402e855e2f92`  
		Last Modified: Sun, 02 Feb 2020 03:34:58 GMT  
		Size: 2.7 MB (2735858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a0c8052dd4f2d2e8e61136ca875e5667f9fdd869156f21339a352533be465b`  
		Last Modified: Sun, 02 Feb 2020 03:35:25 GMT  
		Size: 57.7 MB (57664549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b47a626d921e859c5def90095c9624aa612e063bcacdce5bb5485574308e28`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.0-alpine`

```console
$ docker pull redmine@sha256:4cf27b467b7efee154bf1200b03925094dcbee0d8db708c2c1ddf5587ef8a0b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1.0-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:8dca5e32e3f4f1b74e2d3b12ee4509223694f6c35c80a35b462350f530e418d8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152675939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aea4d9afbc8b24ba2b8683642b3634cb4af5a361967bf5da6fcafaa4ae3a439`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_MAJOR=2.6
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_VERSION=2.6.5
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Thu, 23 Jan 2020 22:54:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 22:54:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 22:55:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 22:55:00 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:20:34 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 25 Jan 2020 03:02:42 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 25 Jan 2020 03:02:42 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 03:02:42 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 03:02:43 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 03:02:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 03:02:43 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 03:02:44 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 03:02:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:04:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:04:24 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:04:25 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:04:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:04:25 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:04:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058dc40fe23d25b2a6b8b9a31a6064c2eac5b373f52d5acb6d9219394f18a6c`  
		Last Modified: Thu, 23 Jan 2020 23:08:01 GMT  
		Size: 22.1 MB (22078401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabe7657d0e85ffedf267cb47d1b5a01f8da1f182f429defe848b0cdb2233ab1`  
		Last Modified: Thu, 23 Jan 2020 23:07:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a8cf67746eef043d81238dcc09e82c7404ac11ded1b543a0d44ef4b43b1f6f`  
		Last Modified: Fri, 24 Jan 2020 15:26:52 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568aba8514f204b93c18b8eaa4a6a10b1dc92d352b0bfc41cdb4fd157b88d21a`  
		Last Modified: Sat, 25 Jan 2020 03:15:53 GMT  
		Size: 67.8 MB (67774141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dacea602a3aaea9db5b6718ed6f84d15bb2efed2ac2e05bef99abf6569720d1`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dec2fc3052aebbbdb9c6a1a67e059e213b5e5c7c810d9595b33c2f3f342cf2`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6ae9955e302f74f4c9316777133885c5bf958ed173d65759757c8ec5851934`  
		Last Modified: Sat, 25 Jan 2020 03:15:39 GMT  
		Size: 2.7 MB (2736232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296d0c68ebdb2f40e192360f52529db01ea6473b1fc893aced2659b3e4d102d`  
		Last Modified: Sat, 25 Jan 2020 03:15:47 GMT  
		Size: 56.3 MB (56266046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfd7ae63629d03f592f27e8117eaae2d70ee2380134b5581049703258b91339`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.0-passenger`

```console
$ docker pull redmine@sha256:ba7a9f6a40c0321efb4e23c475561ca7900e9b554dc4acc094735f7e662d4b15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:1a4b83e2c247a77f9df50853b0b68e3bc67bd981aae0a2fc71efb39124cb0a36
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240227783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4526c7d5cd953230156bb4a6db6a31bbfaa56aa6bf8bcc06f6e5371921ae60`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:59:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:59:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:59:53 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:59:53 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:59:53 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:59:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:59:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:01:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:01:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:01:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:01:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:01:50 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:01:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:02:09 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:02:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:02:28 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:02:28 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:02:28 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20875f0e3d3802e64f74c9b1930e47473aa008ac1e3e2f5449ad290a85ab57`  
		Last Modified: Sat, 25 Jan 2020 03:15:23 GMT  
		Size: 93.1 MB (93059371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309a0bcae95c3ed0d1e34a294ec279f52939042fe32ae9ce3795d64ac30b93b`  
		Last Modified: Sat, 25 Jan 2020 03:15:04 GMT  
		Size: 1.3 MB (1307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce465b077ee104502ac0d3bb56ee609f8466b52df3019fc8e0eb9910c16c2475`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fd3dbd195628a62fb6e32bdc5cb84a1ad44500433876fab465c8e8d1d23c9`  
		Last Modified: Sat, 25 Jan 2020 03:15:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc96f26d91b45b07346a0a2064741540002911ab51b1c01a69d794eb672085c`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.7 MB (2735388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d61a0e145c858537c040f69d6811589e5d6e96ac59368d19b40ec966610ba7`  
		Last Modified: Sat, 25 Jan 2020 03:15:11 GMT  
		Size: 57.2 MB (57190428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5794504759a01ead1a31eb3f4b6799addca73aaca089b237498d8b773f0400f4`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff399de53c760559fd2eee97d976fac5edfad88174424ed39eb1c80f14d2e7d`  
		Last Modified: Sat, 25 Jan 2020 03:15:33 GMT  
		Size: 19.9 MB (19935002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0411f053fc05d6fa100b4b761e3b8fd4ad0ac893351b89b722ec5c86087665a`  
		Last Modified: Sat, 25 Jan 2020 03:15:31 GMT  
		Size: 4.9 MB (4917846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-alpine`

```console
$ docker pull redmine@sha256:4cf27b467b7efee154bf1200b03925094dcbee0d8db708c2c1ddf5587ef8a0b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:8dca5e32e3f4f1b74e2d3b12ee4509223694f6c35c80a35b462350f530e418d8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152675939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aea4d9afbc8b24ba2b8683642b3634cb4af5a361967bf5da6fcafaa4ae3a439`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_MAJOR=2.6
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_VERSION=2.6.5
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Thu, 23 Jan 2020 22:54:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 22:54:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 22:55:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 22:55:00 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:20:34 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 25 Jan 2020 03:02:42 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 25 Jan 2020 03:02:42 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 03:02:42 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 03:02:43 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 03:02:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 03:02:43 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 03:02:44 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 03:02:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:04:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:04:24 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:04:25 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:04:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:04:25 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:04:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058dc40fe23d25b2a6b8b9a31a6064c2eac5b373f52d5acb6d9219394f18a6c`  
		Last Modified: Thu, 23 Jan 2020 23:08:01 GMT  
		Size: 22.1 MB (22078401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabe7657d0e85ffedf267cb47d1b5a01f8da1f182f429defe848b0cdb2233ab1`  
		Last Modified: Thu, 23 Jan 2020 23:07:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a8cf67746eef043d81238dcc09e82c7404ac11ded1b543a0d44ef4b43b1f6f`  
		Last Modified: Fri, 24 Jan 2020 15:26:52 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568aba8514f204b93c18b8eaa4a6a10b1dc92d352b0bfc41cdb4fd157b88d21a`  
		Last Modified: Sat, 25 Jan 2020 03:15:53 GMT  
		Size: 67.8 MB (67774141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dacea602a3aaea9db5b6718ed6f84d15bb2efed2ac2e05bef99abf6569720d1`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dec2fc3052aebbbdb9c6a1a67e059e213b5e5c7c810d9595b33c2f3f342cf2`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6ae9955e302f74f4c9316777133885c5bf958ed173d65759757c8ec5851934`  
		Last Modified: Sat, 25 Jan 2020 03:15:39 GMT  
		Size: 2.7 MB (2736232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296d0c68ebdb2f40e192360f52529db01ea6473b1fc893aced2659b3e4d102d`  
		Last Modified: Sat, 25 Jan 2020 03:15:47 GMT  
		Size: 56.3 MB (56266046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfd7ae63629d03f592f27e8117eaae2d70ee2380134b5581049703258b91339`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-passenger`

```console
$ docker pull redmine@sha256:ba7a9f6a40c0321efb4e23c475561ca7900e9b554dc4acc094735f7e662d4b15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:1a4b83e2c247a77f9df50853b0b68e3bc67bd981aae0a2fc71efb39124cb0a36
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240227783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4526c7d5cd953230156bb4a6db6a31bbfaa56aa6bf8bcc06f6e5371921ae60`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:59:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:59:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:59:53 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:59:53 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:59:53 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:59:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:59:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:01:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:01:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:01:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:01:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:01:50 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:01:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:02:09 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:02:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:02:28 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:02:28 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:02:28 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20875f0e3d3802e64f74c9b1930e47473aa008ac1e3e2f5449ad290a85ab57`  
		Last Modified: Sat, 25 Jan 2020 03:15:23 GMT  
		Size: 93.1 MB (93059371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309a0bcae95c3ed0d1e34a294ec279f52939042fe32ae9ce3795d64ac30b93b`  
		Last Modified: Sat, 25 Jan 2020 03:15:04 GMT  
		Size: 1.3 MB (1307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce465b077ee104502ac0d3bb56ee609f8466b52df3019fc8e0eb9910c16c2475`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fd3dbd195628a62fb6e32bdc5cb84a1ad44500433876fab465c8e8d1d23c9`  
		Last Modified: Sat, 25 Jan 2020 03:15:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc96f26d91b45b07346a0a2064741540002911ab51b1c01a69d794eb672085c`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.7 MB (2735388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d61a0e145c858537c040f69d6811589e5d6e96ac59368d19b40ec966610ba7`  
		Last Modified: Sat, 25 Jan 2020 03:15:11 GMT  
		Size: 57.2 MB (57190428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5794504759a01ead1a31eb3f4b6799addca73aaca089b237498d8b773f0400f4`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff399de53c760559fd2eee97d976fac5edfad88174424ed39eb1c80f14d2e7d`  
		Last Modified: Sat, 25 Jan 2020 03:15:33 GMT  
		Size: 19.9 MB (19935002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0411f053fc05d6fa100b4b761e3b8fd4ad0ac893351b89b722ec5c86087665a`  
		Last Modified: Sat, 25 Jan 2020 03:15:31 GMT  
		Size: 4.9 MB (4917846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:4cf27b467b7efee154bf1200b03925094dcbee0d8db708c2c1ddf5587ef8a0b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:8dca5e32e3f4f1b74e2d3b12ee4509223694f6c35c80a35b462350f530e418d8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152675939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aea4d9afbc8b24ba2b8683642b3634cb4af5a361967bf5da6fcafaa4ae3a439`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_MAJOR=2.6
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_VERSION=2.6.5
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Thu, 23 Jan 2020 22:54:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 22:54:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 22:55:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 22:55:00 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:20:34 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 25 Jan 2020 03:02:42 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 25 Jan 2020 03:02:42 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 03:02:42 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 03:02:43 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 03:02:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 03:02:43 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 03:02:44 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 03:02:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:04:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:04:24 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:04:25 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:04:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:04:25 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:04:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058dc40fe23d25b2a6b8b9a31a6064c2eac5b373f52d5acb6d9219394f18a6c`  
		Last Modified: Thu, 23 Jan 2020 23:08:01 GMT  
		Size: 22.1 MB (22078401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabe7657d0e85ffedf267cb47d1b5a01f8da1f182f429defe848b0cdb2233ab1`  
		Last Modified: Thu, 23 Jan 2020 23:07:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a8cf67746eef043d81238dcc09e82c7404ac11ded1b543a0d44ef4b43b1f6f`  
		Last Modified: Fri, 24 Jan 2020 15:26:52 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568aba8514f204b93c18b8eaa4a6a10b1dc92d352b0bfc41cdb4fd157b88d21a`  
		Last Modified: Sat, 25 Jan 2020 03:15:53 GMT  
		Size: 67.8 MB (67774141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dacea602a3aaea9db5b6718ed6f84d15bb2efed2ac2e05bef99abf6569720d1`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dec2fc3052aebbbdb9c6a1a67e059e213b5e5c7c810d9595b33c2f3f342cf2`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6ae9955e302f74f4c9316777133885c5bf958ed173d65759757c8ec5851934`  
		Last Modified: Sat, 25 Jan 2020 03:15:39 GMT  
		Size: 2.7 MB (2736232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296d0c68ebdb2f40e192360f52529db01ea6473b1fc893aced2659b3e4d102d`  
		Last Modified: Sat, 25 Jan 2020 03:15:47 GMT  
		Size: 56.3 MB (56266046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfd7ae63629d03f592f27e8117eaae2d70ee2380134b5581049703258b91339`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:ba7a9f6a40c0321efb4e23c475561ca7900e9b554dc4acc094735f7e662d4b15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:1a4b83e2c247a77f9df50853b0b68e3bc67bd981aae0a2fc71efb39124cb0a36
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240227783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4526c7d5cd953230156bb4a6db6a31bbfaa56aa6bf8bcc06f6e5371921ae60`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:59:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:59:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:59:53 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:59:53 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:59:53 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:59:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:59:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:01:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:01:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:01:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:01:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:01:50 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:01:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:02:09 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:02:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:02:28 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:02:28 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:02:28 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20875f0e3d3802e64f74c9b1930e47473aa008ac1e3e2f5449ad290a85ab57`  
		Last Modified: Sat, 25 Jan 2020 03:15:23 GMT  
		Size: 93.1 MB (93059371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309a0bcae95c3ed0d1e34a294ec279f52939042fe32ae9ce3795d64ac30b93b`  
		Last Modified: Sat, 25 Jan 2020 03:15:04 GMT  
		Size: 1.3 MB (1307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce465b077ee104502ac0d3bb56ee609f8466b52df3019fc8e0eb9910c16c2475`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fd3dbd195628a62fb6e32bdc5cb84a1ad44500433876fab465c8e8d1d23c9`  
		Last Modified: Sat, 25 Jan 2020 03:15:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc96f26d91b45b07346a0a2064741540002911ab51b1c01a69d794eb672085c`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.7 MB (2735388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d61a0e145c858537c040f69d6811589e5d6e96ac59368d19b40ec966610ba7`  
		Last Modified: Sat, 25 Jan 2020 03:15:11 GMT  
		Size: 57.2 MB (57190428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5794504759a01ead1a31eb3f4b6799addca73aaca089b237498d8b773f0400f4`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff399de53c760559fd2eee97d976fac5edfad88174424ed39eb1c80f14d2e7d`  
		Last Modified: Sat, 25 Jan 2020 03:15:33 GMT  
		Size: 19.9 MB (19935002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0411f053fc05d6fa100b4b761e3b8fd4ad0ac893351b89b722ec5c86087665a`  
		Last Modified: Sat, 25 Jan 2020 03:15:31 GMT  
		Size: 4.9 MB (4917846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:alpine`

```console
$ docker pull redmine@sha256:4cf27b467b7efee154bf1200b03925094dcbee0d8db708c2c1ddf5587ef8a0b0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:8dca5e32e3f4f1b74e2d3b12ee4509223694f6c35c80a35b462350f530e418d8
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.7 MB (152675939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0aea4d9afbc8b24ba2b8683642b3634cb4af5a361967bf5da6fcafaa4ae3a439`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 22:45:09 GMT
RUN apk add --no-cache 		gmp-dev
# Thu, 23 Jan 2020 22:45:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_MAJOR=2.6
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_VERSION=2.6.5
# Thu, 23 Jan 2020 22:51:17 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Thu, 23 Jan 2020 22:54:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps 		$runDeps 		bzip2 		ca-certificates 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	! apk --no-network list --installed 		| grep -v '^[.]ruby-rundeps' 		| grep -i ruby 	; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jan 2020 22:54:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jan 2020 22:54:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jan 2020 22:55:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jan 2020 22:55:00 GMT
CMD ["irb"]
# Fri, 24 Jan 2020 15:20:34 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Sat, 25 Jan 2020 03:02:42 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Sat, 25 Jan 2020 03:02:42 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 03:02:42 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 03:02:43 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 03:02:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 03:02:43 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 03:02:44 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 03:02:46 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:04:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		su-exec redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 25 Jan 2020 03:04:24 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:04:25 GMT
COPY file:74f57a1bf0a912dc2879462a72c1d654c2450fd1e1dad78bffaafda2974d3e97 in / 
# Sat, 25 Jan 2020 03:04:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:04:25 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:04:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b33ddc14734d2336fc9bef7d13319b166f5c65e02d4f0ea6bbbf42d29f1b8`  
		Last Modified: Thu, 23 Jan 2020 23:07:19 GMT  
		Size: 1.0 MB (1030290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbca8ca4a5960f56ab9c9b51eee7735d8bfeace0c8683b13e23d834e20e8898c`  
		Last Modified: Thu, 23 Jan 2020 23:07:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058dc40fe23d25b2a6b8b9a31a6064c2eac5b373f52d5acb6d9219394f18a6c`  
		Last Modified: Thu, 23 Jan 2020 23:08:01 GMT  
		Size: 22.1 MB (22078401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fabe7657d0e85ffedf267cb47d1b5a01f8da1f182f429defe848b0cdb2233ab1`  
		Last Modified: Thu, 23 Jan 2020 23:07:49 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a8cf67746eef043d81238dcc09e82c7404ac11ded1b543a0d44ef4b43b1f6f`  
		Last Modified: Fri, 24 Jan 2020 15:26:52 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568aba8514f204b93c18b8eaa4a6a10b1dc92d352b0bfc41cdb4fd157b88d21a`  
		Last Modified: Sat, 25 Jan 2020 03:15:53 GMT  
		Size: 67.8 MB (67774141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dacea602a3aaea9db5b6718ed6f84d15bb2efed2ac2e05bef99abf6569720d1`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 134.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35dec2fc3052aebbbdb9c6a1a67e059e213b5e5c7c810d9595b33c2f3f342cf2`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6ae9955e302f74f4c9316777133885c5bf958ed173d65759757c8ec5851934`  
		Last Modified: Sat, 25 Jan 2020 03:15:39 GMT  
		Size: 2.7 MB (2736232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5296d0c68ebdb2f40e192360f52529db01ea6473b1fc893aced2659b3e4d102d`  
		Last Modified: Sat, 25 Jan 2020 03:15:47 GMT  
		Size: 56.3 MB (56266046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cfd7ae63629d03f592f27e8117eaae2d70ee2380134b5581049703258b91339`  
		Last Modified: Sat, 25 Jan 2020 03:15:38 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:latest`

```console
$ docker pull redmine@sha256:31dc2573b1c77945e98ad71e3ba671f787b3f402abf9d00af0b5062d3e0176bb
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
$ docker pull redmine@sha256:b020b824c4bc29851cb807d079249567fba38953a183e5c6c156843fe044fd5e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.4 MB (215374935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe885543d5387f35a4aa3a2a65968c4ace488cb67a6c40677407a4aec17c9ed`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:59:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:59:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:59:53 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:59:53 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:59:53 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:59:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:59:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:01:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:01:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:01:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:01:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:01:50 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:01:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20875f0e3d3802e64f74c9b1930e47473aa008ac1e3e2f5449ad290a85ab57`  
		Last Modified: Sat, 25 Jan 2020 03:15:23 GMT  
		Size: 93.1 MB (93059371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309a0bcae95c3ed0d1e34a294ec279f52939042fe32ae9ce3795d64ac30b93b`  
		Last Modified: Sat, 25 Jan 2020 03:15:04 GMT  
		Size: 1.3 MB (1307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce465b077ee104502ac0d3bb56ee609f8466b52df3019fc8e0eb9910c16c2475`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fd3dbd195628a62fb6e32bdc5cb84a1ad44500433876fab465c8e8d1d23c9`  
		Last Modified: Sat, 25 Jan 2020 03:15:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc96f26d91b45b07346a0a2064741540002911ab51b1c01a69d794eb672085c`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.7 MB (2735388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d61a0e145c858537c040f69d6811589e5d6e96ac59368d19b40ec966610ba7`  
		Last Modified: Sat, 25 Jan 2020 03:15:11 GMT  
		Size: 57.2 MB (57190428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5794504759a01ead1a31eb3f4b6799addca73aaca089b237498d8b773f0400f4`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:d81487b3c1ad872dcf937922c70e1b33aa56ba4ce5190286fa2d86d8adeedc35
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204856480 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb08d7d0f07498236e41fdcf83db177fea39c1c452b01cf798acd1a6878621b8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:50:35 GMT
ADD file:0d515bfdb830d6d8bec1544b49cc51e696411abf2a1afbc856f406ceb5a82a6c in / 
# Sat, 01 Feb 2020 16:50:36 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 02:08:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 02:08:29 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sun, 02 Feb 2020 02:16:09 GMT
ENV RUBY_MAJOR=2.6
# Sun, 02 Feb 2020 02:16:12 GMT
ENV RUBY_VERSION=2.6.5
# Sun, 02 Feb 2020 02:16:13 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sun, 02 Feb 2020 02:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sun, 02 Feb 2020 02:19:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sun, 02 Feb 2020 02:19:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 02:19:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sun, 02 Feb 2020 02:20:03 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 09:44:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 09:46:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 09:46:21 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:46:22 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 09:46:22 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 09:46:23 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 09:46:25 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 09:46:25 GMT
ENV REDMINE_VERSION=4.1.0
# Sun, 02 Feb 2020 09:46:26 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sun, 02 Feb 2020 09:46:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 09:50:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 09:50:23 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 09:50:23 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 09:50:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 09:50:25 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 09:50:25 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1a225882fe3b547848dd2414c8996683ea413873930a1f3a7dcb241e14fe3e85`  
		Last Modified: Sat, 01 Feb 2020 16:57:06 GMT  
		Size: 24.8 MB (24829678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecb489e800f7f428b98c5f257bb143dc6d911d3b076c3d9e0940d04f0f2557c`  
		Last Modified: Sun, 02 Feb 2020 03:16:08 GMT  
		Size: 10.3 MB (10326074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cddfcf800a56c64451730cbfd34ac7b3da09bfe974245010cf9db34bc74f681`  
		Last Modified: Sun, 02 Feb 2020 03:16:04 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfdd05ffdd7888092a6ef03be377963c297edec0344ce762bb6b3e1e2f114b94`  
		Last Modified: Sun, 02 Feb 2020 03:16:40 GMT  
		Size: 20.7 MB (20712712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e99c39d252f8cf22fae4749b2764aec83374848c63b8546989494f7f7a1cd2`  
		Last Modified: Sun, 02 Feb 2020 03:16:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff532b6c7852f386bab467c7b3f4b83b928ea314de236796805380d538c9717`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2386bd4b4f50f1d8f93b32303170d0866887841332213e58a371ca1bb7a20589`  
		Last Modified: Sun, 02 Feb 2020 10:07:52 GMT  
		Size: 88.7 MB (88656018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3116bbee905e3f17958856da579a4d33255abeddc081a9673f7e7751b098ebe`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 1.3 MB (1265374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a450151953d1dd4bd9521617998e60400bbde5af211dc4477b78be4b3f12675b`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98603c054417f4f97943b58f87a4064bff0a6fdcc842f801c987da619b29ff3b`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23326958468d4e64c292656ee80e58902c0ffdb4d9dd0ebe0f3ab5264ce8d22`  
		Last Modified: Sun, 02 Feb 2020 10:07:19 GMT  
		Size: 2.7 MB (2735847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cdb53308614fca2cb01c7b7851bffaab106d45dee36ec93f25b881241ff56a0`  
		Last Modified: Sun, 02 Feb 2020 10:07:31 GMT  
		Size: 56.3 MB (56326279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2affc3b6a6c7eac6ca68be7e12a92c5998344deee6abc0a859b5698bb25dfdcc`  
		Last Modified: Sun, 02 Feb 2020 10:07:17 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:fd859aecbff1334ede20c1579bbabb5bd45bf7594547561cdc1d27758507b025
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.9 MB (197890698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a5ca2f6d8a5214b523a543ba010bc02d222e1415eb4513f339f22da0cb06cba`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 21:07:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 21:07:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 21:19:30 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 21:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 21:22:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 21:22:59 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 03:12:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 03:12:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 03:12:51 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:39:38 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:06:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:07:01 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:07:02 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:07:03 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:07:04 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:07:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:07:07 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:07:08 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:07:15 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:10:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:10:55 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:10:56 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:10:58 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:10:59 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73268a651977563b4fdcb5f5dfd7b8f7b4b65290a1568813853d244ebf46cca`  
		Last Modified: Sat, 28 Dec 2019 22:12:53 GMT  
		Size: 9.8 MB (9847375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf46deaa8f015b62913dcf008d3f023ffdd9757f740be11a46eb091bf40916a`  
		Last Modified: Sat, 28 Dec 2019 22:12:50 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d4c32e3c622deadf3234025d30c88895c18ae7eac94288d4e42f903c4a72f5`  
		Last Modified: Sat, 28 Dec 2019 22:13:25 GMT  
		Size: 20.6 MB (20620161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fe49bcffa8c82983470bbf0074d2412dacbf1f325bcc2ffb85fddcbda7c7da8`  
		Last Modified: Tue, 07 Jan 2020 03:17:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67711a5ad765c81e93b31a6b9e1b763d7d8448315399ea1765bf97971567bfcb`  
		Last Modified: Tue, 07 Jan 2020 03:59:01 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22df051691cc30d921b9d70b85efd5cd46a51c055fb7a885fe2ae9ef34f1965`  
		Last Modified: Sat, 25 Jan 2020 02:24:54 GMT  
		Size: 84.7 MB (84708006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d2540796d803b25bed6e74b93432545aae43cc0a48e7fbf6093c5e6823b0a4`  
		Last Modified: Sat, 25 Jan 2020 02:24:26 GMT  
		Size: 1.3 MB (1258219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529a8c6a15e107f7bf7271010e2bdf9b48e58f6598901bd1971275252da7f8ae`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7837a0650c1e2b2d0636d7b4235bda5767e5c67ef97f5a6747edd98b03f63c7`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d2ce28f760155459539026440cf179c5489575000c97eae858f42d01c9568c`  
		Last Modified: Sat, 25 Jan 2020 02:24:25 GMT  
		Size: 2.7 MB (2735850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646d541d0d57a917412aac2e133006b795fac0f438acd943f02709948cba90e6`  
		Last Modified: Sat, 25 Jan 2020 02:24:38 GMT  
		Size: 56.0 MB (56017460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:714489a49c6e19537c912f14ef35b3218572e68b1c1f851192d706acad806bed`  
		Last Modified: Sat, 25 Jan 2020 02:24:24 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:58f2624f1a316fd842c70194c733401281f3850fa6fa8f1340c7d2b9198cfb57
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.1 MB (211120176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d1aa59e95791a967e02ca12ecfd915f8009cbca478126af0f52e55f8759923c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 22:20:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 22:21:00 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 22:28:49 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 22:28:50 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 22:28:51 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 22:32:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 22:32:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:41:11 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:41:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:41:14 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:06:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:34:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:35:11 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:35:13 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:35:15 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:35:15 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:35:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:35:18 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:35:20 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:35:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 02:39:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:40:02 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 02:40:03 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 02:40:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 02:40:12 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 02:40:14 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e15ace899b951b5dc6bea286f0ae88d60b68f7bf6960744e83bfe5e32d2dda`  
		Last Modified: Sat, 28 Dec 2019 23:23:09 GMT  
		Size: 11.2 MB (11244691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a139eea3e1d2ca565fe926d37cc5c8739cf40dacf7e14d474bcea8fc9a3b95`  
		Last Modified: Sat, 28 Dec 2019 23:23:05 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc7342d754a238156ddfd7ee18001a3862d29761cdf787ceb41e05bfde38061`  
		Last Modified: Sat, 28 Dec 2019 23:23:41 GMT  
		Size: 21.3 MB (21281931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1828050bdff9d08ad357e12a1bd0639c7818f955a59966e76a48d90c55ccc2`  
		Last Modified: Tue, 07 Jan 2020 02:45:23 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebec8c6749d85258e801554c4c6b4d94f96e6ca4909194be6fc4aa78f0ba7caf`  
		Last Modified: Tue, 07 Jan 2020 03:31:11 GMT  
		Size: 1.8 KB (1759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79ff809afa32d5baba46f2f7bde80a0ab57dc15374657c246cdb0db778b6c4d`  
		Last Modified: Sat, 25 Jan 2020 02:53:40 GMT  
		Size: 91.6 MB (91645815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee31ede564e2642f141b9f0353eb8a17b5738e42230d2666c77f0057e3c71ed`  
		Last Modified: Sat, 25 Jan 2020 02:53:12 GMT  
		Size: 1.2 MB (1242951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538e9d155ef665df153038fe494404878b140304e7a7358d79c50f3c06cdd0f1`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24c8d492a9f691c39c85e79b35ccf567e2430697d78dabeb9149cb9789d5d1a`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20410b8776eb35b945d7702f61a7e2c0d2f768b9d7e3919c8153e5f1f45b0370`  
		Last Modified: Sat, 25 Jan 2020 02:53:11 GMT  
		Size: 2.7 MB (2735848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17724b15809fcdf62e3624dc2b6d2500d0531bf9fa6a801f1dad1ad4a5e70b87`  
		Last Modified: Sat, 25 Jan 2020 02:53:23 GMT  
		Size: 57.1 MB (57113718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8820389aab406aeaa971c6a195fb163be61f4b7d5b3ff008a5f4f41897e285`  
		Last Modified: Sat, 25 Jan 2020 02:53:10 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:f700874a4b5a04b0de5054424a487980540e0cbc11dd8880c89437153e718aba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **220.8 MB (220831119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13bb3cef0fc5bee43a02ef2d01a7bc6cc73c13e1ecb2668ea53c6064fce16f77`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 15:34:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 15:34:06 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 15:43:14 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 15:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 15:48:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 15:48:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:39:08 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:39:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:39:08 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 03:00:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 01:47:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 01:47:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:47:29 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 01:47:29 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 01:47:29 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 01:47:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 01:47:30 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 01:47:31 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 01:47:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 01:49:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 01:49:23 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 01:49:23 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 01:49:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 01:49:24 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 01:49:24 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f578741a32d9a651490dd6e459dc212ba24462de271542e11d99371b6e6358`  
		Last Modified: Sat, 28 Dec 2019 16:44:09 GMT  
		Size: 17.2 MB (17206012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfea7e4ab816e0d4ed54b9e31ec21865bd3dfe746cb61458602141c78b63966a`  
		Last Modified: Sat, 28 Dec 2019 16:43:58 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b12042d352b3390a1d5c085213ccee7f26bee56d8a1a3fb0a76e80159a411c`  
		Last Modified: Sat, 28 Dec 2019 16:44:44 GMT  
		Size: 20.9 MB (20885521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c53ce40fd432336a5365d519861a9d64c7cf858412dd402f939e5f6cb0ed3f`  
		Last Modified: Tue, 07 Jan 2020 02:41:40 GMT  
		Size: 141.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b71e9da85871d84768b7e4ee95650087a03f4db095955f62e526335b0c09aa4`  
		Last Modified: Tue, 07 Jan 2020 03:11:10 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5f640023220debb54aa59008a23084703fc0537fc624f8ceab4d90009b5f0a`  
		Last Modified: Sat, 25 Jan 2020 01:55:48 GMT  
		Size: 94.7 MB (94693229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c958a54bf64e77189cf05b4486d2756c03a8c3d2dfaa0623e2a09c1a5109e0b`  
		Last Modified: Sat, 25 Jan 2020 01:55:24 GMT  
		Size: 1.3 MB (1275383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00731a6396a0f584e04f340d4a49c149951c796ca229ed740930499b1a882c`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3a2a82b5a98ff43706a5284dab0afd502f20a49c7a2a08ed51f40683ac458d`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d5165755570cce25c28f06dd103a1d73386b43cf12f92cd6ca898131ae5663`  
		Last Modified: Sat, 25 Jan 2020 01:55:24 GMT  
		Size: 2.7 MB (2735383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe1b8246e4d2cefa8623bb1ec59f0b3ab47bb321632de09d3ea2b875a984bc8`  
		Last Modified: Sat, 25 Jan 2020 01:55:33 GMT  
		Size: 56.3 MB (56284173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30a398c5eaf1193a79396d5800707f6528d558924b2c597e2767da34ae511bb6`  
		Last Modified: Sat, 25 Jan 2020 01:55:22 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:f08f037717dc3721e961cb0907ae97ac8328ba24fe1bfa1b059ed270e9cfe715
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227173333 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec2bb12560bf4f88050034a40821bb893c2d88a2a3c4abd85702087a17761c09`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 04:37:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 04:37:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 04:44:05 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 04:44:07 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 04:44:10 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 04:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 04:49:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:18:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:18:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:18:58 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:52:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 03:06:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:06:20 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 03:06:23 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 03:06:27 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 03:06:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 03:06:35 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 03:06:37 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 03:06:47 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:10:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:10:41 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:10:42 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:10:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:10:47 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:10:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e10577c89c450ecfcb6cd75777c15ce8a9c0118a86cd89b181c32ae50e530`  
		Last Modified: Sat, 28 Dec 2019 05:29:25 GMT  
		Size: 12.7 MB (12688889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20f2864ed98b31f7d1955c54fb2f0f3eaabae93374f8c0f8bc6f6e4d871b33c`  
		Last Modified: Sat, 28 Dec 2019 05:29:18 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd8219d68aec763d8d91942869b8dd9ef7233da0ba814028c00dce26b61b1ec`  
		Last Modified: Sat, 28 Dec 2019 05:29:59 GMT  
		Size: 22.0 MB (21968340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88418e7313544081130ec82f1125b007f6673672ed6fe3f2815a8bc0836d834d`  
		Last Modified: Tue, 07 Jan 2020 02:27:35 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c811e39d17ef5178d803832537e4b94505620908b40d2ece5c639ebc74bb249c`  
		Last Modified: Tue, 07 Jan 2020 03:29:32 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1fdc2fee5bcdaa20790472eb3b3e6a238cee4c14ea8503eaf556e87582caf2b`  
		Last Modified: Sat, 25 Jan 2020 03:29:20 GMT  
		Size: 100.3 MB (100282383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37063699c1769c556fcd7e961dae12c108451947f10a4381c9312fb86a65bb6b`  
		Last Modified: Sat, 25 Jan 2020 03:28:58 GMT  
		Size: 1.2 MB (1232203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77c914aba14ea81411aae5a9d0b596dbebda443ecb800ce8e717f0c782a367b`  
		Last Modified: Sat, 25 Jan 2020 03:28:53 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b47a8358f9f444669f85d1a5f3690a1d8e37b0c91e7a827ceb0b4937b251c5`  
		Last Modified: Sat, 25 Jan 2020 03:28:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b553f520f8f427b541d300f1b7cd485adf7ee67d7046a370c78d993aaebff1a7`  
		Last Modified: Sat, 25 Jan 2020 03:28:56 GMT  
		Size: 2.7 MB (2735856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1492d8aabeb5a9c29d1c9c848723748f59b53365c4e70c0d9c897c329ca329`  
		Last Modified: Sat, 25 Jan 2020 03:29:06 GMT  
		Size: 57.7 MB (57743620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556573964a0bd208b3e595f68ab9d500f1405000b822b06641efaa11e9820c7b`  
		Last Modified: Sat, 25 Jan 2020 03:28:54 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:ab1568d6b226e18d614f69224ab5082f76ab6c3c459575b451c0b43a044e4c88
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.6 MB (210607230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e81bbd4d53db9fe58b1f99028cbe990f74848ac4052582c07576953e60742dc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:29 GMT
ADD file:fb7d675adcb17ba15644d52683f50577e05e7e613dee00a1b2e40463f31bbf29 in / 
# Sat, 01 Feb 2020 16:42:30 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 22:24:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 22:24:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_MAJOR=2.6
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 01 Feb 2020 22:34:36 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 01 Feb 2020 22:36:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 01 Feb 2020 22:36:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 01 Feb 2020 22:36:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 01 Feb 2020 22:36:07 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 01 Feb 2020 22:36:07 GMT
CMD ["irb"]
# Sun, 02 Feb 2020 03:24:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 02 Feb 2020 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 03:25:35 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:25:35 GMT
ENV RAILS_ENV=production
# Sun, 02 Feb 2020 03:25:36 GMT
WORKDIR /usr/src/redmine
# Sun, 02 Feb 2020 03:25:36 GMT
ENV HOME=/home/redmine
# Sun, 02 Feb 2020 03:25:36 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 02 Feb 2020 03:25:37 GMT
ENV REDMINE_VERSION=4.1.0
# Sun, 02 Feb 2020 03:25:37 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sun, 02 Feb 2020 03:25:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 02 Feb 2020 03:28:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 02 Feb 2020 03:28:15 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 02 Feb 2020 03:28:15 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sun, 02 Feb 2020 03:28:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 02 Feb 2020 03:28:16 GMT
EXPOSE 3000
# Sun, 02 Feb 2020 03:28:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:56a040772f0865ef22b9f53d560f9780e6aaa2ab7c117116a7832d97a10b06c1`  
		Last Modified: Sat, 01 Feb 2020 16:45:51 GMT  
		Size: 25.7 MB (25705378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c17d8d1356b8293f168a2578ba81c34f07ee79d7a56bd579e776ad498d0b2e8`  
		Last Modified: Sat, 01 Feb 2020 22:56:51 GMT  
		Size: 10.8 MB (10795999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d180073499f34bb9340ecac840eeb00fab127188f731188ba78e76e435b62c`  
		Last Modified: Sat, 01 Feb 2020 22:56:55 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:351f50ba1593f8ab66d1deaf12e190c35ecfea96815beda37efe10f1246f342b`  
		Last Modified: Sat, 01 Feb 2020 22:57:18 GMT  
		Size: 21.6 MB (21592569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d8a5d1fd225888733445fbc5a03464b232ab7c659a3bf619e93c5670a0ca594`  
		Last Modified: Sat, 01 Feb 2020 22:57:14 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6b52758f305e2a6eca340f3801ffcd699d9f9863ebfe870573fbea05f125b`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9b9c2d954e677f77134627d444d4526d3dd757e20731a3db791ee045bd3ff5`  
		Last Modified: Sun, 02 Feb 2020 03:35:13 GMT  
		Size: 90.8 MB (90810821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4b03bbe680823684e8167d23322040275fc82bb40b38251bd1aca1d9759997`  
		Last Modified: Sun, 02 Feb 2020 03:34:59 GMT  
		Size: 1.3 MB (1297549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6a56833da980d550b03c0656e63d42b60190fa8f5b743d0efd1679e03cb5ea`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6743cd35c07b27ae19792d6c94243798a11247fa7a5f0fd8d63ec5fec7f8c8`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0844cdbf926f537d20bc1295376495cb2b126746d549e3cc88402e855e2f92`  
		Last Modified: Sun, 02 Feb 2020 03:34:58 GMT  
		Size: 2.7 MB (2735858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a0c8052dd4f2d2e8e61136ca875e5667f9fdd869156f21339a352533be465b`  
		Last Modified: Sun, 02 Feb 2020 03:35:25 GMT  
		Size: 57.7 MB (57664549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b47a626d921e859c5def90095c9624aa612e063bcacdce5bb5485574308e28`  
		Last Modified: Sun, 02 Feb 2020 03:34:57 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:passenger`

```console
$ docker pull redmine@sha256:ba7a9f6a40c0321efb4e23c475561ca7900e9b554dc4acc094735f7e662d4b15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:1a4b83e2c247a77f9df50853b0b68e3bc67bd981aae0a2fc71efb39124cb0a36
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240227783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e4526c7d5cd953230156bb4a6db6a31bbfaa56aa6bf8bcc06f6e5371921ae60`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 14:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 14:28:19 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_MAJOR=2.6
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 28 Dec 2019 14:36:24 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 28 Dec 2019 14:39:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 28 Dec 2019 14:39:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 07 Jan 2020 02:20:33 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Jan 2020 02:20:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 07 Jan 2020 02:20:34 GMT
CMD ["irb"]
# Tue, 07 Jan 2020 02:41:39 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 25 Jan 2020 02:59:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 25 Jan 2020 02:59:52 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 02:59:53 GMT
ENV RAILS_ENV=production
# Sat, 25 Jan 2020 02:59:53 GMT
WORKDIR /usr/src/redmine
# Sat, 25 Jan 2020 02:59:53 GMT
ENV HOME=/home/redmine
# Sat, 25 Jan 2020 02:59:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_VERSION=4.1.0
# Sat, 25 Jan 2020 02:59:54 GMT
ENV REDMINE_DOWNLOAD_MD5=32c7b9ce4c419092da439b540cbc1dbf
# Sat, 25 Jan 2020 02:59:57 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 25 Jan 2020 03:01:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:01:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 25 Jan 2020 03:01:50 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Sat, 25 Jan 2020 03:01:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 25 Jan 2020 03:01:50 GMT
EXPOSE 3000
# Sat, 25 Jan 2020 03:01:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Sat, 25 Jan 2020 03:02:09 GMT
ENV PASSENGER_VERSION=6.0.4
# Sat, 25 Jan 2020 03:02:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 25 Jan 2020 03:02:28 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Sat, 25 Jan 2020 03:02:28 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Sat, 25 Jan 2020 03:02:28 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b696148f80a3c55c2ac62fc43b0dc9affda80e9d211be56b08eef2f1ed659e`  
		Last Modified: Sat, 28 Dec 2019 15:18:07 GMT  
		Size: 12.5 MB (12539763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf092395f95bf11a093c51888632dadaf83f109f32ddf902cbecac8dd79cc89`  
		Last Modified: Sat, 28 Dec 2019 15:18:03 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a36680cb06fd38e45aac23a7011098c9d1758b5a43eac90b5c6ffff256f1464`  
		Last Modified: Sat, 28 Dec 2019 15:18:25 GMT  
		Size: 21.4 MB (21445640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99fd40d9a9ace0f7aed9e5a259d44332d8449577afa416ece494654eebfea1e0`  
		Last Modified: Tue, 07 Jan 2020 02:22:59 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57bbb61ed5d5be2c4bcad836a9ca7c8585b621afa2d63929ca63ed54bba5b6`  
		Last Modified: Tue, 07 Jan 2020 02:58:46 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab20875f0e3d3802e64f74c9b1930e47473aa008ac1e3e2f5449ad290a85ab57`  
		Last Modified: Sat, 25 Jan 2020 03:15:23 GMT  
		Size: 93.1 MB (93059371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6309a0bcae95c3ed0d1e34a294ec279f52939042fe32ae9ce3795d64ac30b93b`  
		Last Modified: Sat, 25 Jan 2020 03:15:04 GMT  
		Size: 1.3 MB (1307662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce465b077ee104502ac0d3bb56ee609f8466b52df3019fc8e0eb9910c16c2475`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4fd3dbd195628a62fb6e32bdc5cb84a1ad44500433876fab465c8e8d1d23c9`  
		Last Modified: Sat, 25 Jan 2020 03:15:02 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc96f26d91b45b07346a0a2064741540002911ab51b1c01a69d794eb672085c`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.7 MB (2735388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d61a0e145c858537c040f69d6811589e5d6e96ac59368d19b40ec966610ba7`  
		Last Modified: Sat, 25 Jan 2020 03:15:11 GMT  
		Size: 57.2 MB (57190428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5794504759a01ead1a31eb3f4b6799addca73aaca089b237498d8b773f0400f4`  
		Last Modified: Sat, 25 Jan 2020 03:15:03 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff399de53c760559fd2eee97d976fac5edfad88174424ed39eb1c80f14d2e7d`  
		Last Modified: Sat, 25 Jan 2020 03:15:33 GMT  
		Size: 19.9 MB (19935002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0411f053fc05d6fa100b4b761e3b8fd4ad0ac893351b89b722ec5c86087665a`  
		Last Modified: Sat, 25 Jan 2020 03:15:31 GMT  
		Size: 4.9 MB (4917846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
