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
-	[`redmine:4.1.4`](#redmine414)
-	[`redmine:4.1.4-alpine`](#redmine414-alpine)
-	[`redmine:4.1.4-passenger`](#redmine414-passenger)
-	[`redmine:4.2`](#redmine42)
-	[`redmine:4.2-alpine`](#redmine42-alpine)
-	[`redmine:4.2-passenger`](#redmine42-passenger)
-	[`redmine:4.2.2`](#redmine422)
-	[`redmine:4.2.2-alpine`](#redmine422-alpine)
-	[`redmine:4.2.2-passenger`](#redmine422-passenger)
-	[`redmine:alpine`](#redminealpine)
-	[`redmine:latest`](#redminelatest)
-	[`redmine:passenger`](#redminepassenger)

## `redmine:4`

```console
$ docker pull redmine@sha256:946ffb0d6839fa3d89d077b47d3024b103b42f905463932ea6950703489217a7
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
$ docker pull redmine@sha256:184738eb8da314459e8b41f33ffdfad41e82d466ec96843bf49cd46d1bc5109a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195495858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab3b16cafa89a7d46015d66e213c5ddc798b96e35c33ae8100fc09ba1d9525e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:21:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:23:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:23:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:23:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:23:47 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:01:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:01:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:01:29 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:01:29 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:01:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 18:01:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:02:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:02:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:02:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:02:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:02:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119720cd004c3495b5cd6b8883e01df56a3438046b3ecc3198ffb3849f6f25df`  
		Last Modified: Tue, 17 Aug 2021 04:42:13 GMT  
		Size: 14.5 MB (14510198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b764bf01e480a9fff1b3e5a263f7f9f9b4fa77325f616c37cb8e2c81d51e3dd9`  
		Last Modified: Tue, 17 Aug 2021 04:42:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84946f74729ab44aaa49a9af6012e6293fb02521ca05cffaccf128e7b157cec`  
		Last Modified: Tue, 17 Aug 2021 18:09:47 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcde4d7d6d22355ecf23701bfa1a2abba49bcabfc5f4dd90c746e0143569ba`  
		Last Modified: Tue, 17 Aug 2021 18:10:07 GMT  
		Size: 94.1 MB (94087892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5742225b6ad582633258fcf1e969851dbdd33be3d03cb05cf61b1ea900d8cc`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81933ac92f0a4be0c34689c7c3035c0aa0e4d7e89153bb41cbe0821a1c2a89f7`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb927d9d1176a8bbb1d88d687d964fae4ee7e61ebd08be4d8648f21caa9299e`  
		Last Modified: Tue, 17 Aug 2021 18:09:46 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d25f4984fe7a6089fe506ca06732024aafbfe47de090d95c448ac84b589e573`  
		Last Modified: Tue, 17 Aug 2021 18:09:53 GMT  
		Size: 44.1 MB (44122772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f790489c8bf8667ba0727c9aa46fb6e9d9128bf89a9c1330b90689f04155bf`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:2e7f776816b5769bfdaa730b3d5c3d64b1025e071ad1c79a6716eff4c1041de1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed286853331cdd20528ca2dacc87e979025cee325cdd5528cc16dd1b6558987f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:31:22 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 17:31:23 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 17:31:23 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 17:35:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:35:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:35:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:35:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:35:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:35:44 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 04:57:25 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 04:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 04:58:43 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 04:58:43 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 04:58:44 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 04:58:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 04:58:46 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 04:58:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 04:58:52 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:04:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:04:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:04:38 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:04:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:04:39 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:04:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add78f82744b7f4c8c7522adfae87214be4104b79f343add868890b00ec859d2`  
		Last Modified: Fri, 03 Sep 2021 18:01:59 GMT  
		Size: 13.9 MB (13871472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea079592f786a6bd50d8249c1ceedc638402805fe700febed7e646dd69ee642`  
		Last Modified: Fri, 03 Sep 2021 18:01:51 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217f2b4088020d7dcc1aed89a3d8db9a8756c8bee078541881250a9dbbad1e6`  
		Last Modified: Sat, 04 Sep 2021 05:20:20 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5101e0f6c49b2df1f4b08067b3c1b135fe25243c4054b5868f953bc3f37490bf`  
		Last Modified: Sat, 04 Sep 2021 05:21:21 GMT  
		Size: 89.6 MB (89576088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ae1568de59acec6c4cb2932be2397e122fea3950b3104ce626623970d75f5`  
		Last Modified: Sat, 04 Sep 2021 05:20:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e297238097a4d3b15fbadef5aa4d865ab9cef981d1cae1bb633f216dd4c9dad`  
		Last Modified: Sat, 04 Sep 2021 05:20:18 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6628563efc672886d9ef6550835ad5efa230a1e39f41e8e612ad2af2c4e7ba99`  
		Last Modified: Sat, 04 Sep 2021 05:20:21 GMT  
		Size: 3.1 MB (3061924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0be986223cb5256d684c7602b705f39bd686a8ffb95e92c116f1db188b1da6`  
		Last Modified: Sat, 04 Sep 2021 05:20:43 GMT  
		Size: 55.2 MB (55234623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcee35bd3d5db50a493ba5105b6272ef59dc2eb800bb91c4eef2c100309638c`  
		Last Modified: Sat, 04 Sep 2021 05:20:18 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cd7275a7d34b3290a919f94e8e29ca61a913d0427cd2718ed49e354450b9eb2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0f96d1f050b7bd3415163fa63302bbaf4443e8741688fdcbbe19819f034e55`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:30:30 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 09:44:16 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 09:44:17 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 09:44:17 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 09:48:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 09:48:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 09:48:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 09:48:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:48:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 09:48:25 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 08:32:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 08:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:33:59 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 08:33:59 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 08:34:00 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 08:34:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 08:34:02 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 18 Aug 2021 08:34:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 18 Aug 2021 08:34:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 08:39:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 08:39:27 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 08:39:27 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 08:39:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 08:39:28 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 08:39:29 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79875132dbc48a8386eb9079eb8b50d17399ed33c29a51ac8d7b2f943f3b1ac`  
		Last Modified: Tue, 17 Aug 2021 10:24:54 GMT  
		Size: 9.9 MB (9872248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ce2d51bf7561cb7c360e69499b42694c2e474b2f24d969e4250ac389dd4bec`  
		Last Modified: Tue, 17 Aug 2021 10:24:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6910fec61b3de474c201c0eaae12d42336d748c8d6c55e7b06571adfef449ac`  
		Last Modified: Tue, 17 Aug 2021 10:26:58 GMT  
		Size: 13.8 MB (13767304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376804c80b6dffd48a9a1ce10f9ae6e593d25030de692dfc17341be078eaad9f`  
		Last Modified: Tue, 17 Aug 2021 10:26:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d2abf0978eca4cf58f5136adb1c1db17ff192b414feb932d7a524feb862a06`  
		Last Modified: Wed, 18 Aug 2021 08:54:19 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25cf090ed21d7e7a084b69c43bc419fc12838e33b344eba331171fc2868d53d`  
		Last Modified: Wed, 18 Aug 2021 08:54:58 GMT  
		Size: 85.6 MB (85590672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782c9d20468a0cc0f8d38101ddc7ef218d18c48ecbeda7932121ed297886d697`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eab3d69b805b2536e4dd6b587ff8eb27d96f2df1057e5e31d91410e872d74f`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b22a54dbdc1d4adfc0f8ae626f1aed9ec9010d827a989cf4af007f1126801d`  
		Last Modified: Wed, 18 Aug 2021 08:54:20 GMT  
		Size: 3.1 MB (3061921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2005224b6c07acc4bbabc1a0bb15ec249509c15fcfd8d777031ad7050b6ce1ac`  
		Last Modified: Wed, 18 Aug 2021 08:54:34 GMT  
		Size: 55.1 MB (55073085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1537e502cf0def19348a8406f66144d8986698047998e80c0a8ce7c1759735`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:54281b02713340086f8270560a0a6f34bd50ef111b8136870436e66a36c494b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203249301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c7d37a5bf5a362ddcdb750e1beba28d0362bd1632eaf9ed4bea0913ac529f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 12:12:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:12:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:12:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:12:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:12:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:12:43 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:04:14 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:04:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:04:38 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:04:38 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:04:39 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:04:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:04:39 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 05:04:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 05:04:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:07:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:07:20 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:07:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:07:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:07:21 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:07:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee312ced32893df36a25a76149db554574daaeb35128bcfb8c1d9d5bbc1fe73d`  
		Last Modified: Fri, 03 Sep 2021 12:28:34 GMT  
		Size: 14.4 MB (14356717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719ff35ff5b1cf24bc8a71ce6e567a505fbb6fcf0e9c141d8bdc230f164a57a0`  
		Last Modified: Fri, 03 Sep 2021 12:28:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd82b0673245cfbd7fe883e89fb55be7bd3e805e26de6ef17064f507f3df13c`  
		Last Modified: Sat, 04 Sep 2021 05:13:30 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d090f849a4da11b63677dfaff64f9709e15e9a24e740bcfbbca2545dc3f6395`  
		Last Modified: Sat, 04 Sep 2021 05:13:46 GMT  
		Size: 92.6 MB (92609378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9748bdee2b0b6d123ea99593dc5ff47d2b23dc011f52aef631f6eff5be900547`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454a0d8da53bfccd39f515fb93989777b3b6ebfc7c78bcb00be2b2e831683de`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323cf17e748812ba32fb6ed26e50ba83a1ddc4ec3eb22dc3674a4ddfc7ab2674`  
		Last Modified: Sat, 04 Sep 2021 05:13:29 GMT  
		Size: 3.1 MB (3061917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f679bdbfd5dafda429d92ba97d958576ee482d6c7e7ef09611df897a8af86ee7`  
		Last Modified: Sat, 04 Sep 2021 05:13:34 GMT  
		Size: 56.0 MB (56037790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080fea9fe34c2c40a03359a1c3402d684badf754bb190a6f22679e53c3d25c08`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; 386

```console
$ docker pull redmine@sha256:ebc552d443096692ec50b0c4279d2cfef5098651e51fab433fa57a8859e864c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202126624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c6ceb9f5cc0c343839ed2f1ed0ac64ccf12847ac4939e863d82309c42e9ec3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:39:26 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 11:39:27 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 11:39:27 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 11:43:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 11:43:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 11:43:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 11:43:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 11:43:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 11:43:41 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 06:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 06:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 06:05:58 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 06:05:59 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 06:05:59 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 06:06:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 06:06:01 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 06:06:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 06:06:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 06:07:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 06:07:41 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 06:07:42 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 06:07:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 06:07:42 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 06:07:43 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ab3f959a8410b96952c0ab29ff5376ff960f0c46619b9da4de191c3e631a2e`  
		Last Modified: Fri, 03 Sep 2021 12:10:29 GMT  
		Size: 14.0 MB (13992725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b213d5105e1a800ff597002681646442fd6df3b46274ee545c1825df025af800`  
		Last Modified: Fri, 03 Sep 2021 12:10:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fa640c55779f987dc35c6cc6766cb5f2fa277c85a28f8b096f1276dedc45ba`  
		Last Modified: Sat, 04 Sep 2021 06:16:20 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae199078f5eaaf3ea967d1448f821631d10ea7afd47dcb79a7701e0fe24ed70`  
		Last Modified: Sat, 04 Sep 2021 06:16:43 GMT  
		Size: 95.7 MB (95703257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61de99b7f1e5da0063d2955ec7a01f01d7ed345b8b6dd804aada111402bf9f`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ba76c31dcad016bf941f0e0be2694f0fa339e5c24d7ef5ee4916be74697f0a`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70e46e86bb38bc42f7060c39fbbc233ea20e6f7089b73e2335d3440c1c33d1`  
		Last Modified: Sat, 04 Sep 2021 06:16:18 GMT  
		Size: 3.1 MB (3061914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb99b00b084c4a0e83a272f225159c4cbf6214c81fe2f8571dfaf4276978ce97`  
		Last Modified: Sat, 04 Sep 2021 06:16:25 GMT  
		Size: 44.3 MB (44340016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cbcc1c6467ba9477359f3f850d4c4535ba281eea1e75124bb96d94ba91c2fa`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; ppc64le

```console
$ docker pull redmine@sha256:750c649c6ed54a1bc79c41c44b1bfb009a38e130ca51356a0a5637a77b452f5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219650978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3733a5127a682e88605681a10a6637a271090e9dddd1ecb6d71d7b4e0b6d2c82`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:32:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:32:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 09:53:38 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 09:53:41 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 09:53:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 10:00:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:00:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:00:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:01:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:01:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:01:28 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 06:54:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 06:59:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:00:07 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 07:00:21 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 07:00:26 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 07:00:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 07:00:43 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 18 Aug 2021 07:00:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 18 Aug 2021 07:01:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 07:07:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 07:07:18 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 07:07:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 07:07:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 07:07:39 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 07:07:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6540cca707f751654267130c5ff13338c730506cf900ab70cbba8eb8f0774f4`  
		Last Modified: Tue, 17 Aug 2021 10:35:53 GMT  
		Size: 12.7 MB (12704229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cb3d072ea667e9971932f23c9c5ddffe4a2d7c9a645aa1f53235dc8c2e2ae5`  
		Last Modified: Tue, 17 Aug 2021 10:35:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29445a92f99df6ece2c68fdd21d13b23e28c76507ae5fc4497cbf9272cd41e91`  
		Last Modified: Tue, 17 Aug 2021 10:37:15 GMT  
		Size: 15.0 MB (14997282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee87ac0f307c59470977ad0b974013269088413f9061698138c7f01175ec9982`  
		Last Modified: Tue, 17 Aug 2021 10:37:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfb261039caaf3d27ac4757a6a0ca770e695ac15e72cce135badcdf8d17b060`  
		Last Modified: Wed, 18 Aug 2021 07:40:45 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa4557b0838e19c4cd9f385a4b5ea0972af6fba31e8bcc39e77336887cd48ee`  
		Last Modified: Wed, 18 Aug 2021 07:41:48 GMT  
		Size: 101.3 MB (101328471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5cb4e6a472bc1f6140175c495cf2115da58206520a01bca00638227f2370ea`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4789be342e86d5f2793092f064c41fde923d87fb85f130d8100b4c88af3474`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2190284052685dcbf10a7e8e39410965a72be33c4c924cedc97130de22e6c8f4`  
		Last Modified: Wed, 18 Aug 2021 07:40:52 GMT  
		Size: 3.1 MB (3061910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b6fa0cc2de623e70d74216ebe78d7dfccc76bda34aae287ec61259ff3f54ce`  
		Last Modified: Wed, 18 Aug 2021 07:41:17 GMT  
		Size: 57.0 MB (57001117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164f878c998618c80d1e4d55973b954723ba05120f5a4984c112bc210edd8c6`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; s390x

```console
$ docker pull redmine@sha256:f764e6f237dd0b4ccc459c4a58872d66f5d9015fa61828ef337cc1aba2dde405
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202557142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:182cde8e814a22a30968ac8996e2499e862f311f0c6cd3a5d1db75334c1b9dce`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 13:38:11 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 13:38:11 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 13:38:12 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 13:41:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 13:41:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 13:41:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 13:41:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 13:41:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 13:41:45 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 02:39:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 02:40:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:40:18 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 02:40:18 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 02:40:19 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 02:40:19 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 02:40:19 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 02:40:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 02:40:23 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 02:42:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 02:42:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 02:42:50 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 02:42:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:42:51 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 02:42:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ea6888b61e31cb5b4a8f014006c7cb8fa8a3b7224b7ad3f0b4af257229c789`  
		Last Modified: Fri, 03 Sep 2021 14:14:23 GMT  
		Size: 14.7 MB (14697502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ef0cfb1210ec8b5dff947c27988590a3931cf76a1437a6fe10f30aae9f813`  
		Last Modified: Fri, 03 Sep 2021 14:14:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a04f5ff5ec2ee8dd1b21974adff7bf0e6fdb70338e190c6094eed2747ceb117`  
		Last Modified: Sat, 04 Sep 2021 02:50:16 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf9140fc0de2f47daa7719c6c1cbbf193066ad2a67f60c95d78b7baf3626508`  
		Last Modified: Sat, 04 Sep 2021 02:50:29 GMT  
		Size: 91.8 MB (91790843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d640980eb96fb9f7eef22043b3c502898b8cc3f7b1447f1f19055222d3a3bf`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80df1a5482c5309af87986c42c45a6cd4c0cfbce1535792b2c1ba652e2c2a304`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9bc3013aec1061db002a07fa5ae39181287f086837e8c8c53c5814049c837d`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 3.1 MB (3061916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9caa222bcb2e88202afcfdf166e5a0613fe99bc55cc9b416dda1e1e2484c4`  
		Last Modified: Sat, 04 Sep 2021 02:50:19 GMT  
		Size: 56.4 MB (56426601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff0983c6ea2bc0e811104db8303487a7286daf0ee17c051de72eb5e75dbbc32`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:b3f4c38a52e764136b2d930a044a60e362120dd0c8900217a3e90e852421ab31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:c5db53d0c811b57d386d30b72d9050a7aa2fe1cf1b73fd86e20caaf5794597b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.7 MB (149701448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e405182f204a9a00f59a9abe4dd5e343cc108150ea4d66c36d925aed95a284`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:46:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Sep 2021 05:46:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Sep 2021 05:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_MAJOR=2.7
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Wed, 01 Sep 2021 05:53:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Sep 2021 05:53:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Sep 2021 05:53:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Sep 2021 05:53:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 05:53:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Sep 2021 05:53:30 GMT
CMD ["irb"]
# Wed, 01 Sep 2021 08:00:22 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 01 Sep 2021 08:00:30 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 01 Sep 2021 08:00:30 GMT
ENV RAILS_ENV=production
# Wed, 01 Sep 2021 08:00:30 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Sep 2021 08:00:31 GMT
ENV HOME=/home/redmine
# Wed, 01 Sep 2021 08:00:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 01 Sep 2021 08:00:32 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 01 Sep 2021 08:00:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 01 Sep 2021 08:03:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 01 Sep 2021 08:03:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 01 Sep 2021 08:05:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 01 Sep 2021 08:05:51 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 01 Sep 2021 08:05:52 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 01 Sep 2021 08:05:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 08:05:52 GMT
EXPOSE 3000
# Wed, 01 Sep 2021 08:05:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439708bfc17dd3e86c8b1415116fcd9de1d32330bdcc8b13fd009f7727844e9`  
		Last Modified: Wed, 01 Sep 2021 05:58:07 GMT  
		Size: 3.6 MB (3581641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260bc7d8cd8f26c27362c4ab1698f2a3e0b0a88516cdfd73a8884747ec12ee`  
		Last Modified: Wed, 01 Sep 2021 05:58:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b385b36ad53753eb77bf737911b40c7b42d1d603a8005a53f2f2f9d3aa2a647`  
		Last Modified: Wed, 01 Sep 2021 05:58:33 GMT  
		Size: 14.0 MB (13991225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92418e596130e2278d466f8249bbfd0342dc1ed5615322250d5291980e5e711`  
		Last Modified: Wed, 01 Sep 2021 05:58:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb69d3417cce9a0cd0808740d79cad62e362f9e7780f9e847fda8698922434f8`  
		Last Modified: Wed, 01 Sep 2021 08:17:11 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff5239c638a3da1239c50061fdbda7f2ab705410a586090f90731563aebf09b`  
		Last Modified: Wed, 01 Sep 2021 08:17:21 GMT  
		Size: 69.5 MB (69527596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4595191c9d0a75afbae796393c0d8785fc677252ad2d85ab2cec624eb5f9c1cf`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be97b97c73e6fb6c46d0181b8440a11bc4bb76e361ae0d2fc5dc5829ad8c890`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2904ae75e075530bcb634aefc3d51e773208ce91e366be679351205797597f5b`  
		Last Modified: Wed, 01 Sep 2021 08:17:09 GMT  
		Size: 3.1 MB (3062876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aa578222ef92d9141208d74301432942113f80ee6a5498fd82515c20955471`  
		Last Modified: Wed, 01 Sep 2021 08:17:14 GMT  
		Size: 56.7 MB (56720303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f3a3dc13988389eb05a94dba971d771fb9fc0e1b3ed1fd8ba96d3f39eac1c3`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:dc1fa7ae440292befc3702f68fd45e6167a13086847d9c4151f3e7fddab3d679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:1384ea37efaf431cdff585a3d29cc018cacfc671a3c5e723b8f2880fa480659f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221546741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65d69f1c7954cffcb45c23d12731b72e27472b5d6ae629622df20fcda3a4d414`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:21:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:23:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:23:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:23:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:23:47 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:01:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:01:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:01:29 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:01:29 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:01:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 18:01:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:02:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:02:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:02:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:02:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:02:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 17 Aug 2021 18:02:25 GMT
ENV PASSENGER_VERSION=6.0.10
# Tue, 17 Aug 2021 18:02:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:45 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 17 Aug 2021 18:02:45 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 17 Aug 2021 18:02:45 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119720cd004c3495b5cd6b8883e01df56a3438046b3ecc3198ffb3849f6f25df`  
		Last Modified: Tue, 17 Aug 2021 04:42:13 GMT  
		Size: 14.5 MB (14510198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b764bf01e480a9fff1b3e5a263f7f9f9b4fa77325f616c37cb8e2c81d51e3dd9`  
		Last Modified: Tue, 17 Aug 2021 04:42:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84946f74729ab44aaa49a9af6012e6293fb02521ca05cffaccf128e7b157cec`  
		Last Modified: Tue, 17 Aug 2021 18:09:47 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcde4d7d6d22355ecf23701bfa1a2abba49bcabfc5f4dd90c746e0143569ba`  
		Last Modified: Tue, 17 Aug 2021 18:10:07 GMT  
		Size: 94.1 MB (94087892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5742225b6ad582633258fcf1e969851dbdd33be3d03cb05cf61b1ea900d8cc`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81933ac92f0a4be0c34689c7c3035c0aa0e4d7e89153bb41cbe0821a1c2a89f7`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb927d9d1176a8bbb1d88d687d964fae4ee7e61ebd08be4d8648f21caa9299e`  
		Last Modified: Tue, 17 Aug 2021 18:09:46 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d25f4984fe7a6089fe506ca06732024aafbfe47de090d95c448ac84b589e573`  
		Last Modified: Tue, 17 Aug 2021 18:09:53 GMT  
		Size: 44.1 MB (44122772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f790489c8bf8667ba0727c9aa46fb6e9d9128bf89a9c1330b90689f04155bf`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b74d84a329f08033107c147b415d461e38428d975adc347ea34654240ab09e`  
		Last Modified: Tue, 17 Aug 2021 18:10:30 GMT  
		Size: 21.1 MB (21131600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235136ff85630baea96544cddd34b782c51fbd5824839b6264d7ac17db683c0a`  
		Last Modified: Tue, 17 Aug 2021 18:10:27 GMT  
		Size: 4.9 MB (4919283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0`

```console
$ docker pull redmine@sha256:e18d85cb2968758d4a74290667b00349a4de0891dd79f66cf424edf05db360c3
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
$ docker pull redmine@sha256:d6d905b7ab421a941dc5c23c46f5bd46fe613971f7f61ea346eef7abf660491e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205070145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b6a0822eb22f16e48160adfb284d9f5ccadf6906b0424b6759a186d5af659d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:34:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:34:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:34:16 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:02:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:06:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:06:04 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:06:04 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:06:05 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:06:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:06:06 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 18:06:07 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 18:06:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:08:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:08:34 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:08:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:08:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:08:34 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:08:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d07c054cf634a28fbb441bc93e20e2d4ae0dbaeb43e6aa17ab1c66f1c26b73`  
		Last Modified: Tue, 17 Aug 2021 04:43:06 GMT  
		Size: 21.5 MB (21468054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051a36df400859440c745a4abab787eac2d2318444dcd251750cf3a456ba21`  
		Last Modified: Tue, 17 Aug 2021 04:43:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85f465fea1749f74517e7a2b2c81d5ab6f19157bf460e5e7476d3aa04d2d7e`  
		Last Modified: Tue, 17 Aug 2021 18:10:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f710b25dd48260ef6143f3bbbe5a8211fb635d0408b6e87588e65a7ee41fd42`  
		Last Modified: Tue, 17 Aug 2021 18:12:00 GMT  
		Size: 81.2 MB (81200061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211f3fb54688e3a1a8be31d871a75ed1126c065165edc8a2ba25fa9695157cad`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f792c3664b204ad48d660ca5f20e9883314566058ebbffdfe26ebd10aa6f132d`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d898b31c3c1fac3afde14c13d73fde16f57fa7ebdcf7616e8d25ae6a9400522`  
		Last Modified: Tue, 17 Aug 2021 18:11:42 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af750b396a24c954d09f413c71c4e4afa14794c1bee955c1c789a369175903`  
		Last Modified: Tue, 17 Aug 2021 18:11:51 GMT  
		Size: 60.1 MB (60146413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa9f2969d5dc9b794bffea58a5c6082382fdff260f8ff75d6f9e2c961db7651`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v5

```console
$ docker pull redmine@sha256:6a8a8262c9ba5dc6df9b95e47d236c4a56e765d5e7206667b057f33ddb0615c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194726032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb4106fca334535887ea4971552fa5aaea0d35b1c0cf1905d71a9ea08e067c40`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:49:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 17:49:01 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 17:49:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 17:53:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:53:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:53:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:53:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:53:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:53:37 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:13:24 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:13:24 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:13:25 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:13:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:13:27 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 04 Sep 2021 05:13:28 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 04 Sep 2021 05:13:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:19:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:19:30 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:19:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:19:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:19:32 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:19:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749f126c44247fab04b474652a00ee1a81c976173ad138c2813b3537ae229aa2`  
		Last Modified: Fri, 03 Sep 2021 18:03:49 GMT  
		Size: 20.7 MB (20733279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5467ac924fdbf4db3557de8b61cb7ff89beb1ec1777164bb78d7b65d64cacf8`  
		Last Modified: Fri, 03 Sep 2021 18:03:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393cf7309fe27f7f56257ac9ce482bb381c56ccb9c19f69d4d4997b57222c9ff`  
		Last Modified: Sat, 04 Sep 2021 05:21:45 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be11d890f25506511f19f29d0681b5a3f1d766245f9b66f66ce11ef6d091350`  
		Last Modified: Sat, 04 Sep 2021 05:23:48 GMT  
		Size: 77.0 MB (76964099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d66fc968058c0f81ac20b4b72dc810263d27a00882a33bc6937d4bf264e70b`  
		Last Modified: Sat, 04 Sep 2021 05:22:56 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc65bc4389ff79ecb126cbdfb666aa1ef7a6042fb6d5910586dce556769cfc1`  
		Last Modified: Sat, 04 Sep 2021 05:22:56 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb87b10f6d168b964493cadf04782c246d3af2518a604d9151a6b5bd9d0559a`  
		Last Modified: Sat, 04 Sep 2021 05:22:59 GMT  
		Size: 2.5 MB (2542535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b23ae862be3b962818760d2d169e748782be4625ffdd5425d906ea81cfc5b65`  
		Last Modified: Sat, 04 Sep 2021 05:23:24 GMT  
		Size: 59.3 MB (59253934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e81a5e797f65108167f47139ecdd9c28d1f31e60015d309a6451403781ebe9`  
		Last Modified: Sat, 04 Sep 2021 05:22:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm variant v7

```console
$ docker pull redmine@sha256:1ce637fecc7342eac9b265931b3fd4f518f7fef5045c76c2b78a1a56a3090430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.1 MB (188053631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a8cf2ac1ab1ca8048e539cf138c97ea02acc95a7347ee081bfc7c9d17cff643`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:30:30 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:09:51 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 10:09:52 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 10:09:52 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 10:13:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:13:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:13:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:13:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:13:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:13:56 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 08:39:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 08:47:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:47:41 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 08:47:41 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 08:47:42 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 08:47:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 08:47:44 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 18 Aug 2021 08:47:44 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 18 Aug 2021 08:47:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 08:53:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 08:53:21 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 08:53:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 08:53:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 08:53:22 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 08:53:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79875132dbc48a8386eb9079eb8b50d17399ed33c29a51ac8d7b2f943f3b1ac`  
		Last Modified: Tue, 17 Aug 2021 10:24:54 GMT  
		Size: 9.9 MB (9872248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ce2d51bf7561cb7c360e69499b42694c2e474b2f24d969e4250ac389dd4bec`  
		Last Modified: Tue, 17 Aug 2021 10:24:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fafe7065fd1b5df7801ad1787255f44a163e6d3c870f0a958a250125ce1dd08`  
		Last Modified: Tue, 17 Aug 2021 10:28:25 GMT  
		Size: 20.6 MB (20643690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981a320ed27e237a24cea403bd7a3a89e91b4c9d130c8d0265231346c903de9d`  
		Last Modified: Tue, 17 Aug 2021 10:28:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42323ca32828488d11f463f3a0603a3ed4a1fb7b8289b17c934621f31ee213c`  
		Last Modified: Wed, 18 Aug 2021 08:55:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c1961bc708837e816ebed62de7203ac9138270ba6bc64bc5c2d52cd4ab366`  
		Last Modified: Wed, 18 Aug 2021 08:57:18 GMT  
		Size: 73.3 MB (73264122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cee4e5fec4f8c5645446f2e8a710432595be13da86f5fbdf3158a3595a3ce1`  
		Last Modified: Wed, 18 Aug 2021 08:56:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d73be27d2cb10a7dd343421d0f8588969857af34d723483a7acaa04530ced6c`  
		Last Modified: Wed, 18 Aug 2021 08:56:30 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3208a6775b0410514b52ce235f38e8d1d313d086ab7bcea59a938ab0fecf458`  
		Last Modified: Wed, 18 Aug 2021 08:56:33 GMT  
		Size: 2.5 MB (2542541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c7d111a76cf59342cba1c6af27bbf4d35e6c2c6d310fde9cc692496d3d29fe`  
		Last Modified: Wed, 18 Aug 2021 08:56:57 GMT  
		Size: 59.0 MB (58980543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4218713f4ebdb29d136fd286c2a6a18b20dfd0f5ca3d1ac1d126a1845b4c35`  
		Last Modified: Wed, 18 Aug 2021 08:56:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:e3ef60a632ce1ce8fa577b3c6351d0a0e69879853ca7986e4c752569dd25815a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200851437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0a94c1383818039b4f52eefef06fcdf65663c81d652796470a8f48f458aabc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 12:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:22:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:22:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:22:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:22:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:22:08 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:07:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:10:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:10:29 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:10:29 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:10:29 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:10:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:10:30 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 04 Sep 2021 05:10:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 04 Sep 2021 05:10:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:12:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:12:57 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:12:57 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:12:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:12:57 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:12:58 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64effe010a8ea4895a32764391d02522a7b931f55473493124a03c221c67e1a2`  
		Last Modified: Fri, 03 Sep 2021 12:29:53 GMT  
		Size: 21.3 MB (21308991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9836139b64d4bdf3ba22538bc724ccc0cac2d0eecbca7a1a2ef12c486f39e4a`  
		Last Modified: Fri, 03 Sep 2021 12:29:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30882468c09d5aac3b9b1c5509386ed9719998eb95284bbc3d82c789aa254f31`  
		Last Modified: Sat, 04 Sep 2021 05:14:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4dbf3648e5975fb50a944db4d279e26b6ebf7198bc8d31de2f0008261baf23`  
		Last Modified: Sat, 04 Sep 2021 05:14:58 GMT  
		Size: 79.7 MB (79748437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293357b254319e34c801659daf459389445acf0f2539c9bce79a44bbe2d3d4cd`  
		Last Modified: Sat, 04 Sep 2021 05:14:43 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad43fbff67e07fec524eaed653a3bcdb7bd3b6f419048dbfbce286757f2ba7ca`  
		Last Modified: Sat, 04 Sep 2021 05:14:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01da9a90c6a5199996356ed9a4cb3170c8bda03f389417dd23f0b9c5b2efda9`  
		Last Modified: Sat, 04 Sep 2021 05:14:43 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca3532d249ae81c59125dc16ba10316dc5c88de55bc4e5265316c4483b96bd5`  
		Last Modified: Sat, 04 Sep 2021 05:14:50 GMT  
		Size: 60.1 MB (60067962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479464dd43a6bc15b1fb260205f77204ca832721770128c826642d5838091034`  
		Last Modified: Sat, 04 Sep 2021 05:14:43 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; 386

```console
$ docker pull redmine@sha256:402a1b949fe520850152fd5e9f89a5054a0bf19c7401c1eaf2647b1ebbe28571
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210337068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c254987a2b9238d5290eb7cbfc266a93d46f8bdf1dc5ae5dfe96bfbf37dda774`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:58:09 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 11:58:10 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 11:58:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 12:02:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:02:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:02:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:02:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:02:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:02:08 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 06:08:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 06:11:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 06:11:30 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 06:11:30 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 06:11:31 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 06:11:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 06:11:33 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 04 Sep 2021 06:11:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 04 Sep 2021 06:11:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 06:15:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 06:15:35 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 06:15:35 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 06:15:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 06:15:36 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 06:15:36 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd42d7474f924c3c64bdd4e3ae8097209463c898897a6fc3d869bfad5458a76a`  
		Last Modified: Fri, 03 Sep 2021 12:12:12 GMT  
		Size: 20.9 MB (20910072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6527ea22b515317b992c2ad83317df356fb9c331a328a6ce09dfc29199063b`  
		Last Modified: Fri, 03 Sep 2021 12:12:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf069e6a84c6a25e1afb5b9e31dfc64d2ad9b8b55ba2a7520e4f7279927520c2`  
		Last Modified: Sat, 04 Sep 2021 06:17:05 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0cc32346dcadab6b3e167cef9a31e47f0a876b12badb12c732baf8745f1251`  
		Last Modified: Sat, 04 Sep 2021 06:18:11 GMT  
		Size: 82.6 MB (82598430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebd3aa90d1957b7830014d0c6ecc34b612187385ab9346312286a4ab247d2d6`  
		Last Modified: Sat, 04 Sep 2021 06:17:45 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9d3a64c095be9fe8db6cf8ad9b5afa807ee7c93073316d1976ac25321795c`  
		Last Modified: Sat, 04 Sep 2021 06:17:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862276654eac72ce1c1673e14d3cf576e4f9476853c7f82b2c2e5136c0dcc43b`  
		Last Modified: Sat, 04 Sep 2021 06:17:46 GMT  
		Size: 2.5 MB (2542545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29d2e828d01b96cb1f84e2f99d2535009e0ebb9096bfdcf34f6f79485122691`  
		Last Modified: Sat, 04 Sep 2021 06:17:58 GMT  
		Size: 59.3 MB (59257301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719e1b92f550ad7e184bd476d0c457542be6376901b9e5cbe8f57d387cc349ea`  
		Last Modified: Sat, 04 Sep 2021 06:17:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:76ba83d2d1cfa3f82fa785e5478575a99a38a53d1414113ea123ed39577a4e63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216451518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f349c7ab3350e911d40fee705416e89e9eccad61ab8cd85e65695a56b26707da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:32:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:32:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:19:08 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 10:19:16 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 10:19:22 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 10:27:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:27:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:27:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:27:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:28:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:28:05 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 07:08:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 07:24:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:24:44 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 07:24:49 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 07:24:55 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 07:25:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 07:25:12 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 18 Aug 2021 07:25:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 18 Aug 2021 07:25:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 07:39:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 07:39:52 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 07:39:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 07:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 07:40:00 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 07:40:03 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6540cca707f751654267130c5ff13338c730506cf900ab70cbba8eb8f0774f4`  
		Last Modified: Tue, 17 Aug 2021 10:35:53 GMT  
		Size: 12.7 MB (12704229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cb3d072ea667e9971932f23c9c5ddffe4a2d7c9a645aa1f53235dc8c2e2ae5`  
		Last Modified: Tue, 17 Aug 2021 10:35:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bbc8b7a7166a6ac7a00adc146da227c8d6dc674ba038b1bd1caaaa5584468f`  
		Last Modified: Tue, 17 Aug 2021 10:38:21 GMT  
		Size: 22.0 MB (21985135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72552c8f8b61b54c71444826adc1ca0cdb28ad48ec85cd5581b79cf258e4cd14`  
		Last Modified: Tue, 17 Aug 2021 10:38:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c23f2b8404f22ff77fdf90613e2d326a1ca11b09c1da15ff531aca2664efdc`  
		Last Modified: Wed, 18 Aug 2021 07:42:12 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e655a595012bc1545fa93461a57a24f9329fa8c6c1576b092e6475d0442bfa`  
		Last Modified: Wed, 18 Aug 2021 07:43:04 GMT  
		Size: 87.9 MB (87903030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f301fdd04fb5885924ed256ae7f99fddc5e266f87b414e92f1f119341d562523`  
		Last Modified: Wed, 18 Aug 2021 07:42:44 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c023a3ca82b4c194b93da2ae3b9be66225e6bc6503aec439ccee3b106f65f6`  
		Last Modified: Wed, 18 Aug 2021 07:42:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efdbe020fa9916b2f6c9be80c92d9424b37fc424f7900aed83141ad7bf159f5`  
		Last Modified: Wed, 18 Aug 2021 07:42:45 GMT  
		Size: 2.5 MB (2542550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e3bbf859ce0cdabd1e40486cc7d410356c2c357013319faae5a55c3dbd40bb`  
		Last Modified: Wed, 18 Aug 2021 07:42:54 GMT  
		Size: 60.8 MB (60758612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ac0a0da658722d0b4bc03a74191fb727f0b62b5dfab3306882033a201b0368`  
		Last Modified: Wed, 18 Aug 2021 07:42:44 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; s390x

```console
$ docker pull redmine@sha256:cdf26917ad558633a54acce429f36abd2ddd0d4424b9d15c4fc669bea1f334e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200272176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c11d8f093b4af9cadf313ad7e1583582b92b1bf82154e35ebc133848384629`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 14:05:37 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 14:05:37 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 14:05:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 14:09:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 14:09:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 14:09:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 14:09:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 14:09:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 14:09:13 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 02:43:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 02:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:46:53 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 02:46:53 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 02:46:53 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 02:46:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 02:46:54 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 04 Sep 2021 02:46:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 04 Sep 2021 02:46:58 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 02:49:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 02:49:32 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 02:49:32 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 02:49:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:49:33 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 02:49:33 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386718fbf88b664e88cd07207db2c71a83df8cf7be0efff09692415187356879`  
		Last Modified: Fri, 03 Sep 2021 14:15:25 GMT  
		Size: 21.6 MB (21620271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5421f7853378d4bdf6f6a95b7d634de691057d827e751215fedb21fcb3a5a10`  
		Last Modified: Fri, 03 Sep 2021 14:15:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0767fa5a27a3127ff1c1fb788fd8d545b99e628373bf6e25aa7a0542f2ba120d`  
		Last Modified: Sat, 04 Sep 2021 02:50:46 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7e27777a33e0cfaa0045e72baa090ed992a30e9ccbd342f73f447cf16a6d64`  
		Last Modified: Sat, 04 Sep 2021 02:51:20 GMT  
		Size: 78.9 MB (78942583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5202258d6a3dd2da5df5974ee817b2f5c4334cbaf74e87a1219d6c3be2457d1d`  
		Last Modified: Sat, 04 Sep 2021 02:51:07 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87053cd3998ad25765749b42fd8b9a6a5b53c52eda691fb95c6edc42d927746c`  
		Last Modified: Sat, 04 Sep 2021 02:51:07 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfb04cd2ba8ea9780f771797aff318e1778d05b69c6d286e896e880ac1cc7c`  
		Last Modified: Sat, 04 Sep 2021 02:51:08 GMT  
		Size: 2.5 MB (2542548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4f1397942c0757f88319ba01421887d0f2468e8388dcc41eec932ba54b9bcd`  
		Last Modified: Sat, 04 Sep 2021 02:51:14 GMT  
		Size: 60.6 MB (60586497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ab566e7398ea27c708ece151b329c1397c2736788d3a17313545f1eca3ca7c`  
		Last Modified: Sat, 04 Sep 2021 02:51:07 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-alpine`

```console
$ docker pull redmine@sha256:0ad1450c3b838313dfd32bfdfca410c14c65249473c824333069059afc9e7483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:3753ae94bf08db3964422b5bccfd5c5c7299449727608b420e935214525c335d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.5 MB (153521532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68e057809afe2deac4315e21b86d5179f040e565a7e0a149f2f9ef96799a801`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:46:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Sep 2021 05:46:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Sep 2021 05:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_MAJOR=2.6
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 01 Sep 2021 05:56:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Sep 2021 05:56:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Sep 2021 05:56:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Sep 2021 05:56:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 05:56:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Sep 2021 05:56:40 GMT
CMD ["irb"]
# Wed, 01 Sep 2021 08:06:09 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 01 Sep 2021 08:11:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Wed, 01 Sep 2021 08:11:49 GMT
ENV RAILS_ENV=production
# Wed, 01 Sep 2021 08:11:49 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Sep 2021 08:11:49 GMT
ENV HOME=/home/redmine
# Wed, 01 Sep 2021 08:11:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 01 Sep 2021 08:11:50 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 01 Sep 2021 08:11:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 01 Sep 2021 08:14:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 01 Sep 2021 08:14:44 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 01 Sep 2021 08:16:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 01 Sep 2021 08:16:21 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 01 Sep 2021 08:16:21 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 01 Sep 2021 08:16:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 08:16:21 GMT
EXPOSE 3000
# Wed, 01 Sep 2021 08:16:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439708bfc17dd3e86c8b1415116fcd9de1d32330bdcc8b13fd009f7727844e9`  
		Last Modified: Wed, 01 Sep 2021 05:58:07 GMT  
		Size: 3.6 MB (3581641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260bc7d8cd8f26c27362c4ab1698f2a3e0b0a88516cdfd73a8884747ec12ee`  
		Last Modified: Wed, 01 Sep 2021 05:58:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c1b8b91f648ba1686d802a6e4dd386aa6f1fdc7064a254ffd6b2a9b5bded9c`  
		Last Modified: Wed, 01 Sep 2021 05:58:53 GMT  
		Size: 19.5 MB (19500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e38e14db89c6e839675f8981eeca140c2207e14190fcf5157f4041889857887`  
		Last Modified: Wed, 01 Sep 2021 05:58:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01010032e23eafcf759f8f1e41d523e70c6d201a3e1d8e6dc98f8d932b310429`  
		Last Modified: Wed, 01 Sep 2021 08:17:42 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587f4b0b5d7da47aa8af5a7c020d7dfac150383877edd22c9d355f7bf56582a`  
		Last Modified: Wed, 01 Sep 2021 08:18:19 GMT  
		Size: 66.2 MB (66176616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6a3138f7a3641ed4fbd625ee6680286078a82c61d56652d81d3585df18725f`  
		Last Modified: Wed, 01 Sep 2021 08:18:06 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04fc6e1474161f018d70e99a04a85ae6dd7dc7ab4a80fc8def20e6b9cf3facf`  
		Last Modified: Wed, 01 Sep 2021 08:18:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e3c1a175a4c494bab05d52cc313c1c176fa48b8aa2977ab3d1ceb9623e3a7`  
		Last Modified: Wed, 01 Sep 2021 08:18:06 GMT  
		Size: 2.5 MB (2543740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574bec3ab73b9305002ab74899ca04ca11147bb0ec8af103caa681c59d115d89`  
		Last Modified: Wed, 01 Sep 2021 08:18:12 GMT  
		Size: 58.9 MB (58901320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62eeef7bb697c10446c94aadfa79a706d57b9d52a5d651c3d8bb71560e70eff`  
		Last Modified: Wed, 01 Sep 2021 08:18:06 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0-passenger`

```console
$ docker pull redmine@sha256:e7e408f9eb8f968a37463926e78e44e83295684a50b1478ea9abbe571041e0aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:ebc222582af1442d5c5cac87d0d4744a6abc05204de35b1f0e31ba4705774181
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231316887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6169fca8925a4ef6d5803650edbd59de50a53861d2b81eaec8821a34182de790`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:34:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:34:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:34:16 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:02:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:06:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:06:04 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:06:04 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:06:05 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:06:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:06:06 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 18:06:07 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 18:06:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:08:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:08:34 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:08:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:08:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:08:34 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:08:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 17 Aug 2021 18:08:41 GMT
ENV PASSENGER_VERSION=6.0.10
# Tue, 17 Aug 2021 18:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:09:01 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 17 Aug 2021 18:09:01 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 17 Aug 2021 18:09:01 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d07c054cf634a28fbb441bc93e20e2d4ae0dbaeb43e6aa17ab1c66f1c26b73`  
		Last Modified: Tue, 17 Aug 2021 04:43:06 GMT  
		Size: 21.5 MB (21468054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051a36df400859440c745a4abab787eac2d2318444dcd251750cf3a456ba21`  
		Last Modified: Tue, 17 Aug 2021 04:43:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85f465fea1749f74517e7a2b2c81d5ab6f19157bf460e5e7476d3aa04d2d7e`  
		Last Modified: Tue, 17 Aug 2021 18:10:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f710b25dd48260ef6143f3bbbe5a8211fb635d0408b6e87588e65a7ee41fd42`  
		Last Modified: Tue, 17 Aug 2021 18:12:00 GMT  
		Size: 81.2 MB (81200061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211f3fb54688e3a1a8be31d871a75ed1126c065165edc8a2ba25fa9695157cad`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f792c3664b204ad48d660ca5f20e9883314566058ebbffdfe26ebd10aa6f132d`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d898b31c3c1fac3afde14c13d73fde16f57fa7ebdcf7616e8d25ae6a9400522`  
		Last Modified: Tue, 17 Aug 2021 18:11:42 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af750b396a24c954d09f413c71c4e4afa14794c1bee955c1c789a369175903`  
		Last Modified: Tue, 17 Aug 2021 18:11:51 GMT  
		Size: 60.1 MB (60146413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa9f2969d5dc9b794bffea58a5c6082382fdff260f8ff75d6f9e2c961db7651`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae663f321be159b9674adfe28d63839ebdb4ca128edd43ce2883c5cd7528b39`  
		Last Modified: Tue, 17 Aug 2021 18:12:16 GMT  
		Size: 21.3 MB (21327460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908f0a51a4e0a49ab824df46562bf0c7fb7d2475ef4eee3e1c99849fe05a8283`  
		Last Modified: Tue, 17 Aug 2021 18:12:14 GMT  
		Size: 4.9 MB (4919282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9`

```console
$ docker pull redmine@sha256:e18d85cb2968758d4a74290667b00349a4de0891dd79f66cf424edf05db360c3
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
$ docker pull redmine@sha256:d6d905b7ab421a941dc5c23c46f5bd46fe613971f7f61ea346eef7abf660491e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.1 MB (205070145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58b6a0822eb22f16e48160adfb284d9f5ccadf6906b0424b6759a186d5af659d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:34:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:34:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:34:16 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:02:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:06:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:06:04 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:06:04 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:06:05 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:06:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:06:06 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 18:06:07 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 18:06:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:08:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:08:34 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:08:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:08:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:08:34 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:08:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d07c054cf634a28fbb441bc93e20e2d4ae0dbaeb43e6aa17ab1c66f1c26b73`  
		Last Modified: Tue, 17 Aug 2021 04:43:06 GMT  
		Size: 21.5 MB (21468054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051a36df400859440c745a4abab787eac2d2318444dcd251750cf3a456ba21`  
		Last Modified: Tue, 17 Aug 2021 04:43:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85f465fea1749f74517e7a2b2c81d5ab6f19157bf460e5e7476d3aa04d2d7e`  
		Last Modified: Tue, 17 Aug 2021 18:10:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f710b25dd48260ef6143f3bbbe5a8211fb635d0408b6e87588e65a7ee41fd42`  
		Last Modified: Tue, 17 Aug 2021 18:12:00 GMT  
		Size: 81.2 MB (81200061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211f3fb54688e3a1a8be31d871a75ed1126c065165edc8a2ba25fa9695157cad`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f792c3664b204ad48d660ca5f20e9883314566058ebbffdfe26ebd10aa6f132d`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d898b31c3c1fac3afde14c13d73fde16f57fa7ebdcf7616e8d25ae6a9400522`  
		Last Modified: Tue, 17 Aug 2021 18:11:42 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af750b396a24c954d09f413c71c4e4afa14794c1bee955c1c789a369175903`  
		Last Modified: Tue, 17 Aug 2021 18:11:51 GMT  
		Size: 60.1 MB (60146413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa9f2969d5dc9b794bffea58a5c6082382fdff260f8ff75d6f9e2c961db7651`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm variant v5

```console
$ docker pull redmine@sha256:6a8a8262c9ba5dc6df9b95e47d236c4a56e765d5e7206667b057f33ddb0615c7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.7 MB (194726032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb4106fca334535887ea4971552fa5aaea0d35b1c0cf1905d71a9ea08e067c40`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:49:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 17:49:01 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 17:49:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 17:53:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:53:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:53:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:53:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:53:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:53:37 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:13:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:13:24 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:13:24 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:13:25 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:13:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:13:27 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 04 Sep 2021 05:13:28 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 04 Sep 2021 05:13:33 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:19:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:19:30 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:19:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:19:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:19:32 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:19:32 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749f126c44247fab04b474652a00ee1a81c976173ad138c2813b3537ae229aa2`  
		Last Modified: Fri, 03 Sep 2021 18:03:49 GMT  
		Size: 20.7 MB (20733279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5467ac924fdbf4db3557de8b61cb7ff89beb1ec1777164bb78d7b65d64cacf8`  
		Last Modified: Fri, 03 Sep 2021 18:03:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393cf7309fe27f7f56257ac9ce482bb381c56ccb9c19f69d4d4997b57222c9ff`  
		Last Modified: Sat, 04 Sep 2021 05:21:45 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be11d890f25506511f19f29d0681b5a3f1d766245f9b66f66ce11ef6d091350`  
		Last Modified: Sat, 04 Sep 2021 05:23:48 GMT  
		Size: 77.0 MB (76964099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d66fc968058c0f81ac20b4b72dc810263d27a00882a33bc6937d4bf264e70b`  
		Last Modified: Sat, 04 Sep 2021 05:22:56 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc65bc4389ff79ecb126cbdfb666aa1ef7a6042fb6d5910586dce556769cfc1`  
		Last Modified: Sat, 04 Sep 2021 05:22:56 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb87b10f6d168b964493cadf04782c246d3af2518a604d9151a6b5bd9d0559a`  
		Last Modified: Sat, 04 Sep 2021 05:22:59 GMT  
		Size: 2.5 MB (2542535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b23ae862be3b962818760d2d169e748782be4625ffdd5425d906ea81cfc5b65`  
		Last Modified: Sat, 04 Sep 2021 05:23:24 GMT  
		Size: 59.3 MB (59253934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4e81a5e797f65108167f47139ecdd9c28d1f31e60015d309a6451403781ebe9`  
		Last Modified: Sat, 04 Sep 2021 05:22:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm variant v7

```console
$ docker pull redmine@sha256:1ce637fecc7342eac9b265931b3fd4f518f7fef5045c76c2b78a1a56a3090430
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.1 MB (188053631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a8cf2ac1ab1ca8048e539cf138c97ea02acc95a7347ee081bfc7c9d17cff643`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:30:30 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:09:51 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 10:09:52 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 10:09:52 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 10:13:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:13:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:13:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:13:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:13:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:13:56 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 08:39:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 08:47:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:47:41 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 08:47:41 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 08:47:42 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 08:47:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 08:47:44 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 18 Aug 2021 08:47:44 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 18 Aug 2021 08:47:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 08:53:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 08:53:21 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 08:53:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 08:53:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 08:53:22 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 08:53:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79875132dbc48a8386eb9079eb8b50d17399ed33c29a51ac8d7b2f943f3b1ac`  
		Last Modified: Tue, 17 Aug 2021 10:24:54 GMT  
		Size: 9.9 MB (9872248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ce2d51bf7561cb7c360e69499b42694c2e474b2f24d969e4250ac389dd4bec`  
		Last Modified: Tue, 17 Aug 2021 10:24:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fafe7065fd1b5df7801ad1787255f44a163e6d3c870f0a958a250125ce1dd08`  
		Last Modified: Tue, 17 Aug 2021 10:28:25 GMT  
		Size: 20.6 MB (20643690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981a320ed27e237a24cea403bd7a3a89e91b4c9d130c8d0265231346c903de9d`  
		Last Modified: Tue, 17 Aug 2021 10:28:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42323ca32828488d11f463f3a0603a3ed4a1fb7b8289b17c934621f31ee213c`  
		Last Modified: Wed, 18 Aug 2021 08:55:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:148c1961bc708837e816ebed62de7203ac9138270ba6bc64bc5c2d52cd4ab366`  
		Last Modified: Wed, 18 Aug 2021 08:57:18 GMT  
		Size: 73.3 MB (73264122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99cee4e5fec4f8c5645446f2e8a710432595be13da86f5fbdf3158a3595a3ce1`  
		Last Modified: Wed, 18 Aug 2021 08:56:30 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d73be27d2cb10a7dd343421d0f8588969857af34d723483a7acaa04530ced6c`  
		Last Modified: Wed, 18 Aug 2021 08:56:30 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3208a6775b0410514b52ce235f38e8d1d313d086ab7bcea59a938ab0fecf458`  
		Last Modified: Wed, 18 Aug 2021 08:56:33 GMT  
		Size: 2.5 MB (2542541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c7d111a76cf59342cba1c6af27bbf4d35e6c2c6d310fde9cc692496d3d29fe`  
		Last Modified: Wed, 18 Aug 2021 08:56:57 GMT  
		Size: 59.0 MB (58980543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4218713f4ebdb29d136fd286c2a6a18b20dfd0f5ca3d1ac1d126a1845b4c35`  
		Last Modified: Wed, 18 Aug 2021 08:56:29 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:e3ef60a632ce1ce8fa577b3c6351d0a0e69879853ca7986e4c752569dd25815a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200851437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d0a94c1383818039b4f52eefef06fcdf65663c81d652796470a8f48f458aabc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 12:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:22:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:22:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:22:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:22:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:22:08 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:07:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:10:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:10:29 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:10:29 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:10:29 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:10:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:10:30 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 04 Sep 2021 05:10:31 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 04 Sep 2021 05:10:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:12:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:12:57 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:12:57 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:12:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:12:57 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:12:58 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64effe010a8ea4895a32764391d02522a7b931f55473493124a03c221c67e1a2`  
		Last Modified: Fri, 03 Sep 2021 12:29:53 GMT  
		Size: 21.3 MB (21308991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9836139b64d4bdf3ba22538bc724ccc0cac2d0eecbca7a1a2ef12c486f39e4a`  
		Last Modified: Fri, 03 Sep 2021 12:29:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30882468c09d5aac3b9b1c5509386ed9719998eb95284bbc3d82c789aa254f31`  
		Last Modified: Sat, 04 Sep 2021 05:14:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4dbf3648e5975fb50a944db4d279e26b6ebf7198bc8d31de2f0008261baf23`  
		Last Modified: Sat, 04 Sep 2021 05:14:58 GMT  
		Size: 79.7 MB (79748437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293357b254319e34c801659daf459389445acf0f2539c9bce79a44bbe2d3d4cd`  
		Last Modified: Sat, 04 Sep 2021 05:14:43 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad43fbff67e07fec524eaed653a3bcdb7bd3b6f419048dbfbce286757f2ba7ca`  
		Last Modified: Sat, 04 Sep 2021 05:14:43 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01da9a90c6a5199996356ed9a4cb3170c8bda03f389417dd23f0b9c5b2efda9`  
		Last Modified: Sat, 04 Sep 2021 05:14:43 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca3532d249ae81c59125dc16ba10316dc5c88de55bc4e5265316c4483b96bd5`  
		Last Modified: Sat, 04 Sep 2021 05:14:50 GMT  
		Size: 60.1 MB (60067962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479464dd43a6bc15b1fb260205f77204ca832721770128c826642d5838091034`  
		Last Modified: Sat, 04 Sep 2021 05:14:43 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; 386

```console
$ docker pull redmine@sha256:402a1b949fe520850152fd5e9f89a5054a0bf19c7401c1eaf2647b1ebbe28571
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210337068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c254987a2b9238d5290eb7cbfc266a93d46f8bdf1dc5ae5dfe96bfbf37dda774`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:58:09 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 11:58:10 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 11:58:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 12:02:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:02:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:02:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:02:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:02:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:02:08 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 06:08:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 06:11:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 06:11:30 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 06:11:30 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 06:11:31 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 06:11:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 06:11:33 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 04 Sep 2021 06:11:33 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 04 Sep 2021 06:11:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 06:15:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 06:15:35 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 06:15:35 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 06:15:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 06:15:36 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 06:15:36 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd42d7474f924c3c64bdd4e3ae8097209463c898897a6fc3d869bfad5458a76a`  
		Last Modified: Fri, 03 Sep 2021 12:12:12 GMT  
		Size: 20.9 MB (20910072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6527ea22b515317b992c2ad83317df356fb9c331a328a6ce09dfc29199063b`  
		Last Modified: Fri, 03 Sep 2021 12:12:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf069e6a84c6a25e1afb5b9e31dfc64d2ad9b8b55ba2a7520e4f7279927520c2`  
		Last Modified: Sat, 04 Sep 2021 06:17:05 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb0cc32346dcadab6b3e167cef9a31e47f0a876b12badb12c732baf8745f1251`  
		Last Modified: Sat, 04 Sep 2021 06:18:11 GMT  
		Size: 82.6 MB (82598430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebd3aa90d1957b7830014d0c6ecc34b612187385ab9346312286a4ab247d2d6`  
		Last Modified: Sat, 04 Sep 2021 06:17:45 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce9d3a64c095be9fe8db6cf8ad9b5afa807ee7c93073316d1976ac25321795c`  
		Last Modified: Sat, 04 Sep 2021 06:17:45 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862276654eac72ce1c1673e14d3cf576e4f9476853c7f82b2c2e5136c0dcc43b`  
		Last Modified: Sat, 04 Sep 2021 06:17:46 GMT  
		Size: 2.5 MB (2542545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29d2e828d01b96cb1f84e2f99d2535009e0ebb9096bfdcf34f6f79485122691`  
		Last Modified: Sat, 04 Sep 2021 06:17:58 GMT  
		Size: 59.3 MB (59257301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719e1b92f550ad7e184bd476d0c457542be6376901b9e5cbe8f57d387cc349ea`  
		Last Modified: Sat, 04 Sep 2021 06:17:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; ppc64le

```console
$ docker pull redmine@sha256:76ba83d2d1cfa3f82fa785e5478575a99a38a53d1414113ea123ed39577a4e63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216451518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f349c7ab3350e911d40fee705416e89e9eccad61ab8cd85e65695a56b26707da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:32:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:32:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:19:08 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 10:19:16 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 10:19:22 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 10:27:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:27:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:27:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:27:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:28:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:28:05 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 07:08:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 07:24:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:24:44 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 07:24:49 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 07:24:55 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 07:25:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 07:25:12 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 18 Aug 2021 07:25:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 18 Aug 2021 07:25:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 07:39:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 07:39:52 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 07:39:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 07:39:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 07:40:00 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 07:40:03 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6540cca707f751654267130c5ff13338c730506cf900ab70cbba8eb8f0774f4`  
		Last Modified: Tue, 17 Aug 2021 10:35:53 GMT  
		Size: 12.7 MB (12704229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cb3d072ea667e9971932f23c9c5ddffe4a2d7c9a645aa1f53235dc8c2e2ae5`  
		Last Modified: Tue, 17 Aug 2021 10:35:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bbc8b7a7166a6ac7a00adc146da227c8d6dc674ba038b1bd1caaaa5584468f`  
		Last Modified: Tue, 17 Aug 2021 10:38:21 GMT  
		Size: 22.0 MB (21985135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72552c8f8b61b54c71444826adc1ca0cdb28ad48ec85cd5581b79cf258e4cd14`  
		Last Modified: Tue, 17 Aug 2021 10:38:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c23f2b8404f22ff77fdf90613e2d326a1ca11b09c1da15ff531aca2664efdc`  
		Last Modified: Wed, 18 Aug 2021 07:42:12 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e655a595012bc1545fa93461a57a24f9329fa8c6c1576b092e6475d0442bfa`  
		Last Modified: Wed, 18 Aug 2021 07:43:04 GMT  
		Size: 87.9 MB (87903030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f301fdd04fb5885924ed256ae7f99fddc5e266f87b414e92f1f119341d562523`  
		Last Modified: Wed, 18 Aug 2021 07:42:44 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c023a3ca82b4c194b93da2ae3b9be66225e6bc6503aec439ccee3b106f65f6`  
		Last Modified: Wed, 18 Aug 2021 07:42:44 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efdbe020fa9916b2f6c9be80c92d9424b37fc424f7900aed83141ad7bf159f5`  
		Last Modified: Wed, 18 Aug 2021 07:42:45 GMT  
		Size: 2.5 MB (2542550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e3bbf859ce0cdabd1e40486cc7d410356c2c357013319faae5a55c3dbd40bb`  
		Last Modified: Wed, 18 Aug 2021 07:42:54 GMT  
		Size: 60.8 MB (60758612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ac0a0da658722d0b4bc03a74191fb727f0b62b5dfab3306882033a201b0368`  
		Last Modified: Wed, 18 Aug 2021 07:42:44 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; s390x

```console
$ docker pull redmine@sha256:cdf26917ad558633a54acce429f36abd2ddd0d4424b9d15c4fc669bea1f334e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200272176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2c11d8f093b4af9cadf313ad7e1583582b92b1bf82154e35ebc133848384629`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 14:05:37 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 14:05:37 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 14:05:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 14:09:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 14:09:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 14:09:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 14:09:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 14:09:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 14:09:13 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 02:43:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 02:46:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:46:53 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 02:46:53 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 02:46:53 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 02:46:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 02:46:54 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 04 Sep 2021 02:46:54 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 04 Sep 2021 02:46:58 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 02:49:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 02:49:32 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 02:49:32 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 02:49:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:49:33 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 02:49:33 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386718fbf88b664e88cd07207db2c71a83df8cf7be0efff09692415187356879`  
		Last Modified: Fri, 03 Sep 2021 14:15:25 GMT  
		Size: 21.6 MB (21620271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5421f7853378d4bdf6f6a95b7d634de691057d827e751215fedb21fcb3a5a10`  
		Last Modified: Fri, 03 Sep 2021 14:15:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0767fa5a27a3127ff1c1fb788fd8d545b99e628373bf6e25aa7a0542f2ba120d`  
		Last Modified: Sat, 04 Sep 2021 02:50:46 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac7e27777a33e0cfaa0045e72baa090ed992a30e9ccbd342f73f447cf16a6d64`  
		Last Modified: Sat, 04 Sep 2021 02:51:20 GMT  
		Size: 78.9 MB (78942583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5202258d6a3dd2da5df5974ee817b2f5c4334cbaf74e87a1219d6c3be2457d1d`  
		Last Modified: Sat, 04 Sep 2021 02:51:07 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87053cd3998ad25765749b42fd8b9a6a5b53c52eda691fb95c6edc42d927746c`  
		Last Modified: Sat, 04 Sep 2021 02:51:07 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08dfb04cd2ba8ea9780f771797aff318e1778d05b69c6d286e896e880ac1cc7c`  
		Last Modified: Sat, 04 Sep 2021 02:51:08 GMT  
		Size: 2.5 MB (2542548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db4f1397942c0757f88319ba01421887d0f2468e8388dcc41eec932ba54b9bcd`  
		Last Modified: Sat, 04 Sep 2021 02:51:14 GMT  
		Size: 60.6 MB (60586497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71ab566e7398ea27c708ece151b329c1397c2736788d3a17313545f1eca3ca7c`  
		Last Modified: Sat, 04 Sep 2021 02:51:07 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9-alpine`

```console
$ docker pull redmine@sha256:0ad1450c3b838313dfd32bfdfca410c14c65249473c824333069059afc9e7483
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0.9-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:3753ae94bf08db3964422b5bccfd5c5c7299449727608b420e935214525c335d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.5 MB (153521532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68e057809afe2deac4315e21b86d5179f040e565a7e0a149f2f9ef96799a801`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:46:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Sep 2021 05:46:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Sep 2021 05:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_MAJOR=2.6
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 01 Sep 2021 05:56:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Sep 2021 05:56:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Sep 2021 05:56:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Sep 2021 05:56:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 05:56:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Sep 2021 05:56:40 GMT
CMD ["irb"]
# Wed, 01 Sep 2021 08:06:09 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 01 Sep 2021 08:11:48 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript-fonts 		imagemagick6 	;
# Wed, 01 Sep 2021 08:11:49 GMT
ENV RAILS_ENV=production
# Wed, 01 Sep 2021 08:11:49 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Sep 2021 08:11:49 GMT
ENV HOME=/home/redmine
# Wed, 01 Sep 2021 08:11:50 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 01 Sep 2021 08:11:50 GMT
ENV REDMINE_VERSION=4.0.9
# Wed, 01 Sep 2021 08:11:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Wed, 01 Sep 2021 08:14:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 01 Sep 2021 08:14:44 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 01 Sep 2021 08:16:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 		imagemagick6-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 01 Sep 2021 08:16:21 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 01 Sep 2021 08:16:21 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 01 Sep 2021 08:16:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 08:16:21 GMT
EXPOSE 3000
# Wed, 01 Sep 2021 08:16:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439708bfc17dd3e86c8b1415116fcd9de1d32330bdcc8b13fd009f7727844e9`  
		Last Modified: Wed, 01 Sep 2021 05:58:07 GMT  
		Size: 3.6 MB (3581641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260bc7d8cd8f26c27362c4ab1698f2a3e0b0a88516cdfd73a8884747ec12ee`  
		Last Modified: Wed, 01 Sep 2021 05:58:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c1b8b91f648ba1686d802a6e4dd386aa6f1fdc7064a254ffd6b2a9b5bded9c`  
		Last Modified: Wed, 01 Sep 2021 05:58:53 GMT  
		Size: 19.5 MB (19500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e38e14db89c6e839675f8981eeca140c2207e14190fcf5157f4041889857887`  
		Last Modified: Wed, 01 Sep 2021 05:58:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01010032e23eafcf759f8f1e41d523e70c6d201a3e1d8e6dc98f8d932b310429`  
		Last Modified: Wed, 01 Sep 2021 08:17:42 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4587f4b0b5d7da47aa8af5a7c020d7dfac150383877edd22c9d355f7bf56582a`  
		Last Modified: Wed, 01 Sep 2021 08:18:19 GMT  
		Size: 66.2 MB (66176616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6a3138f7a3641ed4fbd625ee6680286078a82c61d56652d81d3585df18725f`  
		Last Modified: Wed, 01 Sep 2021 08:18:06 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e04fc6e1474161f018d70e99a04a85ae6dd7dc7ab4a80fc8def20e6b9cf3facf`  
		Last Modified: Wed, 01 Sep 2021 08:18:06 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70e3c1a175a4c494bab05d52cc313c1c176fa48b8aa2977ab3d1ceb9623e3a7`  
		Last Modified: Wed, 01 Sep 2021 08:18:06 GMT  
		Size: 2.5 MB (2543740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574bec3ab73b9305002ab74899ca04ca11147bb0ec8af103caa681c59d115d89`  
		Last Modified: Wed, 01 Sep 2021 08:18:12 GMT  
		Size: 58.9 MB (58901320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d62eeef7bb697c10446c94aadfa79a706d57b9d52a5d651c3d8bb71560e70eff`  
		Last Modified: Wed, 01 Sep 2021 08:18:06 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.0.9-passenger`

```console
$ docker pull redmine@sha256:e7e408f9eb8f968a37463926e78e44e83295684a50b1478ea9abbe571041e0aa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.0.9-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:ebc222582af1442d5c5cac87d0d4744a6abc05204de35b1f0e31ba4705774181
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231316887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6169fca8925a4ef6d5803650edbd59de50a53861d2b81eaec8821a34182de790`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:34:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:34:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:34:16 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:02:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:06:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:06:04 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:06:04 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:06:05 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:06:06 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:06:06 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 18:06:07 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 18:06:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:08:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:08:34 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:08:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:08:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:08:34 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:08:34 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 17 Aug 2021 18:08:41 GMT
ENV PASSENGER_VERSION=6.0.10
# Tue, 17 Aug 2021 18:08:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:09:01 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 17 Aug 2021 18:09:01 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 17 Aug 2021 18:09:01 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d07c054cf634a28fbb441bc93e20e2d4ae0dbaeb43e6aa17ab1c66f1c26b73`  
		Last Modified: Tue, 17 Aug 2021 04:43:06 GMT  
		Size: 21.5 MB (21468054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051a36df400859440c745a4abab787eac2d2318444dcd251750cf3a456ba21`  
		Last Modified: Tue, 17 Aug 2021 04:43:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85f465fea1749f74517e7a2b2c81d5ab6f19157bf460e5e7476d3aa04d2d7e`  
		Last Modified: Tue, 17 Aug 2021 18:10:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f710b25dd48260ef6143f3bbbe5a8211fb635d0408b6e87588e65a7ee41fd42`  
		Last Modified: Tue, 17 Aug 2021 18:12:00 GMT  
		Size: 81.2 MB (81200061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211f3fb54688e3a1a8be31d871a75ed1126c065165edc8a2ba25fa9695157cad`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f792c3664b204ad48d660ca5f20e9883314566058ebbffdfe26ebd10aa6f132d`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d898b31c3c1fac3afde14c13d73fde16f57fa7ebdcf7616e8d25ae6a9400522`  
		Last Modified: Tue, 17 Aug 2021 18:11:42 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05af750b396a24c954d09f413c71c4e4afa14794c1bee955c1c789a369175903`  
		Last Modified: Tue, 17 Aug 2021 18:11:51 GMT  
		Size: 60.1 MB (60146413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa9f2969d5dc9b794bffea58a5c6082382fdff260f8ff75d6f9e2c961db7651`  
		Last Modified: Tue, 17 Aug 2021 18:11:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae663f321be159b9674adfe28d63839ebdb4ca128edd43ce2883c5cd7528b39`  
		Last Modified: Tue, 17 Aug 2021 18:12:16 GMT  
		Size: 21.3 MB (21327460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908f0a51a4e0a49ab824df46562bf0c7fb7d2475ef4eee3e1c99849fe05a8283`  
		Last Modified: Tue, 17 Aug 2021 18:12:14 GMT  
		Size: 4.9 MB (4919282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1`

```console
$ docker pull redmine@sha256:0c687f9fbe88a3381bd4a91a538f73df6890ea6c43f75c9fe40e859d08af63d7
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
$ docker pull redmine@sha256:79620ad17c6061c101fe3a07a8fad3594fa291ff144352a9a8df130081839091
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.7 MB (206651817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf5593c96102abe227b98e4b51d5bbb46aff23a46b119a77903a081fc0a5ed2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:34:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:34:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:34:16 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:02:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:03:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:03:29 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:03:30 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:03:30 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:03:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:03:32 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 18:03:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 18:03:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:04:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:04:40 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:04:41 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:04:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:04:41 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:04:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d07c054cf634a28fbb441bc93e20e2d4ae0dbaeb43e6aa17ab1c66f1c26b73`  
		Last Modified: Tue, 17 Aug 2021 04:43:06 GMT  
		Size: 21.5 MB (21468054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051a36df400859440c745a4abab787eac2d2318444dcd251750cf3a456ba21`  
		Last Modified: Tue, 17 Aug 2021 04:43:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85f465fea1749f74517e7a2b2c81d5ab6f19157bf460e5e7476d3aa04d2d7e`  
		Last Modified: Tue, 17 Aug 2021 18:10:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00de815fcdb1a6feb851a112e729207c26f6cbdd814903f8d7fb5d5b3618832`  
		Last Modified: Tue, 17 Aug 2021 18:11:13 GMT  
		Size: 94.1 MB (94088503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6dd4cade454377a496d734498902101532e5a3fc75e1d464b07f8e7d0b229e`  
		Last Modified: Tue, 17 Aug 2021 18:10:50 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb35b58efaa3018c9928e6ceaf42ba28c690355758565edd2ee14da281d74139`  
		Last Modified: Tue, 17 Aug 2021 18:10:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5ef1b243346c0a06cbf794b2195499317d58250e4485b7822abf270b4d229f`  
		Last Modified: Tue, 17 Aug 2021 18:10:52 GMT  
		Size: 2.7 MB (2749062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004c2031ebe227cb058ab066f0a87358cb28ebd69895c9a44ebfefbbc670845`  
		Last Modified: Tue, 17 Aug 2021 18:10:59 GMT  
		Size: 48.6 MB (48633124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b825d8abfc9574a6c4b650575e0ff513214b45b4f07756a300b46cb0f26ddeb`  
		Last Modified: Tue, 17 Aug 2021 18:10:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v5

```console
$ docker pull redmine@sha256:820710f4ac5c3e27c19513944d6efeb5cc8f227858222a3e2b6bfe5b5a9ea542
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210669898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670ad4b2f9ed3a1d97388b2a0dd55a15f2c147c722ff61167b3c50813fa5a7c8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:49:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 17:49:01 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 17:49:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 17:53:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:53:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:53:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:53:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:53:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:53:37 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:06:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:06:13 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:06:13 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:06:14 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:06:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:06:16 GMT
ENV REDMINE_VERSION=4.1.4
# Sat, 04 Sep 2021 05:06:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Sat, 04 Sep 2021 05:06:22 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:11:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:11:59 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:12:00 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:12:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:12:01 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:12:01 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749f126c44247fab04b474652a00ee1a81c976173ad138c2813b3537ae229aa2`  
		Last Modified: Fri, 03 Sep 2021 18:03:49 GMT  
		Size: 20.7 MB (20733279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5467ac924fdbf4db3557de8b61cb7ff89beb1ec1777164bb78d7b65d64cacf8`  
		Last Modified: Fri, 03 Sep 2021 18:03:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393cf7309fe27f7f56257ac9ce482bb381c56ccb9c19f69d4d4997b57222c9ff`  
		Last Modified: Sat, 04 Sep 2021 05:21:45 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d532998c02f6c9a866287ce631e361dcf9745dc03e5c9d074b7153f3b7c29`  
		Last Modified: Sat, 04 Sep 2021 05:22:43 GMT  
		Size: 89.6 MB (89576618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171faf2191b22aac8fd9f161aaa2b916ca52128abcf3e355f8aeeaaaa110ffa0`  
		Last Modified: Sat, 04 Sep 2021 05:21:43 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc60bb6f99d05a9fade0765ecb9cebdb152ab117e2c87eb6940510af32e0dd`  
		Last Modified: Sat, 04 Sep 2021 05:21:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8178ad802a290b21fbb51dbc75475bd793fb3e655da90a110ce533bc2b33c3a`  
		Last Modified: Sat, 04 Sep 2021 05:21:47 GMT  
		Size: 2.7 MB (2749062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebda4f1e758b5be42d3d195c12360777d7fe3dadacc09cc41e188c93162e2b5`  
		Last Modified: Sat, 04 Sep 2021 05:22:11 GMT  
		Size: 62.4 MB (62378756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11218622960555ad9afcc7d2960f59429b83ad60b704d5fa537823ee81ddd9`  
		Last Modified: Sat, 04 Sep 2021 05:21:43 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:99bf6eb7a4c90631440b9f5a1518978033c3d76c412f9ba72b4c1e9746ee78aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203844212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194ecb467b361afc105e966f3bfc18b722f741c1d231b551a82679b4f0d508b4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:30:30 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:09:51 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 10:09:52 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 10:09:52 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 10:13:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:13:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:13:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:13:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:13:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:13:56 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 08:39:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 08:40:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:40:54 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 08:40:55 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 08:40:55 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 08:40:57 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 08:40:57 GMT
ENV REDMINE_VERSION=4.1.4
# Wed, 18 Aug 2021 08:40:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Wed, 18 Aug 2021 08:41:04 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 08:46:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 08:46:20 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 08:46:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 08:46:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 08:46:21 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 08:46:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79875132dbc48a8386eb9079eb8b50d17399ed33c29a51ac8d7b2f943f3b1ac`  
		Last Modified: Tue, 17 Aug 2021 10:24:54 GMT  
		Size: 9.9 MB (9872248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ce2d51bf7561cb7c360e69499b42694c2e474b2f24d969e4250ac389dd4bec`  
		Last Modified: Tue, 17 Aug 2021 10:24:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fafe7065fd1b5df7801ad1787255f44a163e6d3c870f0a958a250125ce1dd08`  
		Last Modified: Tue, 17 Aug 2021 10:28:25 GMT  
		Size: 20.6 MB (20643690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981a320ed27e237a24cea403bd7a3a89e91b4c9d130c8d0265231346c903de9d`  
		Last Modified: Tue, 17 Aug 2021 10:28:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42323ca32828488d11f463f3a0603a3ed4a1fb7b8289b17c934621f31ee213c`  
		Last Modified: Wed, 18 Aug 2021 08:55:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc71522bb4b2c7a1ca1650d66db744b9b79c3abaf22c9796b25c400fe05e120f`  
		Last Modified: Wed, 18 Aug 2021 08:56:16 GMT  
		Size: 85.6 MB (85590409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8e1c03b25c8d1b7b70ae7adb351fa6fcbfeca38a7725de12115c5787b40951`  
		Last Modified: Wed, 18 Aug 2021 08:55:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579e678098ca93cf89148b75bdedc18658c8f6d76a5d3e962d2f6f1b5ed8d5e5`  
		Last Modified: Wed, 18 Aug 2021 08:55:20 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bfd4a46d9c2e31abbe07d0c6c71cd11f25f72683fbc1a3b8e84e8f49045e90`  
		Last Modified: Wed, 18 Aug 2021 08:55:23 GMT  
		Size: 2.7 MB (2749056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14f14c8dc1382cf377e8aa751c5e3d71ed0a79f11c866eb1fb8c9d305151b9`  
		Last Modified: Wed, 18 Aug 2021 08:55:49 GMT  
		Size: 62.2 MB (62238320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92a4cdd95e2f9e715a4ad8a056c9b2d67ed5798007b5125dcbfedea161398e3`  
		Last Modified: Wed, 18 Aug 2021 08:55:20 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:03050db75dcf9c5f92a42065092427328e1ff95b14cfe4eb0145b34b1772ec3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217545418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5832c6b908dc3582d811982b31cb0736beaf8b988b4d1e3d40b27a7ea6171743`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 12:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:22:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:22:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:22:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:22:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:22:08 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:07:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:07:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:07:50 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:07:50 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:07:50 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:07:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:07:51 GMT
ENV REDMINE_VERSION=4.1.4
# Sat, 04 Sep 2021 05:07:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Sat, 04 Sep 2021 05:07:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:09:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:10:00 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:10:00 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:10:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:10:00 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:10:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64effe010a8ea4895a32764391d02522a7b931f55473493124a03c221c67e1a2`  
		Last Modified: Fri, 03 Sep 2021 12:29:53 GMT  
		Size: 21.3 MB (21308991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9836139b64d4bdf3ba22538bc724ccc0cac2d0eecbca7a1a2ef12c486f39e4a`  
		Last Modified: Fri, 03 Sep 2021 12:29:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30882468c09d5aac3b9b1c5509386ed9719998eb95284bbc3d82c789aa254f31`  
		Last Modified: Sat, 04 Sep 2021 05:14:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fbd53cdf3d8fd12dd9858d43a5f75ff6934ea03373505bcdf9f61fbe3b4385`  
		Last Modified: Sat, 04 Sep 2021 05:14:26 GMT  
		Size: 92.6 MB (92610545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1064cbb77106f38550f68ad21538df88b0d2e80c74c5a33cc6d599dade25a2`  
		Last Modified: Sat, 04 Sep 2021 05:14:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd94a5f71d8c4419f9e66c36c86d1835b66aef7dcd9ae2d4cbec8f16e207ceb`  
		Last Modified: Sat, 04 Sep 2021 05:14:08 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7f8eb2d3ae7a8b942835c3976c1e611f9bfef9f55cd17d83e074b8dec393df`  
		Last Modified: Sat, 04 Sep 2021 05:14:09 GMT  
		Size: 2.7 MB (2749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbfe9573c141edbf4f99af468d979c15bcf21f10e415885cc18d04c8fd2aac5`  
		Last Modified: Sat, 04 Sep 2021 05:14:16 GMT  
		Size: 63.7 MB (63693325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc8b6de7c6d30b4b38ba818b339df7b8e1c624c9ec8cf341492badeb539cc43`  
		Last Modified: Sat, 04 Sep 2021 05:14:08 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; 386

```console
$ docker pull redmine@sha256:b19011e8b39cc7ec6a822049f9e031cb344fb4ac238b0b54cf46fad11699d06d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213004456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8865b21d35b0e141a83ad423da3570e6f614d64a4abde308461caafeb197b61c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:58:09 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 11:58:10 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 11:58:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 12:02:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:02:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:02:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:02:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:02:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:02:08 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 06:08:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 06:08:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 06:08:53 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 06:08:53 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 06:08:53 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 06:08:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 06:08:56 GMT
ENV REDMINE_VERSION=4.1.4
# Sat, 04 Sep 2021 06:08:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Sat, 04 Sep 2021 06:09:02 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 06:10:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 06:10:29 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 06:10:30 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 06:10:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 06:10:30 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 06:10:31 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd42d7474f924c3c64bdd4e3ae8097209463c898897a6fc3d869bfad5458a76a`  
		Last Modified: Fri, 03 Sep 2021 12:12:12 GMT  
		Size: 20.9 MB (20910072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6527ea22b515317b992c2ad83317df356fb9c331a328a6ce09dfc29199063b`  
		Last Modified: Fri, 03 Sep 2021 12:12:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf069e6a84c6a25e1afb5b9e31dfc64d2ad9b8b55ba2a7520e4f7279927520c2`  
		Last Modified: Sat, 04 Sep 2021 06:17:05 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3471af7fd62676cb8bebe5257d6f29e9936bc1b6ec48ff1730a6c82b676dd1`  
		Last Modified: Sat, 04 Sep 2021 06:17:32 GMT  
		Size: 95.7 MB (95702608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f5db09056e5bb6fce4854295752a64f439c54c2acb62bdbf0b180de138488b`  
		Last Modified: Sat, 04 Sep 2021 06:17:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0183266bad02bc74edb95f172168ca409f6296887c8bec3dc867794923cf4c`  
		Last Modified: Sat, 04 Sep 2021 06:17:02 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d104bfae633cb1a962170fadf84377f025501c3d98366743dd9a430993ccf418`  
		Last Modified: Sat, 04 Sep 2021 06:17:04 GMT  
		Size: 2.7 MB (2749058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd796a832d5bb0c3758e5d068f8d3225552459787c09b32754eb6c19bcc7107`  
		Last Modified: Sat, 04 Sep 2021 06:17:12 GMT  
		Size: 48.6 MB (48613997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0a1857b6274ee53681f06612c1bee21f195193b1b0da94dab0e675da4a1d57`  
		Last Modified: Sat, 04 Sep 2021 06:17:02 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:1fb3f50d384f40401f119db274f0ad77036efe6b120a7f8db59ce93613f47a63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234101070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b153f0ce481b562a17a0a248a8901128512898a98543d06fd9e170f83ca815d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:32:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:32:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:19:08 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 10:19:16 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 10:19:22 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 10:27:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:27:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:27:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:27:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:28:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:28:05 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 07:08:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 07:13:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:13:48 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 07:13:53 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 07:13:56 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 07:14:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 07:14:09 GMT
ENV REDMINE_VERSION=4.1.4
# Wed, 18 Aug 2021 07:14:12 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Wed, 18 Aug 2021 07:14:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 07:20:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 07:20:21 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 07:20:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 07:20:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 07:20:28 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 07:20:31 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6540cca707f751654267130c5ff13338c730506cf900ab70cbba8eb8f0774f4`  
		Last Modified: Tue, 17 Aug 2021 10:35:53 GMT  
		Size: 12.7 MB (12704229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cb3d072ea667e9971932f23c9c5ddffe4a2d7c9a645aa1f53235dc8c2e2ae5`  
		Last Modified: Tue, 17 Aug 2021 10:35:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bbc8b7a7166a6ac7a00adc146da227c8d6dc674ba038b1bd1caaaa5584468f`  
		Last Modified: Tue, 17 Aug 2021 10:38:21 GMT  
		Size: 22.0 MB (21985135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72552c8f8b61b54c71444826adc1ca0cdb28ad48ec85cd5581b79cf258e4cd14`  
		Last Modified: Tue, 17 Aug 2021 10:38:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c23f2b8404f22ff77fdf90613e2d326a1ca11b09c1da15ff531aca2664efdc`  
		Last Modified: Wed, 18 Aug 2021 07:42:12 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ca5b7d6e0b60d89d19742009d27288dfc318679db7fc1cb7cc1344ae1e03c1`  
		Last Modified: Wed, 18 Aug 2021 07:42:32 GMT  
		Size: 101.3 MB (101328184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0c128368536cb3d8c984915e8d254fbbdf8a29031aef7b3404f7b03d353fdf`  
		Last Modified: Wed, 18 Aug 2021 07:42:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d059e0dee8988de5f102c551db08dd3e943e218ae6133e4a3305baab95120872`  
		Last Modified: Wed, 18 Aug 2021 07:42:09 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4a60c3ba0873df54906d49525bedad7791493c20a8f7fec0788834901533e7`  
		Last Modified: Wed, 18 Aug 2021 07:42:11 GMT  
		Size: 2.7 MB (2749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eba23e0d2f2018a281366f37a23f99bd4f9e78e583fb6df1c2d1f5863cff42`  
		Last Modified: Wed, 18 Aug 2021 07:42:19 GMT  
		Size: 64.8 MB (64776505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be28fce3dd14f86d47294d145f359079e1e42aba99d6854214bd6e7cc9d41483`  
		Last Modified: Wed, 18 Aug 2021 07:42:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; s390x

```console
$ docker pull redmine@sha256:3c150d2a41f279cb1db3539e31aed05f1351360ab9a23d54e8fc3f4cccf1d5b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216904370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:413d2927825c1f4c04d9fa2900f0d5140269f5a14ecc007a333f55162d69719f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 14:05:37 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 14:05:37 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 14:05:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 14:09:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 14:09:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 14:09:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 14:09:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 14:09:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 14:09:13 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 02:43:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 02:43:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:44:03 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 02:44:03 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 02:44:04 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 02:44:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 02:44:05 GMT
ENV REDMINE_VERSION=4.1.4
# Sat, 04 Sep 2021 02:44:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Sat, 04 Sep 2021 02:44:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 02:46:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 02:46:05 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 02:46:05 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 02:46:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:46:06 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 02:46:06 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386718fbf88b664e88cd07207db2c71a83df8cf7be0efff09692415187356879`  
		Last Modified: Fri, 03 Sep 2021 14:15:25 GMT  
		Size: 21.6 MB (21620271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5421f7853378d4bdf6f6a95b7d634de691057d827e751215fedb21fcb3a5a10`  
		Last Modified: Fri, 03 Sep 2021 14:15:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0767fa5a27a3127ff1c1fb788fd8d545b99e628373bf6e25aa7a0542f2ba120d`  
		Last Modified: Sat, 04 Sep 2021 02:50:46 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e76bd5cd10190ef4325aff3acee9066572a63fc6ea18aa12ef6cfa0de654b0`  
		Last Modified: Sat, 04 Sep 2021 02:50:58 GMT  
		Size: 91.8 MB (91789340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226814246b8e631091c35393417ead7ce6e345791bb18be0dd0f13b5f5e88d7e`  
		Last Modified: Sat, 04 Sep 2021 02:50:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ed19d9182def8b0c788d7d8e3c203f8612e58d42730ded3a336142bc694331`  
		Last Modified: Sat, 04 Sep 2021 02:50:44 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c6ee0291852fb5529665e47f28a96b8760f366d392fdcc6ede42fcb4436aa4`  
		Last Modified: Sat, 04 Sep 2021 02:50:44 GMT  
		Size: 2.7 MB (2749060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba0e5ab47b72de75862fda50b3d1acf8eecdf2abb77de328284258108f6763`  
		Last Modified: Sat, 04 Sep 2021 02:50:50 GMT  
		Size: 64.2 MB (64165419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f9028ff2c196df9625c1f135a722529a8de109219dec814802db0700b6e56c`  
		Last Modified: Sat, 04 Sep 2021 02:50:44 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-alpine`

```console
$ docker pull redmine@sha256:7e2b0e72f0fc9e06c3c126604523c6148838908a1db15bf6820b7dac12a18022
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:743c3f2cdeff8bd79cfa67a433d13c850572643100215b29c7927998725f0d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160689411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc29a022e94c365dece6c9a27112414f7fd626bbd741c8c5994b22bb7167bb4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:46:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Sep 2021 05:46:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Sep 2021 05:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_MAJOR=2.6
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 01 Sep 2021 05:56:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Sep 2021 05:56:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Sep 2021 05:56:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Sep 2021 05:56:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 05:56:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Sep 2021 05:56:40 GMT
CMD ["irb"]
# Wed, 01 Sep 2021 08:06:09 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 01 Sep 2021 08:06:17 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 01 Sep 2021 08:06:18 GMT
ENV RAILS_ENV=production
# Wed, 01 Sep 2021 08:06:18 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Sep 2021 08:06:18 GMT
ENV HOME=/home/redmine
# Wed, 01 Sep 2021 08:06:19 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 01 Sep 2021 08:06:19 GMT
ENV REDMINE_VERSION=4.1.4
# Wed, 01 Sep 2021 08:06:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Wed, 01 Sep 2021 08:09:10 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 01 Sep 2021 08:09:10 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 01 Sep 2021 08:11:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 01 Sep 2021 08:11:21 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 01 Sep 2021 08:11:21 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 01 Sep 2021 08:11:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 08:11:22 GMT
EXPOSE 3000
# Wed, 01 Sep 2021 08:11:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439708bfc17dd3e86c8b1415116fcd9de1d32330bdcc8b13fd009f7727844e9`  
		Last Modified: Wed, 01 Sep 2021 05:58:07 GMT  
		Size: 3.6 MB (3581641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260bc7d8cd8f26c27362c4ab1698f2a3e0b0a88516cdfd73a8884747ec12ee`  
		Last Modified: Wed, 01 Sep 2021 05:58:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c1b8b91f648ba1686d802a6e4dd386aa6f1fdc7064a254ffd6b2a9b5bded9c`  
		Last Modified: Wed, 01 Sep 2021 05:58:53 GMT  
		Size: 19.5 MB (19500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e38e14db89c6e839675f8981eeca140c2207e14190fcf5157f4041889857887`  
		Last Modified: Wed, 01 Sep 2021 05:58:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01010032e23eafcf759f8f1e41d523e70c6d201a3e1d8e6dc98f8d932b310429`  
		Last Modified: Wed, 01 Sep 2021 08:17:42 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ad2015e785efe3383671991b1d243af9742dae4b10370feacaf46811f9b3df`  
		Last Modified: Wed, 01 Sep 2021 08:17:53 GMT  
		Size: 69.5 MB (69527372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a096fdc361992f435e3d458db130407e167eb3872dedda83a6fc7a0425d8904a`  
		Last Modified: Wed, 01 Sep 2021 08:17:39 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7441b89101bb9a3b69f20854026e9918a89a2ae35eb9bd2c166a3355b69b7939`  
		Last Modified: Wed, 01 Sep 2021 08:17:39 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90aca8a6bdedfd865c370c8ee8c4857dbd1805aab2a5e0948fc3e5101fe003`  
		Last Modified: Wed, 01 Sep 2021 08:17:40 GMT  
		Size: 2.7 MB (2749743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff6318cf51dc1f1ff1b392c22ed4cdce52f2c3f3cd4009eed09291a383fe5b5`  
		Last Modified: Wed, 01 Sep 2021 08:17:46 GMT  
		Size: 62.5 MB (62512442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a3badf8631d16b9317d3eff2fe25663d469e559f07d341c25c50d94c6ca20`  
		Last Modified: Wed, 01 Sep 2021 08:17:39 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-passenger`

```console
$ docker pull redmine@sha256:53d814d2bf6b122c9edad0277d1a287fc0965f7724b0ccb077715b911c3cb532
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:ffc09235451c8ff1cd4eeba98c1c0ef69eb9a2f1e542b64606b5dfcdf5912231
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232893749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6ea8462fca3ce29d9d4bc160c25afe3caaf3d2d05c0da233ab632100be164f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:34:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:34:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:34:16 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:02:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:03:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:03:29 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:03:30 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:03:30 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:03:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:03:32 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 18:03:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 18:03:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:04:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:04:40 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:04:41 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:04:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:04:41 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:04:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 17 Aug 2021 18:04:50 GMT
ENV PASSENGER_VERSION=6.0.10
# Tue, 17 Aug 2021 18:05:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:05:18 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 17 Aug 2021 18:05:18 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 17 Aug 2021 18:05:19 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d07c054cf634a28fbb441bc93e20e2d4ae0dbaeb43e6aa17ab1c66f1c26b73`  
		Last Modified: Tue, 17 Aug 2021 04:43:06 GMT  
		Size: 21.5 MB (21468054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051a36df400859440c745a4abab787eac2d2318444dcd251750cf3a456ba21`  
		Last Modified: Tue, 17 Aug 2021 04:43:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85f465fea1749f74517e7a2b2c81d5ab6f19157bf460e5e7476d3aa04d2d7e`  
		Last Modified: Tue, 17 Aug 2021 18:10:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00de815fcdb1a6feb851a112e729207c26f6cbdd814903f8d7fb5d5b3618832`  
		Last Modified: Tue, 17 Aug 2021 18:11:13 GMT  
		Size: 94.1 MB (94088503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6dd4cade454377a496d734498902101532e5a3fc75e1d464b07f8e7d0b229e`  
		Last Modified: Tue, 17 Aug 2021 18:10:50 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb35b58efaa3018c9928e6ceaf42ba28c690355758565edd2ee14da281d74139`  
		Last Modified: Tue, 17 Aug 2021 18:10:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5ef1b243346c0a06cbf794b2195499317d58250e4485b7822abf270b4d229f`  
		Last Modified: Tue, 17 Aug 2021 18:10:52 GMT  
		Size: 2.7 MB (2749062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004c2031ebe227cb058ab066f0a87358cb28ebd69895c9a44ebfefbbc670845`  
		Last Modified: Tue, 17 Aug 2021 18:10:59 GMT  
		Size: 48.6 MB (48633124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b825d8abfc9574a6c4b650575e0ff513214b45b4f07756a300b46cb0f26ddeb`  
		Last Modified: Tue, 17 Aug 2021 18:10:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb75a811ee48f8e31dd520d86da998c98aad18d54f87df5756f5456559b963db`  
		Last Modified: Tue, 17 Aug 2021 18:11:29 GMT  
		Size: 21.3 MB (21322644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b01cf08dbfcaefccee6e6128408f7250dda5ead32d45599a318c57efe281f`  
		Last Modified: Tue, 17 Aug 2021 18:11:26 GMT  
		Size: 4.9 MB (4919288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.4`

```console
$ docker pull redmine@sha256:0c687f9fbe88a3381bd4a91a538f73df6890ea6c43f75c9fe40e859d08af63d7
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

### `redmine:4.1.4` - linux; amd64

```console
$ docker pull redmine@sha256:79620ad17c6061c101fe3a07a8fad3594fa291ff144352a9a8df130081839091
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.7 MB (206651817 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbf5593c96102abe227b98e4b51d5bbb46aff23a46b119a77903a081fc0a5ed2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:34:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:34:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:34:16 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:02:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:03:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:03:29 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:03:30 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:03:30 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:03:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:03:32 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 18:03:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 18:03:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:04:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:04:40 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:04:41 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:04:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:04:41 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:04:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d07c054cf634a28fbb441bc93e20e2d4ae0dbaeb43e6aa17ab1c66f1c26b73`  
		Last Modified: Tue, 17 Aug 2021 04:43:06 GMT  
		Size: 21.5 MB (21468054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051a36df400859440c745a4abab787eac2d2318444dcd251750cf3a456ba21`  
		Last Modified: Tue, 17 Aug 2021 04:43:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85f465fea1749f74517e7a2b2c81d5ab6f19157bf460e5e7476d3aa04d2d7e`  
		Last Modified: Tue, 17 Aug 2021 18:10:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00de815fcdb1a6feb851a112e729207c26f6cbdd814903f8d7fb5d5b3618832`  
		Last Modified: Tue, 17 Aug 2021 18:11:13 GMT  
		Size: 94.1 MB (94088503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6dd4cade454377a496d734498902101532e5a3fc75e1d464b07f8e7d0b229e`  
		Last Modified: Tue, 17 Aug 2021 18:10:50 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb35b58efaa3018c9928e6ceaf42ba28c690355758565edd2ee14da281d74139`  
		Last Modified: Tue, 17 Aug 2021 18:10:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5ef1b243346c0a06cbf794b2195499317d58250e4485b7822abf270b4d229f`  
		Last Modified: Tue, 17 Aug 2021 18:10:52 GMT  
		Size: 2.7 MB (2749062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004c2031ebe227cb058ab066f0a87358cb28ebd69895c9a44ebfefbbc670845`  
		Last Modified: Tue, 17 Aug 2021 18:10:59 GMT  
		Size: 48.6 MB (48633124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b825d8abfc9574a6c4b650575e0ff513214b45b4f07756a300b46cb0f26ddeb`  
		Last Modified: Tue, 17 Aug 2021 18:10:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; arm variant v5

```console
$ docker pull redmine@sha256:820710f4ac5c3e27c19513944d6efeb5cc8f227858222a3e2b6bfe5b5a9ea542
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210669898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:670ad4b2f9ed3a1d97388b2a0dd55a15f2c147c722ff61167b3c50813fa5a7c8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:49:01 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 17:49:01 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 17:49:02 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 17:53:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:53:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:53:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:53:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:53:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:53:37 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:06:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:06:13 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:06:13 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:06:14 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:06:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:06:16 GMT
ENV REDMINE_VERSION=4.1.4
# Sat, 04 Sep 2021 05:06:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Sat, 04 Sep 2021 05:06:22 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:11:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:11:59 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:12:00 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:12:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:12:01 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:12:01 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749f126c44247fab04b474652a00ee1a81c976173ad138c2813b3537ae229aa2`  
		Last Modified: Fri, 03 Sep 2021 18:03:49 GMT  
		Size: 20.7 MB (20733279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5467ac924fdbf4db3557de8b61cb7ff89beb1ec1777164bb78d7b65d64cacf8`  
		Last Modified: Fri, 03 Sep 2021 18:03:40 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393cf7309fe27f7f56257ac9ce482bb381c56ccb9c19f69d4d4997b57222c9ff`  
		Last Modified: Sat, 04 Sep 2021 05:21:45 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2d532998c02f6c9a866287ce631e361dcf9745dc03e5c9d074b7153f3b7c29`  
		Last Modified: Sat, 04 Sep 2021 05:22:43 GMT  
		Size: 89.6 MB (89576618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171faf2191b22aac8fd9f161aaa2b916ca52128abcf3e355f8aeeaaaa110ffa0`  
		Last Modified: Sat, 04 Sep 2021 05:21:43 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cc60bb6f99d05a9fade0765ecb9cebdb152ab117e2c87eb6940510af32e0dd`  
		Last Modified: Sat, 04 Sep 2021 05:21:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8178ad802a290b21fbb51dbc75475bd793fb3e655da90a110ce533bc2b33c3a`  
		Last Modified: Sat, 04 Sep 2021 05:21:47 GMT  
		Size: 2.7 MB (2749062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ebda4f1e758b5be42d3d195c12360777d7fe3dadacc09cc41e188c93162e2b5`  
		Last Modified: Sat, 04 Sep 2021 05:22:11 GMT  
		Size: 62.4 MB (62378756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11218622960555ad9afcc7d2960f59429b83ad60b704d5fa537823ee81ddd9`  
		Last Modified: Sat, 04 Sep 2021 05:21:43 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:99bf6eb7a4c90631440b9f5a1518978033c3d76c412f9ba72b4c1e9746ee78aa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203844212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:194ecb467b361afc105e966f3bfc18b722f741c1d231b551a82679b4f0d508b4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:30:30 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:09:51 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 10:09:52 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 10:09:52 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 10:13:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:13:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:13:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:13:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:13:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:13:56 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 08:39:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 08:40:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:40:54 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 08:40:55 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 08:40:55 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 08:40:57 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 08:40:57 GMT
ENV REDMINE_VERSION=4.1.4
# Wed, 18 Aug 2021 08:40:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Wed, 18 Aug 2021 08:41:04 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 08:46:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 08:46:20 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 08:46:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 08:46:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 08:46:21 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 08:46:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79875132dbc48a8386eb9079eb8b50d17399ed33c29a51ac8d7b2f943f3b1ac`  
		Last Modified: Tue, 17 Aug 2021 10:24:54 GMT  
		Size: 9.9 MB (9872248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ce2d51bf7561cb7c360e69499b42694c2e474b2f24d969e4250ac389dd4bec`  
		Last Modified: Tue, 17 Aug 2021 10:24:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fafe7065fd1b5df7801ad1787255f44a163e6d3c870f0a958a250125ce1dd08`  
		Last Modified: Tue, 17 Aug 2021 10:28:25 GMT  
		Size: 20.6 MB (20643690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981a320ed27e237a24cea403bd7a3a89e91b4c9d130c8d0265231346c903de9d`  
		Last Modified: Tue, 17 Aug 2021 10:28:16 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42323ca32828488d11f463f3a0603a3ed4a1fb7b8289b17c934621f31ee213c`  
		Last Modified: Wed, 18 Aug 2021 08:55:22 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc71522bb4b2c7a1ca1650d66db744b9b79c3abaf22c9796b25c400fe05e120f`  
		Last Modified: Wed, 18 Aug 2021 08:56:16 GMT  
		Size: 85.6 MB (85590409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8e1c03b25c8d1b7b70ae7adb351fa6fcbfeca38a7725de12115c5787b40951`  
		Last Modified: Wed, 18 Aug 2021 08:55:20 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579e678098ca93cf89148b75bdedc18658c8f6d76a5d3e962d2f6f1b5ed8d5e5`  
		Last Modified: Wed, 18 Aug 2021 08:55:20 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4bfd4a46d9c2e31abbe07d0c6c71cd11f25f72683fbc1a3b8e84e8f49045e90`  
		Last Modified: Wed, 18 Aug 2021 08:55:23 GMT  
		Size: 2.7 MB (2749056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a14f14c8dc1382cf377e8aa751c5e3d71ed0a79f11c866eb1fb8c9d305151b9`  
		Last Modified: Wed, 18 Aug 2021 08:55:49 GMT  
		Size: 62.2 MB (62238320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92a4cdd95e2f9e715a4ad8a056c9b2d67ed5798007b5125dcbfedea161398e3`  
		Last Modified: Wed, 18 Aug 2021 08:55:20 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:03050db75dcf9c5f92a42065092427328e1ff95b14cfe4eb0145b34b1772ec3c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217545418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5832c6b908dc3582d811982b31cb0736beaf8b988b4d1e3d40b27a7ea6171743`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 12:19:58 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 12:22:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:22:07 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:22:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:22:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:22:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:22:08 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:07:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:07:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:07:50 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:07:50 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:07:50 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:07:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:07:51 GMT
ENV REDMINE_VERSION=4.1.4
# Sat, 04 Sep 2021 05:07:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Sat, 04 Sep 2021 05:07:55 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:09:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:10:00 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:10:00 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:10:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:10:00 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:10:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64effe010a8ea4895a32764391d02522a7b931f55473493124a03c221c67e1a2`  
		Last Modified: Fri, 03 Sep 2021 12:29:53 GMT  
		Size: 21.3 MB (21308991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9836139b64d4bdf3ba22538bc724ccc0cac2d0eecbca7a1a2ef12c486f39e4a`  
		Last Modified: Fri, 03 Sep 2021 12:29:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30882468c09d5aac3b9b1c5509386ed9719998eb95284bbc3d82c789aa254f31`  
		Last Modified: Sat, 04 Sep 2021 05:14:11 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82fbd53cdf3d8fd12dd9858d43a5f75ff6934ea03373505bcdf9f61fbe3b4385`  
		Last Modified: Sat, 04 Sep 2021 05:14:26 GMT  
		Size: 92.6 MB (92610545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1064cbb77106f38550f68ad21538df88b0d2e80c74c5a33cc6d599dade25a2`  
		Last Modified: Sat, 04 Sep 2021 05:14:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd94a5f71d8c4419f9e66c36c86d1835b66aef7dcd9ae2d4cbec8f16e207ceb`  
		Last Modified: Sat, 04 Sep 2021 05:14:08 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7f8eb2d3ae7a8b942835c3976c1e611f9bfef9f55cd17d83e074b8dec393df`  
		Last Modified: Sat, 04 Sep 2021 05:14:09 GMT  
		Size: 2.7 MB (2749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbfe9573c141edbf4f99af468d979c15bcf21f10e415885cc18d04c8fd2aac5`  
		Last Modified: Sat, 04 Sep 2021 05:14:16 GMT  
		Size: 63.7 MB (63693325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc8b6de7c6d30b4b38ba818b339df7b8e1c624c9ec8cf341492badeb539cc43`  
		Last Modified: Sat, 04 Sep 2021 05:14:08 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; 386

```console
$ docker pull redmine@sha256:b19011e8b39cc7ec6a822049f9e031cb344fb4ac238b0b54cf46fad11699d06d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213004456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8865b21d35b0e141a83ad423da3570e6f614d64a4abde308461caafeb197b61c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:58:09 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 11:58:10 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 11:58:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 12:02:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:02:05 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:02:05 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:02:06 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:02:08 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:02:08 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 06:08:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 06:08:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 06:08:53 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 06:08:53 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 06:08:53 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 06:08:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 06:08:56 GMT
ENV REDMINE_VERSION=4.1.4
# Sat, 04 Sep 2021 06:08:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Sat, 04 Sep 2021 06:09:02 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 06:10:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 06:10:29 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 06:10:30 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 06:10:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 06:10:30 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 06:10:31 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd42d7474f924c3c64bdd4e3ae8097209463c898897a6fc3d869bfad5458a76a`  
		Last Modified: Fri, 03 Sep 2021 12:12:12 GMT  
		Size: 20.9 MB (20910072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6527ea22b515317b992c2ad83317df356fb9c331a328a6ce09dfc29199063b`  
		Last Modified: Fri, 03 Sep 2021 12:12:08 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf069e6a84c6a25e1afb5b9e31dfc64d2ad9b8b55ba2a7520e4f7279927520c2`  
		Last Modified: Sat, 04 Sep 2021 06:17:05 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3471af7fd62676cb8bebe5257d6f29e9936bc1b6ec48ff1730a6c82b676dd1`  
		Last Modified: Sat, 04 Sep 2021 06:17:32 GMT  
		Size: 95.7 MB (95702608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f5db09056e5bb6fce4854295752a64f439c54c2acb62bdbf0b180de138488b`  
		Last Modified: Sat, 04 Sep 2021 06:17:02 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0183266bad02bc74edb95f172168ca409f6296887c8bec3dc867794923cf4c`  
		Last Modified: Sat, 04 Sep 2021 06:17:02 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d104bfae633cb1a962170fadf84377f025501c3d98366743dd9a430993ccf418`  
		Last Modified: Sat, 04 Sep 2021 06:17:04 GMT  
		Size: 2.7 MB (2749058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd796a832d5bb0c3758e5d068f8d3225552459787c09b32754eb6c19bcc7107`  
		Last Modified: Sat, 04 Sep 2021 06:17:12 GMT  
		Size: 48.6 MB (48613997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0a1857b6274ee53681f06612c1bee21f195193b1b0da94dab0e675da4a1d57`  
		Last Modified: Sat, 04 Sep 2021 06:17:02 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; ppc64le

```console
$ docker pull redmine@sha256:1fb3f50d384f40401f119db274f0ad77036efe6b120a7f8db59ce93613f47a63
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234101070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b153f0ce481b562a17a0a248a8901128512898a98543d06fd9e170f83ca815d`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:32:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:32:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 10:19:08 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 10:19:16 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 10:19:22 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 10:27:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:27:36 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:27:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:27:47 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:28:02 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:28:05 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 07:08:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 07:13:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:13:48 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 07:13:53 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 07:13:56 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 07:14:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 07:14:09 GMT
ENV REDMINE_VERSION=4.1.4
# Wed, 18 Aug 2021 07:14:12 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Wed, 18 Aug 2021 07:14:31 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 07:20:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 07:20:21 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 07:20:22 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 07:20:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 07:20:28 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 07:20:31 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6540cca707f751654267130c5ff13338c730506cf900ab70cbba8eb8f0774f4`  
		Last Modified: Tue, 17 Aug 2021 10:35:53 GMT  
		Size: 12.7 MB (12704229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cb3d072ea667e9971932f23c9c5ddffe4a2d7c9a645aa1f53235dc8c2e2ae5`  
		Last Modified: Tue, 17 Aug 2021 10:35:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7bbc8b7a7166a6ac7a00adc146da227c8d6dc674ba038b1bd1caaaa5584468f`  
		Last Modified: Tue, 17 Aug 2021 10:38:21 GMT  
		Size: 22.0 MB (21985135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72552c8f8b61b54c71444826adc1ca0cdb28ad48ec85cd5581b79cf258e4cd14`  
		Last Modified: Tue, 17 Aug 2021 10:38:17 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8c23f2b8404f22ff77fdf90613e2d326a1ca11b09c1da15ff531aca2664efdc`  
		Last Modified: Wed, 18 Aug 2021 07:42:12 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0ca5b7d6e0b60d89d19742009d27288dfc318679db7fc1cb7cc1344ae1e03c1`  
		Last Modified: Wed, 18 Aug 2021 07:42:32 GMT  
		Size: 101.3 MB (101328184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0c128368536cb3d8c984915e8d254fbbdf8a29031aef7b3404f7b03d353fdf`  
		Last Modified: Wed, 18 Aug 2021 07:42:10 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d059e0dee8988de5f102c551db08dd3e943e218ae6133e4a3305baab95120872`  
		Last Modified: Wed, 18 Aug 2021 07:42:09 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4a60c3ba0873df54906d49525bedad7791493c20a8f7fec0788834901533e7`  
		Last Modified: Wed, 18 Aug 2021 07:42:11 GMT  
		Size: 2.7 MB (2749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eba23e0d2f2018a281366f37a23f99bd4f9e78e583fb6df1c2d1f5863cff42`  
		Last Modified: Wed, 18 Aug 2021 07:42:19 GMT  
		Size: 64.8 MB (64776505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be28fce3dd14f86d47294d145f359079e1e42aba99d6854214bd6e7cc9d41483`  
		Last Modified: Wed, 18 Aug 2021 07:42:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; s390x

```console
$ docker pull redmine@sha256:3c150d2a41f279cb1db3539e31aed05f1351360ab9a23d54e8fc3f4cccf1d5b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216904370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:413d2927825c1f4c04d9fa2900f0d5140269f5a14ecc007a333f55162d69719f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 14:05:37 GMT
ENV RUBY_MAJOR=2.6
# Fri, 03 Sep 2021 14:05:37 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 03 Sep 2021 14:05:38 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 03 Sep 2021 14:09:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 14:09:11 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 14:09:11 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 14:09:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 14:09:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 14:09:13 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 02:43:12 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 02:43:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:44:03 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 02:44:03 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 02:44:04 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 02:44:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 02:44:05 GMT
ENV REDMINE_VERSION=4.1.4
# Sat, 04 Sep 2021 02:44:05 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Sat, 04 Sep 2021 02:44:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 02:46:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 02:46:05 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 02:46:05 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 02:46:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:46:06 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 02:46:06 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:386718fbf88b664e88cd07207db2c71a83df8cf7be0efff09692415187356879`  
		Last Modified: Fri, 03 Sep 2021 14:15:25 GMT  
		Size: 21.6 MB (21620271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5421f7853378d4bdf6f6a95b7d634de691057d827e751215fedb21fcb3a5a10`  
		Last Modified: Fri, 03 Sep 2021 14:15:24 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0767fa5a27a3127ff1c1fb788fd8d545b99e628373bf6e25aa7a0542f2ba120d`  
		Last Modified: Sat, 04 Sep 2021 02:50:46 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e76bd5cd10190ef4325aff3acee9066572a63fc6ea18aa12ef6cfa0de654b0`  
		Last Modified: Sat, 04 Sep 2021 02:50:58 GMT  
		Size: 91.8 MB (91789340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226814246b8e631091c35393417ead7ce6e345791bb18be0dd0f13b5f5e88d7e`  
		Last Modified: Sat, 04 Sep 2021 02:50:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92ed19d9182def8b0c788d7d8e3c203f8612e58d42730ded3a336142bc694331`  
		Last Modified: Sat, 04 Sep 2021 02:50:44 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c6ee0291852fb5529665e47f28a96b8760f366d392fdcc6ede42fcb4436aa4`  
		Last Modified: Sat, 04 Sep 2021 02:50:44 GMT  
		Size: 2.7 MB (2749060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eba0e5ab47b72de75862fda50b3d1acf8eecdf2abb77de328284258108f6763`  
		Last Modified: Sat, 04 Sep 2021 02:50:50 GMT  
		Size: 64.2 MB (64165419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f9028ff2c196df9625c1f135a722529a8de109219dec814802db0700b6e56c`  
		Last Modified: Sat, 04 Sep 2021 02:50:44 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.4-alpine`

```console
$ docker pull redmine@sha256:7e2b0e72f0fc9e06c3c126604523c6148838908a1db15bf6820b7dac12a18022
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1.4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:743c3f2cdeff8bd79cfa67a433d13c850572643100215b29c7927998725f0d5c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.7 MB (160689411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffc29a022e94c365dece6c9a27112414f7fd626bbd741c8c5994b22bb7167bb4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:46:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Sep 2021 05:46:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Sep 2021 05:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_MAJOR=2.6
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_VERSION=2.6.8
# Wed, 01 Sep 2021 05:53:48 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Wed, 01 Sep 2021 05:56:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Sep 2021 05:56:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Sep 2021 05:56:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Sep 2021 05:56:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 05:56:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Sep 2021 05:56:40 GMT
CMD ["irb"]
# Wed, 01 Sep 2021 08:06:09 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 01 Sep 2021 08:06:17 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 01 Sep 2021 08:06:18 GMT
ENV RAILS_ENV=production
# Wed, 01 Sep 2021 08:06:18 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Sep 2021 08:06:18 GMT
ENV HOME=/home/redmine
# Wed, 01 Sep 2021 08:06:19 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 01 Sep 2021 08:06:19 GMT
ENV REDMINE_VERSION=4.1.4
# Wed, 01 Sep 2021 08:06:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Wed, 01 Sep 2021 08:09:10 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 01 Sep 2021 08:09:10 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 01 Sep 2021 08:11:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 01 Sep 2021 08:11:21 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 01 Sep 2021 08:11:21 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 01 Sep 2021 08:11:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 08:11:22 GMT
EXPOSE 3000
# Wed, 01 Sep 2021 08:11:22 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439708bfc17dd3e86c8b1415116fcd9de1d32330bdcc8b13fd009f7727844e9`  
		Last Modified: Wed, 01 Sep 2021 05:58:07 GMT  
		Size: 3.6 MB (3581641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260bc7d8cd8f26c27362c4ab1698f2a3e0b0a88516cdfd73a8884747ec12ee`  
		Last Modified: Wed, 01 Sep 2021 05:58:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c1b8b91f648ba1686d802a6e4dd386aa6f1fdc7064a254ffd6b2a9b5bded9c`  
		Last Modified: Wed, 01 Sep 2021 05:58:53 GMT  
		Size: 19.5 MB (19500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e38e14db89c6e839675f8981eeca140c2207e14190fcf5157f4041889857887`  
		Last Modified: Wed, 01 Sep 2021 05:58:51 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01010032e23eafcf759f8f1e41d523e70c6d201a3e1d8e6dc98f8d932b310429`  
		Last Modified: Wed, 01 Sep 2021 08:17:42 GMT  
		Size: 1.2 KB (1207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ad2015e785efe3383671991b1d243af9742dae4b10370feacaf46811f9b3df`  
		Last Modified: Wed, 01 Sep 2021 08:17:53 GMT  
		Size: 69.5 MB (69527372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a096fdc361992f435e3d458db130407e167eb3872dedda83a6fc7a0425d8904a`  
		Last Modified: Wed, 01 Sep 2021 08:17:39 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7441b89101bb9a3b69f20854026e9918a89a2ae35eb9bd2c166a3355b69b7939`  
		Last Modified: Wed, 01 Sep 2021 08:17:39 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd90aca8a6bdedfd865c370c8ee8c4857dbd1805aab2a5e0948fc3e5101fe003`  
		Last Modified: Wed, 01 Sep 2021 08:17:40 GMT  
		Size: 2.7 MB (2749743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff6318cf51dc1f1ff1b392c22ed4cdce52f2c3f3cd4009eed09291a383fe5b5`  
		Last Modified: Wed, 01 Sep 2021 08:17:46 GMT  
		Size: 62.5 MB (62512442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4a3badf8631d16b9317d3eff2fe25663d469e559f07d341c25c50d94c6ca20`  
		Last Modified: Wed, 01 Sep 2021 08:17:39 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.4-passenger`

```console
$ docker pull redmine@sha256:53d814d2bf6b122c9edad0277d1a287fc0965f7724b0ccb077715b911c3cb532
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1.4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:ffc09235451c8ff1cd4eeba98c1c0ef69eb9a2f1e542b64606b5dfcdf5912231
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.9 MB (232893749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6ea8462fca3ce29d9d4bc160c25afe3caaf3d2d05c0da233ab632100be164f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:30:49 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:34:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:34:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:34:15 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:34:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:34:16 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:02:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:03:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:03:29 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:03:30 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:03:30 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:03:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:03:32 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 18:03:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 18:03:37 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:04:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:04:40 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:04:41 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:04:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:04:41 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:04:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 17 Aug 2021 18:04:50 GMT
ENV PASSENGER_VERSION=6.0.10
# Tue, 17 Aug 2021 18:05:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:05:18 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 17 Aug 2021 18:05:18 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 17 Aug 2021 18:05:19 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41d07c054cf634a28fbb441bc93e20e2d4ae0dbaeb43e6aa17ab1c66f1c26b73`  
		Last Modified: Tue, 17 Aug 2021 04:43:06 GMT  
		Size: 21.5 MB (21468054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051a36df400859440c745a4abab787eac2d2318444dcd251750cf3a456ba21`  
		Last Modified: Tue, 17 Aug 2021 04:43:03 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85f465fea1749f74517e7a2b2c81d5ab6f19157bf460e5e7476d3aa04d2d7e`  
		Last Modified: Tue, 17 Aug 2021 18:10:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00de815fcdb1a6feb851a112e729207c26f6cbdd814903f8d7fb5d5b3618832`  
		Last Modified: Tue, 17 Aug 2021 18:11:13 GMT  
		Size: 94.1 MB (94088503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6dd4cade454377a496d734498902101532e5a3fc75e1d464b07f8e7d0b229e`  
		Last Modified: Tue, 17 Aug 2021 18:10:50 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb35b58efaa3018c9928e6ceaf42ba28c690355758565edd2ee14da281d74139`  
		Last Modified: Tue, 17 Aug 2021 18:10:51 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5ef1b243346c0a06cbf794b2195499317d58250e4485b7822abf270b4d229f`  
		Last Modified: Tue, 17 Aug 2021 18:10:52 GMT  
		Size: 2.7 MB (2749062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c004c2031ebe227cb058ab066f0a87358cb28ebd69895c9a44ebfefbbc670845`  
		Last Modified: Tue, 17 Aug 2021 18:10:59 GMT  
		Size: 48.6 MB (48633124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b825d8abfc9574a6c4b650575e0ff513214b45b4f07756a300b46cb0f26ddeb`  
		Last Modified: Tue, 17 Aug 2021 18:10:51 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb75a811ee48f8e31dd520d86da998c98aad18d54f87df5756f5456559b963db`  
		Last Modified: Tue, 17 Aug 2021 18:11:29 GMT  
		Size: 21.3 MB (21322644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b01cf08dbfcaefccee6e6128408f7250dda5ead32d45599a318c57efe281f`  
		Last Modified: Tue, 17 Aug 2021 18:11:26 GMT  
		Size: 4.9 MB (4919288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2`

```console
$ docker pull redmine@sha256:946ffb0d6839fa3d89d077b47d3024b103b42f905463932ea6950703489217a7
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
$ docker pull redmine@sha256:184738eb8da314459e8b41f33ffdfad41e82d466ec96843bf49cd46d1bc5109a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195495858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab3b16cafa89a7d46015d66e213c5ddc798b96e35c33ae8100fc09ba1d9525e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:21:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:23:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:23:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:23:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:23:47 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:01:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:01:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:01:29 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:01:29 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:01:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 18:01:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:02:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:02:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:02:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:02:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:02:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119720cd004c3495b5cd6b8883e01df56a3438046b3ecc3198ffb3849f6f25df`  
		Last Modified: Tue, 17 Aug 2021 04:42:13 GMT  
		Size: 14.5 MB (14510198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b764bf01e480a9fff1b3e5a263f7f9f9b4fa77325f616c37cb8e2c81d51e3dd9`  
		Last Modified: Tue, 17 Aug 2021 04:42:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84946f74729ab44aaa49a9af6012e6293fb02521ca05cffaccf128e7b157cec`  
		Last Modified: Tue, 17 Aug 2021 18:09:47 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcde4d7d6d22355ecf23701bfa1a2abba49bcabfc5f4dd90c746e0143569ba`  
		Last Modified: Tue, 17 Aug 2021 18:10:07 GMT  
		Size: 94.1 MB (94087892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5742225b6ad582633258fcf1e969851dbdd33be3d03cb05cf61b1ea900d8cc`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81933ac92f0a4be0c34689c7c3035c0aa0e4d7e89153bb41cbe0821a1c2a89f7`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb927d9d1176a8bbb1d88d687d964fae4ee7e61ebd08be4d8648f21caa9299e`  
		Last Modified: Tue, 17 Aug 2021 18:09:46 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d25f4984fe7a6089fe506ca06732024aafbfe47de090d95c448ac84b589e573`  
		Last Modified: Tue, 17 Aug 2021 18:09:53 GMT  
		Size: 44.1 MB (44122772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f790489c8bf8667ba0727c9aa46fb6e9d9128bf89a9c1330b90689f04155bf`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v5

```console
$ docker pull redmine@sha256:2e7f776816b5769bfdaa730b3d5c3d64b1025e071ad1c79a6716eff4c1041de1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed286853331cdd20528ca2dacc87e979025cee325cdd5528cc16dd1b6558987f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:31:22 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 17:31:23 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 17:31:23 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 17:35:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:35:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:35:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:35:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:35:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:35:44 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 04:57:25 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 04:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 04:58:43 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 04:58:43 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 04:58:44 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 04:58:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 04:58:46 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 04:58:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 04:58:52 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:04:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:04:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:04:38 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:04:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:04:39 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:04:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add78f82744b7f4c8c7522adfae87214be4104b79f343add868890b00ec859d2`  
		Last Modified: Fri, 03 Sep 2021 18:01:59 GMT  
		Size: 13.9 MB (13871472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea079592f786a6bd50d8249c1ceedc638402805fe700febed7e646dd69ee642`  
		Last Modified: Fri, 03 Sep 2021 18:01:51 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217f2b4088020d7dcc1aed89a3d8db9a8756c8bee078541881250a9dbbad1e6`  
		Last Modified: Sat, 04 Sep 2021 05:20:20 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5101e0f6c49b2df1f4b08067b3c1b135fe25243c4054b5868f953bc3f37490bf`  
		Last Modified: Sat, 04 Sep 2021 05:21:21 GMT  
		Size: 89.6 MB (89576088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ae1568de59acec6c4cb2932be2397e122fea3950b3104ce626623970d75f5`  
		Last Modified: Sat, 04 Sep 2021 05:20:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e297238097a4d3b15fbadef5aa4d865ab9cef981d1cae1bb633f216dd4c9dad`  
		Last Modified: Sat, 04 Sep 2021 05:20:18 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6628563efc672886d9ef6550835ad5efa230a1e39f41e8e612ad2af2c4e7ba99`  
		Last Modified: Sat, 04 Sep 2021 05:20:21 GMT  
		Size: 3.1 MB (3061924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0be986223cb5256d684c7602b705f39bd686a8ffb95e92c116f1db188b1da6`  
		Last Modified: Sat, 04 Sep 2021 05:20:43 GMT  
		Size: 55.2 MB (55234623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcee35bd3d5db50a493ba5105b6272ef59dc2eb800bb91c4eef2c100309638c`  
		Last Modified: Sat, 04 Sep 2021 05:20:18 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cd7275a7d34b3290a919f94e8e29ca61a913d0427cd2718ed49e354450b9eb2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0f96d1f050b7bd3415163fa63302bbaf4443e8741688fdcbbe19819f034e55`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:30:30 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 09:44:16 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 09:44:17 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 09:44:17 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 09:48:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 09:48:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 09:48:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 09:48:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:48:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 09:48:25 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 08:32:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 08:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:33:59 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 08:33:59 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 08:34:00 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 08:34:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 08:34:02 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 18 Aug 2021 08:34:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 18 Aug 2021 08:34:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 08:39:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 08:39:27 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 08:39:27 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 08:39:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 08:39:28 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 08:39:29 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79875132dbc48a8386eb9079eb8b50d17399ed33c29a51ac8d7b2f943f3b1ac`  
		Last Modified: Tue, 17 Aug 2021 10:24:54 GMT  
		Size: 9.9 MB (9872248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ce2d51bf7561cb7c360e69499b42694c2e474b2f24d969e4250ac389dd4bec`  
		Last Modified: Tue, 17 Aug 2021 10:24:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6910fec61b3de474c201c0eaae12d42336d748c8d6c55e7b06571adfef449ac`  
		Last Modified: Tue, 17 Aug 2021 10:26:58 GMT  
		Size: 13.8 MB (13767304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376804c80b6dffd48a9a1ce10f9ae6e593d25030de692dfc17341be078eaad9f`  
		Last Modified: Tue, 17 Aug 2021 10:26:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d2abf0978eca4cf58f5136adb1c1db17ff192b414feb932d7a524feb862a06`  
		Last Modified: Wed, 18 Aug 2021 08:54:19 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25cf090ed21d7e7a084b69c43bc419fc12838e33b344eba331171fc2868d53d`  
		Last Modified: Wed, 18 Aug 2021 08:54:58 GMT  
		Size: 85.6 MB (85590672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782c9d20468a0cc0f8d38101ddc7ef218d18c48ecbeda7932121ed297886d697`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eab3d69b805b2536e4dd6b587ff8eb27d96f2df1057e5e31d91410e872d74f`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b22a54dbdc1d4adfc0f8ae626f1aed9ec9010d827a989cf4af007f1126801d`  
		Last Modified: Wed, 18 Aug 2021 08:54:20 GMT  
		Size: 3.1 MB (3061921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2005224b6c07acc4bbabc1a0bb15ec249509c15fcfd8d777031ad7050b6ce1ac`  
		Last Modified: Wed, 18 Aug 2021 08:54:34 GMT  
		Size: 55.1 MB (55073085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1537e502cf0def19348a8406f66144d8986698047998e80c0a8ce7c1759735`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:54281b02713340086f8270560a0a6f34bd50ef111b8136870436e66a36c494b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203249301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c7d37a5bf5a362ddcdb750e1beba28d0362bd1632eaf9ed4bea0913ac529f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 12:12:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:12:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:12:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:12:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:12:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:12:43 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:04:14 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:04:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:04:38 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:04:38 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:04:39 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:04:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:04:39 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 05:04:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 05:04:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:07:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:07:20 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:07:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:07:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:07:21 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:07:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee312ced32893df36a25a76149db554574daaeb35128bcfb8c1d9d5bbc1fe73d`  
		Last Modified: Fri, 03 Sep 2021 12:28:34 GMT  
		Size: 14.4 MB (14356717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719ff35ff5b1cf24bc8a71ce6e567a505fbb6fcf0e9c141d8bdc230f164a57a0`  
		Last Modified: Fri, 03 Sep 2021 12:28:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd82b0673245cfbd7fe883e89fb55be7bd3e805e26de6ef17064f507f3df13c`  
		Last Modified: Sat, 04 Sep 2021 05:13:30 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d090f849a4da11b63677dfaff64f9709e15e9a24e740bcfbbca2545dc3f6395`  
		Last Modified: Sat, 04 Sep 2021 05:13:46 GMT  
		Size: 92.6 MB (92609378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9748bdee2b0b6d123ea99593dc5ff47d2b23dc011f52aef631f6eff5be900547`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454a0d8da53bfccd39f515fb93989777b3b6ebfc7c78bcb00be2b2e831683de`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323cf17e748812ba32fb6ed26e50ba83a1ddc4ec3eb22dc3674a4ddfc7ab2674`  
		Last Modified: Sat, 04 Sep 2021 05:13:29 GMT  
		Size: 3.1 MB (3061917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f679bdbfd5dafda429d92ba97d958576ee482d6c7e7ef09611df897a8af86ee7`  
		Last Modified: Sat, 04 Sep 2021 05:13:34 GMT  
		Size: 56.0 MB (56037790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080fea9fe34c2c40a03359a1c3402d684badf754bb190a6f22679e53c3d25c08`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; 386

```console
$ docker pull redmine@sha256:ebc552d443096692ec50b0c4279d2cfef5098651e51fab433fa57a8859e864c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202126624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c6ceb9f5cc0c343839ed2f1ed0ac64ccf12847ac4939e863d82309c42e9ec3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:39:26 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 11:39:27 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 11:39:27 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 11:43:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 11:43:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 11:43:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 11:43:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 11:43:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 11:43:41 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 06:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 06:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 06:05:58 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 06:05:59 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 06:05:59 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 06:06:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 06:06:01 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 06:06:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 06:06:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 06:07:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 06:07:41 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 06:07:42 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 06:07:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 06:07:42 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 06:07:43 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ab3f959a8410b96952c0ab29ff5376ff960f0c46619b9da4de191c3e631a2e`  
		Last Modified: Fri, 03 Sep 2021 12:10:29 GMT  
		Size: 14.0 MB (13992725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b213d5105e1a800ff597002681646442fd6df3b46274ee545c1825df025af800`  
		Last Modified: Fri, 03 Sep 2021 12:10:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fa640c55779f987dc35c6cc6766cb5f2fa277c85a28f8b096f1276dedc45ba`  
		Last Modified: Sat, 04 Sep 2021 06:16:20 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae199078f5eaaf3ea967d1448f821631d10ea7afd47dcb79a7701e0fe24ed70`  
		Last Modified: Sat, 04 Sep 2021 06:16:43 GMT  
		Size: 95.7 MB (95703257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61de99b7f1e5da0063d2955ec7a01f01d7ed345b8b6dd804aada111402bf9f`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ba76c31dcad016bf941f0e0be2694f0fa339e5c24d7ef5ee4916be74697f0a`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70e46e86bb38bc42f7060c39fbbc233ea20e6f7089b73e2335d3440c1c33d1`  
		Last Modified: Sat, 04 Sep 2021 06:16:18 GMT  
		Size: 3.1 MB (3061914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb99b00b084c4a0e83a272f225159c4cbf6214c81fe2f8571dfaf4276978ce97`  
		Last Modified: Sat, 04 Sep 2021 06:16:25 GMT  
		Size: 44.3 MB (44340016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cbcc1c6467ba9477359f3f850d4c4535ba281eea1e75124bb96d94ba91c2fa`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; ppc64le

```console
$ docker pull redmine@sha256:750c649c6ed54a1bc79c41c44b1bfb009a38e130ca51356a0a5637a77b452f5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219650978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3733a5127a682e88605681a10a6637a271090e9dddd1ecb6d71d7b4e0b6d2c82`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:32:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:32:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 09:53:38 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 09:53:41 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 09:53:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 10:00:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:00:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:00:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:01:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:01:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:01:28 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 06:54:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 06:59:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:00:07 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 07:00:21 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 07:00:26 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 07:00:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 07:00:43 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 18 Aug 2021 07:00:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 18 Aug 2021 07:01:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 07:07:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 07:07:18 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 07:07:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 07:07:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 07:07:39 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 07:07:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6540cca707f751654267130c5ff13338c730506cf900ab70cbba8eb8f0774f4`  
		Last Modified: Tue, 17 Aug 2021 10:35:53 GMT  
		Size: 12.7 MB (12704229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cb3d072ea667e9971932f23c9c5ddffe4a2d7c9a645aa1f53235dc8c2e2ae5`  
		Last Modified: Tue, 17 Aug 2021 10:35:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29445a92f99df6ece2c68fdd21d13b23e28c76507ae5fc4497cbf9272cd41e91`  
		Last Modified: Tue, 17 Aug 2021 10:37:15 GMT  
		Size: 15.0 MB (14997282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee87ac0f307c59470977ad0b974013269088413f9061698138c7f01175ec9982`  
		Last Modified: Tue, 17 Aug 2021 10:37:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfb261039caaf3d27ac4757a6a0ca770e695ac15e72cce135badcdf8d17b060`  
		Last Modified: Wed, 18 Aug 2021 07:40:45 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa4557b0838e19c4cd9f385a4b5ea0972af6fba31e8bcc39e77336887cd48ee`  
		Last Modified: Wed, 18 Aug 2021 07:41:48 GMT  
		Size: 101.3 MB (101328471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5cb4e6a472bc1f6140175c495cf2115da58206520a01bca00638227f2370ea`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4789be342e86d5f2793092f064c41fde923d87fb85f130d8100b4c88af3474`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2190284052685dcbf10a7e8e39410965a72be33c4c924cedc97130de22e6c8f4`  
		Last Modified: Wed, 18 Aug 2021 07:40:52 GMT  
		Size: 3.1 MB (3061910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b6fa0cc2de623e70d74216ebe78d7dfccc76bda34aae287ec61259ff3f54ce`  
		Last Modified: Wed, 18 Aug 2021 07:41:17 GMT  
		Size: 57.0 MB (57001117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164f878c998618c80d1e4d55973b954723ba05120f5a4984c112bc210edd8c6`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; s390x

```console
$ docker pull redmine@sha256:f764e6f237dd0b4ccc459c4a58872d66f5d9015fa61828ef337cc1aba2dde405
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202557142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:182cde8e814a22a30968ac8996e2499e862f311f0c6cd3a5d1db75334c1b9dce`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 13:38:11 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 13:38:11 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 13:38:12 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 13:41:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 13:41:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 13:41:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 13:41:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 13:41:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 13:41:45 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 02:39:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 02:40:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:40:18 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 02:40:18 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 02:40:19 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 02:40:19 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 02:40:19 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 02:40:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 02:40:23 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 02:42:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 02:42:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 02:42:50 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 02:42:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:42:51 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 02:42:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ea6888b61e31cb5b4a8f014006c7cb8fa8a3b7224b7ad3f0b4af257229c789`  
		Last Modified: Fri, 03 Sep 2021 14:14:23 GMT  
		Size: 14.7 MB (14697502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ef0cfb1210ec8b5dff947c27988590a3931cf76a1437a6fe10f30aae9f813`  
		Last Modified: Fri, 03 Sep 2021 14:14:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a04f5ff5ec2ee8dd1b21974adff7bf0e6fdb70338e190c6094eed2747ceb117`  
		Last Modified: Sat, 04 Sep 2021 02:50:16 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf9140fc0de2f47daa7719c6c1cbbf193066ad2a67f60c95d78b7baf3626508`  
		Last Modified: Sat, 04 Sep 2021 02:50:29 GMT  
		Size: 91.8 MB (91790843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d640980eb96fb9f7eef22043b3c502898b8cc3f7b1447f1f19055222d3a3bf`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80df1a5482c5309af87986c42c45a6cd4c0cfbce1535792b2c1ba652e2c2a304`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9bc3013aec1061db002a07fa5ae39181287f086837e8c8c53c5814049c837d`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 3.1 MB (3061916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9caa222bcb2e88202afcfdf166e5a0613fe99bc55cc9b416dda1e1e2484c4`  
		Last Modified: Sat, 04 Sep 2021 02:50:19 GMT  
		Size: 56.4 MB (56426601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff0983c6ea2bc0e811104db8303487a7286daf0ee17c051de72eb5e75dbbc32`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-alpine`

```console
$ docker pull redmine@sha256:b3f4c38a52e764136b2d930a044a60e362120dd0c8900217a3e90e852421ab31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:c5db53d0c811b57d386d30b72d9050a7aa2fe1cf1b73fd86e20caaf5794597b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.7 MB (149701448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e405182f204a9a00f59a9abe4dd5e343cc108150ea4d66c36d925aed95a284`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:46:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Sep 2021 05:46:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Sep 2021 05:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_MAJOR=2.7
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Wed, 01 Sep 2021 05:53:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Sep 2021 05:53:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Sep 2021 05:53:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Sep 2021 05:53:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 05:53:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Sep 2021 05:53:30 GMT
CMD ["irb"]
# Wed, 01 Sep 2021 08:00:22 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 01 Sep 2021 08:00:30 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 01 Sep 2021 08:00:30 GMT
ENV RAILS_ENV=production
# Wed, 01 Sep 2021 08:00:30 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Sep 2021 08:00:31 GMT
ENV HOME=/home/redmine
# Wed, 01 Sep 2021 08:00:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 01 Sep 2021 08:00:32 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 01 Sep 2021 08:00:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 01 Sep 2021 08:03:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 01 Sep 2021 08:03:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 01 Sep 2021 08:05:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 01 Sep 2021 08:05:51 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 01 Sep 2021 08:05:52 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 01 Sep 2021 08:05:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 08:05:52 GMT
EXPOSE 3000
# Wed, 01 Sep 2021 08:05:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439708bfc17dd3e86c8b1415116fcd9de1d32330bdcc8b13fd009f7727844e9`  
		Last Modified: Wed, 01 Sep 2021 05:58:07 GMT  
		Size: 3.6 MB (3581641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260bc7d8cd8f26c27362c4ab1698f2a3e0b0a88516cdfd73a8884747ec12ee`  
		Last Modified: Wed, 01 Sep 2021 05:58:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b385b36ad53753eb77bf737911b40c7b42d1d603a8005a53f2f2f9d3aa2a647`  
		Last Modified: Wed, 01 Sep 2021 05:58:33 GMT  
		Size: 14.0 MB (13991225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92418e596130e2278d466f8249bbfd0342dc1ed5615322250d5291980e5e711`  
		Last Modified: Wed, 01 Sep 2021 05:58:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb69d3417cce9a0cd0808740d79cad62e362f9e7780f9e847fda8698922434f8`  
		Last Modified: Wed, 01 Sep 2021 08:17:11 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff5239c638a3da1239c50061fdbda7f2ab705410a586090f90731563aebf09b`  
		Last Modified: Wed, 01 Sep 2021 08:17:21 GMT  
		Size: 69.5 MB (69527596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4595191c9d0a75afbae796393c0d8785fc677252ad2d85ab2cec624eb5f9c1cf`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be97b97c73e6fb6c46d0181b8440a11bc4bb76e361ae0d2fc5dc5829ad8c890`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2904ae75e075530bcb634aefc3d51e773208ce91e366be679351205797597f5b`  
		Last Modified: Wed, 01 Sep 2021 08:17:09 GMT  
		Size: 3.1 MB (3062876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aa578222ef92d9141208d74301432942113f80ee6a5498fd82515c20955471`  
		Last Modified: Wed, 01 Sep 2021 08:17:14 GMT  
		Size: 56.7 MB (56720303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f3a3dc13988389eb05a94dba971d771fb9fc0e1b3ed1fd8ba96d3f39eac1c3`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-passenger`

```console
$ docker pull redmine@sha256:dc1fa7ae440292befc3702f68fd45e6167a13086847d9c4151f3e7fddab3d679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:1384ea37efaf431cdff585a3d29cc018cacfc671a3c5e723b8f2880fa480659f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221546741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65d69f1c7954cffcb45c23d12731b72e27472b5d6ae629622df20fcda3a4d414`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:21:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:23:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:23:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:23:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:23:47 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:01:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:01:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:01:29 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:01:29 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:01:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 18:01:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:02:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:02:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:02:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:02:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:02:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 17 Aug 2021 18:02:25 GMT
ENV PASSENGER_VERSION=6.0.10
# Tue, 17 Aug 2021 18:02:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:45 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 17 Aug 2021 18:02:45 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 17 Aug 2021 18:02:45 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119720cd004c3495b5cd6b8883e01df56a3438046b3ecc3198ffb3849f6f25df`  
		Last Modified: Tue, 17 Aug 2021 04:42:13 GMT  
		Size: 14.5 MB (14510198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b764bf01e480a9fff1b3e5a263f7f9f9b4fa77325f616c37cb8e2c81d51e3dd9`  
		Last Modified: Tue, 17 Aug 2021 04:42:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84946f74729ab44aaa49a9af6012e6293fb02521ca05cffaccf128e7b157cec`  
		Last Modified: Tue, 17 Aug 2021 18:09:47 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcde4d7d6d22355ecf23701bfa1a2abba49bcabfc5f4dd90c746e0143569ba`  
		Last Modified: Tue, 17 Aug 2021 18:10:07 GMT  
		Size: 94.1 MB (94087892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5742225b6ad582633258fcf1e969851dbdd33be3d03cb05cf61b1ea900d8cc`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81933ac92f0a4be0c34689c7c3035c0aa0e4d7e89153bb41cbe0821a1c2a89f7`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb927d9d1176a8bbb1d88d687d964fae4ee7e61ebd08be4d8648f21caa9299e`  
		Last Modified: Tue, 17 Aug 2021 18:09:46 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d25f4984fe7a6089fe506ca06732024aafbfe47de090d95c448ac84b589e573`  
		Last Modified: Tue, 17 Aug 2021 18:09:53 GMT  
		Size: 44.1 MB (44122772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f790489c8bf8667ba0727c9aa46fb6e9d9128bf89a9c1330b90689f04155bf`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b74d84a329f08033107c147b415d461e38428d975adc347ea34654240ab09e`  
		Last Modified: Tue, 17 Aug 2021 18:10:30 GMT  
		Size: 21.1 MB (21131600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235136ff85630baea96544cddd34b782c51fbd5824839b6264d7ac17db683c0a`  
		Last Modified: Tue, 17 Aug 2021 18:10:27 GMT  
		Size: 4.9 MB (4919283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.2`

```console
$ docker pull redmine@sha256:946ffb0d6839fa3d89d077b47d3024b103b42f905463932ea6950703489217a7
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

### `redmine:4.2.2` - linux; amd64

```console
$ docker pull redmine@sha256:184738eb8da314459e8b41f33ffdfad41e82d466ec96843bf49cd46d1bc5109a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195495858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab3b16cafa89a7d46015d66e213c5ddc798b96e35c33ae8100fc09ba1d9525e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:21:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:23:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:23:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:23:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:23:47 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:01:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:01:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:01:29 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:01:29 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:01:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 18:01:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:02:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:02:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:02:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:02:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:02:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119720cd004c3495b5cd6b8883e01df56a3438046b3ecc3198ffb3849f6f25df`  
		Last Modified: Tue, 17 Aug 2021 04:42:13 GMT  
		Size: 14.5 MB (14510198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b764bf01e480a9fff1b3e5a263f7f9f9b4fa77325f616c37cb8e2c81d51e3dd9`  
		Last Modified: Tue, 17 Aug 2021 04:42:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84946f74729ab44aaa49a9af6012e6293fb02521ca05cffaccf128e7b157cec`  
		Last Modified: Tue, 17 Aug 2021 18:09:47 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcde4d7d6d22355ecf23701bfa1a2abba49bcabfc5f4dd90c746e0143569ba`  
		Last Modified: Tue, 17 Aug 2021 18:10:07 GMT  
		Size: 94.1 MB (94087892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5742225b6ad582633258fcf1e969851dbdd33be3d03cb05cf61b1ea900d8cc`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81933ac92f0a4be0c34689c7c3035c0aa0e4d7e89153bb41cbe0821a1c2a89f7`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb927d9d1176a8bbb1d88d687d964fae4ee7e61ebd08be4d8648f21caa9299e`  
		Last Modified: Tue, 17 Aug 2021 18:09:46 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d25f4984fe7a6089fe506ca06732024aafbfe47de090d95c448ac84b589e573`  
		Last Modified: Tue, 17 Aug 2021 18:09:53 GMT  
		Size: 44.1 MB (44122772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f790489c8bf8667ba0727c9aa46fb6e9d9128bf89a9c1330b90689f04155bf`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; arm variant v5

```console
$ docker pull redmine@sha256:2e7f776816b5769bfdaa730b3d5c3d64b1025e071ad1c79a6716eff4c1041de1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed286853331cdd20528ca2dacc87e979025cee325cdd5528cc16dd1b6558987f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:31:22 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 17:31:23 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 17:31:23 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 17:35:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:35:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:35:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:35:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:35:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:35:44 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 04:57:25 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 04:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 04:58:43 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 04:58:43 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 04:58:44 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 04:58:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 04:58:46 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 04:58:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 04:58:52 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:04:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:04:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:04:38 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:04:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:04:39 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:04:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add78f82744b7f4c8c7522adfae87214be4104b79f343add868890b00ec859d2`  
		Last Modified: Fri, 03 Sep 2021 18:01:59 GMT  
		Size: 13.9 MB (13871472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea079592f786a6bd50d8249c1ceedc638402805fe700febed7e646dd69ee642`  
		Last Modified: Fri, 03 Sep 2021 18:01:51 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217f2b4088020d7dcc1aed89a3d8db9a8756c8bee078541881250a9dbbad1e6`  
		Last Modified: Sat, 04 Sep 2021 05:20:20 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5101e0f6c49b2df1f4b08067b3c1b135fe25243c4054b5868f953bc3f37490bf`  
		Last Modified: Sat, 04 Sep 2021 05:21:21 GMT  
		Size: 89.6 MB (89576088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ae1568de59acec6c4cb2932be2397e122fea3950b3104ce626623970d75f5`  
		Last Modified: Sat, 04 Sep 2021 05:20:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e297238097a4d3b15fbadef5aa4d865ab9cef981d1cae1bb633f216dd4c9dad`  
		Last Modified: Sat, 04 Sep 2021 05:20:18 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6628563efc672886d9ef6550835ad5efa230a1e39f41e8e612ad2af2c4e7ba99`  
		Last Modified: Sat, 04 Sep 2021 05:20:21 GMT  
		Size: 3.1 MB (3061924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0be986223cb5256d684c7602b705f39bd686a8ffb95e92c116f1db188b1da6`  
		Last Modified: Sat, 04 Sep 2021 05:20:43 GMT  
		Size: 55.2 MB (55234623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcee35bd3d5db50a493ba5105b6272ef59dc2eb800bb91c4eef2c100309638c`  
		Last Modified: Sat, 04 Sep 2021 05:20:18 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cd7275a7d34b3290a919f94e8e29ca61a913d0427cd2718ed49e354450b9eb2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0f96d1f050b7bd3415163fa63302bbaf4443e8741688fdcbbe19819f034e55`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:30:30 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 09:44:16 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 09:44:17 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 09:44:17 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 09:48:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 09:48:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 09:48:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 09:48:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:48:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 09:48:25 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 08:32:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 08:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:33:59 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 08:33:59 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 08:34:00 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 08:34:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 08:34:02 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 18 Aug 2021 08:34:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 18 Aug 2021 08:34:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 08:39:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 08:39:27 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 08:39:27 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 08:39:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 08:39:28 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 08:39:29 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79875132dbc48a8386eb9079eb8b50d17399ed33c29a51ac8d7b2f943f3b1ac`  
		Last Modified: Tue, 17 Aug 2021 10:24:54 GMT  
		Size: 9.9 MB (9872248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ce2d51bf7561cb7c360e69499b42694c2e474b2f24d969e4250ac389dd4bec`  
		Last Modified: Tue, 17 Aug 2021 10:24:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6910fec61b3de474c201c0eaae12d42336d748c8d6c55e7b06571adfef449ac`  
		Last Modified: Tue, 17 Aug 2021 10:26:58 GMT  
		Size: 13.8 MB (13767304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376804c80b6dffd48a9a1ce10f9ae6e593d25030de692dfc17341be078eaad9f`  
		Last Modified: Tue, 17 Aug 2021 10:26:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d2abf0978eca4cf58f5136adb1c1db17ff192b414feb932d7a524feb862a06`  
		Last Modified: Wed, 18 Aug 2021 08:54:19 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25cf090ed21d7e7a084b69c43bc419fc12838e33b344eba331171fc2868d53d`  
		Last Modified: Wed, 18 Aug 2021 08:54:58 GMT  
		Size: 85.6 MB (85590672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782c9d20468a0cc0f8d38101ddc7ef218d18c48ecbeda7932121ed297886d697`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eab3d69b805b2536e4dd6b587ff8eb27d96f2df1057e5e31d91410e872d74f`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b22a54dbdc1d4adfc0f8ae626f1aed9ec9010d827a989cf4af007f1126801d`  
		Last Modified: Wed, 18 Aug 2021 08:54:20 GMT  
		Size: 3.1 MB (3061921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2005224b6c07acc4bbabc1a0bb15ec249509c15fcfd8d777031ad7050b6ce1ac`  
		Last Modified: Wed, 18 Aug 2021 08:54:34 GMT  
		Size: 55.1 MB (55073085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1537e502cf0def19348a8406f66144d8986698047998e80c0a8ce7c1759735`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:54281b02713340086f8270560a0a6f34bd50ef111b8136870436e66a36c494b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203249301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c7d37a5bf5a362ddcdb750e1beba28d0362bd1632eaf9ed4bea0913ac529f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 12:12:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:12:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:12:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:12:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:12:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:12:43 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:04:14 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:04:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:04:38 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:04:38 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:04:39 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:04:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:04:39 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 05:04:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 05:04:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:07:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:07:20 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:07:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:07:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:07:21 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:07:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee312ced32893df36a25a76149db554574daaeb35128bcfb8c1d9d5bbc1fe73d`  
		Last Modified: Fri, 03 Sep 2021 12:28:34 GMT  
		Size: 14.4 MB (14356717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719ff35ff5b1cf24bc8a71ce6e567a505fbb6fcf0e9c141d8bdc230f164a57a0`  
		Last Modified: Fri, 03 Sep 2021 12:28:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd82b0673245cfbd7fe883e89fb55be7bd3e805e26de6ef17064f507f3df13c`  
		Last Modified: Sat, 04 Sep 2021 05:13:30 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d090f849a4da11b63677dfaff64f9709e15e9a24e740bcfbbca2545dc3f6395`  
		Last Modified: Sat, 04 Sep 2021 05:13:46 GMT  
		Size: 92.6 MB (92609378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9748bdee2b0b6d123ea99593dc5ff47d2b23dc011f52aef631f6eff5be900547`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454a0d8da53bfccd39f515fb93989777b3b6ebfc7c78bcb00be2b2e831683de`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323cf17e748812ba32fb6ed26e50ba83a1ddc4ec3eb22dc3674a4ddfc7ab2674`  
		Last Modified: Sat, 04 Sep 2021 05:13:29 GMT  
		Size: 3.1 MB (3061917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f679bdbfd5dafda429d92ba97d958576ee482d6c7e7ef09611df897a8af86ee7`  
		Last Modified: Sat, 04 Sep 2021 05:13:34 GMT  
		Size: 56.0 MB (56037790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080fea9fe34c2c40a03359a1c3402d684badf754bb190a6f22679e53c3d25c08`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; 386

```console
$ docker pull redmine@sha256:ebc552d443096692ec50b0c4279d2cfef5098651e51fab433fa57a8859e864c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202126624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c6ceb9f5cc0c343839ed2f1ed0ac64ccf12847ac4939e863d82309c42e9ec3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:39:26 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 11:39:27 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 11:39:27 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 11:43:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 11:43:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 11:43:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 11:43:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 11:43:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 11:43:41 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 06:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 06:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 06:05:58 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 06:05:59 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 06:05:59 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 06:06:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 06:06:01 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 06:06:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 06:06:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 06:07:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 06:07:41 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 06:07:42 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 06:07:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 06:07:42 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 06:07:43 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ab3f959a8410b96952c0ab29ff5376ff960f0c46619b9da4de191c3e631a2e`  
		Last Modified: Fri, 03 Sep 2021 12:10:29 GMT  
		Size: 14.0 MB (13992725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b213d5105e1a800ff597002681646442fd6df3b46274ee545c1825df025af800`  
		Last Modified: Fri, 03 Sep 2021 12:10:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fa640c55779f987dc35c6cc6766cb5f2fa277c85a28f8b096f1276dedc45ba`  
		Last Modified: Sat, 04 Sep 2021 06:16:20 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae199078f5eaaf3ea967d1448f821631d10ea7afd47dcb79a7701e0fe24ed70`  
		Last Modified: Sat, 04 Sep 2021 06:16:43 GMT  
		Size: 95.7 MB (95703257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61de99b7f1e5da0063d2955ec7a01f01d7ed345b8b6dd804aada111402bf9f`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ba76c31dcad016bf941f0e0be2694f0fa339e5c24d7ef5ee4916be74697f0a`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70e46e86bb38bc42f7060c39fbbc233ea20e6f7089b73e2335d3440c1c33d1`  
		Last Modified: Sat, 04 Sep 2021 06:16:18 GMT  
		Size: 3.1 MB (3061914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb99b00b084c4a0e83a272f225159c4cbf6214c81fe2f8571dfaf4276978ce97`  
		Last Modified: Sat, 04 Sep 2021 06:16:25 GMT  
		Size: 44.3 MB (44340016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cbcc1c6467ba9477359f3f850d4c4535ba281eea1e75124bb96d94ba91c2fa`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; ppc64le

```console
$ docker pull redmine@sha256:750c649c6ed54a1bc79c41c44b1bfb009a38e130ca51356a0a5637a77b452f5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219650978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3733a5127a682e88605681a10a6637a271090e9dddd1ecb6d71d7b4e0b6d2c82`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:32:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:32:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 09:53:38 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 09:53:41 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 09:53:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 10:00:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:00:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:00:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:01:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:01:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:01:28 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 06:54:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 06:59:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:00:07 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 07:00:21 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 07:00:26 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 07:00:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 07:00:43 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 18 Aug 2021 07:00:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 18 Aug 2021 07:01:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 07:07:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 07:07:18 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 07:07:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 07:07:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 07:07:39 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 07:07:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6540cca707f751654267130c5ff13338c730506cf900ab70cbba8eb8f0774f4`  
		Last Modified: Tue, 17 Aug 2021 10:35:53 GMT  
		Size: 12.7 MB (12704229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cb3d072ea667e9971932f23c9c5ddffe4a2d7c9a645aa1f53235dc8c2e2ae5`  
		Last Modified: Tue, 17 Aug 2021 10:35:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29445a92f99df6ece2c68fdd21d13b23e28c76507ae5fc4497cbf9272cd41e91`  
		Last Modified: Tue, 17 Aug 2021 10:37:15 GMT  
		Size: 15.0 MB (14997282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee87ac0f307c59470977ad0b974013269088413f9061698138c7f01175ec9982`  
		Last Modified: Tue, 17 Aug 2021 10:37:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfb261039caaf3d27ac4757a6a0ca770e695ac15e72cce135badcdf8d17b060`  
		Last Modified: Wed, 18 Aug 2021 07:40:45 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa4557b0838e19c4cd9f385a4b5ea0972af6fba31e8bcc39e77336887cd48ee`  
		Last Modified: Wed, 18 Aug 2021 07:41:48 GMT  
		Size: 101.3 MB (101328471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5cb4e6a472bc1f6140175c495cf2115da58206520a01bca00638227f2370ea`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4789be342e86d5f2793092f064c41fde923d87fb85f130d8100b4c88af3474`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2190284052685dcbf10a7e8e39410965a72be33c4c924cedc97130de22e6c8f4`  
		Last Modified: Wed, 18 Aug 2021 07:40:52 GMT  
		Size: 3.1 MB (3061910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b6fa0cc2de623e70d74216ebe78d7dfccc76bda34aae287ec61259ff3f54ce`  
		Last Modified: Wed, 18 Aug 2021 07:41:17 GMT  
		Size: 57.0 MB (57001117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164f878c998618c80d1e4d55973b954723ba05120f5a4984c112bc210edd8c6`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; s390x

```console
$ docker pull redmine@sha256:f764e6f237dd0b4ccc459c4a58872d66f5d9015fa61828ef337cc1aba2dde405
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202557142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:182cde8e814a22a30968ac8996e2499e862f311f0c6cd3a5d1db75334c1b9dce`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 13:38:11 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 13:38:11 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 13:38:12 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 13:41:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 13:41:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 13:41:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 13:41:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 13:41:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 13:41:45 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 02:39:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 02:40:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:40:18 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 02:40:18 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 02:40:19 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 02:40:19 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 02:40:19 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 02:40:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 02:40:23 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 02:42:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 02:42:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 02:42:50 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 02:42:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:42:51 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 02:42:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ea6888b61e31cb5b4a8f014006c7cb8fa8a3b7224b7ad3f0b4af257229c789`  
		Last Modified: Fri, 03 Sep 2021 14:14:23 GMT  
		Size: 14.7 MB (14697502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ef0cfb1210ec8b5dff947c27988590a3931cf76a1437a6fe10f30aae9f813`  
		Last Modified: Fri, 03 Sep 2021 14:14:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a04f5ff5ec2ee8dd1b21974adff7bf0e6fdb70338e190c6094eed2747ceb117`  
		Last Modified: Sat, 04 Sep 2021 02:50:16 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf9140fc0de2f47daa7719c6c1cbbf193066ad2a67f60c95d78b7baf3626508`  
		Last Modified: Sat, 04 Sep 2021 02:50:29 GMT  
		Size: 91.8 MB (91790843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d640980eb96fb9f7eef22043b3c502898b8cc3f7b1447f1f19055222d3a3bf`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80df1a5482c5309af87986c42c45a6cd4c0cfbce1535792b2c1ba652e2c2a304`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9bc3013aec1061db002a07fa5ae39181287f086837e8c8c53c5814049c837d`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 3.1 MB (3061916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9caa222bcb2e88202afcfdf166e5a0613fe99bc55cc9b416dda1e1e2484c4`  
		Last Modified: Sat, 04 Sep 2021 02:50:19 GMT  
		Size: 56.4 MB (56426601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff0983c6ea2bc0e811104db8303487a7286daf0ee17c051de72eb5e75dbbc32`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.2-alpine`

```console
$ docker pull redmine@sha256:b3f4c38a52e764136b2d930a044a60e362120dd0c8900217a3e90e852421ab31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2.2-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:c5db53d0c811b57d386d30b72d9050a7aa2fe1cf1b73fd86e20caaf5794597b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.7 MB (149701448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e405182f204a9a00f59a9abe4dd5e343cc108150ea4d66c36d925aed95a284`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:46:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Sep 2021 05:46:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Sep 2021 05:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_MAJOR=2.7
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Wed, 01 Sep 2021 05:53:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Sep 2021 05:53:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Sep 2021 05:53:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Sep 2021 05:53:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 05:53:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Sep 2021 05:53:30 GMT
CMD ["irb"]
# Wed, 01 Sep 2021 08:00:22 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 01 Sep 2021 08:00:30 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 01 Sep 2021 08:00:30 GMT
ENV RAILS_ENV=production
# Wed, 01 Sep 2021 08:00:30 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Sep 2021 08:00:31 GMT
ENV HOME=/home/redmine
# Wed, 01 Sep 2021 08:00:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 01 Sep 2021 08:00:32 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 01 Sep 2021 08:00:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 01 Sep 2021 08:03:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 01 Sep 2021 08:03:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 01 Sep 2021 08:05:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 01 Sep 2021 08:05:51 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 01 Sep 2021 08:05:52 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 01 Sep 2021 08:05:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 08:05:52 GMT
EXPOSE 3000
# Wed, 01 Sep 2021 08:05:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439708bfc17dd3e86c8b1415116fcd9de1d32330bdcc8b13fd009f7727844e9`  
		Last Modified: Wed, 01 Sep 2021 05:58:07 GMT  
		Size: 3.6 MB (3581641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260bc7d8cd8f26c27362c4ab1698f2a3e0b0a88516cdfd73a8884747ec12ee`  
		Last Modified: Wed, 01 Sep 2021 05:58:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b385b36ad53753eb77bf737911b40c7b42d1d603a8005a53f2f2f9d3aa2a647`  
		Last Modified: Wed, 01 Sep 2021 05:58:33 GMT  
		Size: 14.0 MB (13991225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92418e596130e2278d466f8249bbfd0342dc1ed5615322250d5291980e5e711`  
		Last Modified: Wed, 01 Sep 2021 05:58:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb69d3417cce9a0cd0808740d79cad62e362f9e7780f9e847fda8698922434f8`  
		Last Modified: Wed, 01 Sep 2021 08:17:11 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff5239c638a3da1239c50061fdbda7f2ab705410a586090f90731563aebf09b`  
		Last Modified: Wed, 01 Sep 2021 08:17:21 GMT  
		Size: 69.5 MB (69527596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4595191c9d0a75afbae796393c0d8785fc677252ad2d85ab2cec624eb5f9c1cf`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be97b97c73e6fb6c46d0181b8440a11bc4bb76e361ae0d2fc5dc5829ad8c890`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2904ae75e075530bcb634aefc3d51e773208ce91e366be679351205797597f5b`  
		Last Modified: Wed, 01 Sep 2021 08:17:09 GMT  
		Size: 3.1 MB (3062876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aa578222ef92d9141208d74301432942113f80ee6a5498fd82515c20955471`  
		Last Modified: Wed, 01 Sep 2021 08:17:14 GMT  
		Size: 56.7 MB (56720303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f3a3dc13988389eb05a94dba971d771fb9fc0e1b3ed1fd8ba96d3f39eac1c3`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.2-passenger`

```console
$ docker pull redmine@sha256:dc1fa7ae440292befc3702f68fd45e6167a13086847d9c4151f3e7fddab3d679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2.2-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:1384ea37efaf431cdff585a3d29cc018cacfc671a3c5e723b8f2880fa480659f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221546741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65d69f1c7954cffcb45c23d12731b72e27472b5d6ae629622df20fcda3a4d414`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:21:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:23:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:23:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:23:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:23:47 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:01:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:01:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:01:29 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:01:29 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:01:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 18:01:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:02:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:02:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:02:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:02:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:02:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 17 Aug 2021 18:02:25 GMT
ENV PASSENGER_VERSION=6.0.10
# Tue, 17 Aug 2021 18:02:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:45 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 17 Aug 2021 18:02:45 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 17 Aug 2021 18:02:45 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119720cd004c3495b5cd6b8883e01df56a3438046b3ecc3198ffb3849f6f25df`  
		Last Modified: Tue, 17 Aug 2021 04:42:13 GMT  
		Size: 14.5 MB (14510198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b764bf01e480a9fff1b3e5a263f7f9f9b4fa77325f616c37cb8e2c81d51e3dd9`  
		Last Modified: Tue, 17 Aug 2021 04:42:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84946f74729ab44aaa49a9af6012e6293fb02521ca05cffaccf128e7b157cec`  
		Last Modified: Tue, 17 Aug 2021 18:09:47 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcde4d7d6d22355ecf23701bfa1a2abba49bcabfc5f4dd90c746e0143569ba`  
		Last Modified: Tue, 17 Aug 2021 18:10:07 GMT  
		Size: 94.1 MB (94087892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5742225b6ad582633258fcf1e969851dbdd33be3d03cb05cf61b1ea900d8cc`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81933ac92f0a4be0c34689c7c3035c0aa0e4d7e89153bb41cbe0821a1c2a89f7`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb927d9d1176a8bbb1d88d687d964fae4ee7e61ebd08be4d8648f21caa9299e`  
		Last Modified: Tue, 17 Aug 2021 18:09:46 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d25f4984fe7a6089fe506ca06732024aafbfe47de090d95c448ac84b589e573`  
		Last Modified: Tue, 17 Aug 2021 18:09:53 GMT  
		Size: 44.1 MB (44122772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f790489c8bf8667ba0727c9aa46fb6e9d9128bf89a9c1330b90689f04155bf`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b74d84a329f08033107c147b415d461e38428d975adc347ea34654240ab09e`  
		Last Modified: Tue, 17 Aug 2021 18:10:30 GMT  
		Size: 21.1 MB (21131600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235136ff85630baea96544cddd34b782c51fbd5824839b6264d7ac17db683c0a`  
		Last Modified: Tue, 17 Aug 2021 18:10:27 GMT  
		Size: 4.9 MB (4919283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:alpine`

```console
$ docker pull redmine@sha256:b3f4c38a52e764136b2d930a044a60e362120dd0c8900217a3e90e852421ab31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:c5db53d0c811b57d386d30b72d9050a7aa2fe1cf1b73fd86e20caaf5794597b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.7 MB (149701448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49e405182f204a9a00f59a9abe4dd5e343cc108150ea4d66c36d925aed95a284`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 05:46:58 GMT
RUN set -eux; 	apk add --no-cache 		bzip2 		ca-certificates 		gmp-dev 		libffi-dev 		procps 		yaml-dev 		zlib-dev 	;
# Wed, 01 Sep 2021 05:46:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 01 Sep 2021 05:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_MAJOR=2.7
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 01 Sep 2021 05:50:53 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Wed, 01 Sep 2021 05:53:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .ruby-builddeps 		autoconf 		bison 		bzip2 		bzip2-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		g++ 		gcc 		gdbm-dev 		glib-dev 		libc-dev 		libffi-dev 		libxml2-dev 		libxslt-dev 		linux-headers 		make 		ncurses-dev 		openssl 		openssl-dev 		patch 		procps 		readline-dev 		ruby 		tar 		xz 		yaml-dev 		zlib-dev 	; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		wget -O 'thread-stack-fix.patch' 'https://bugs.ruby-lang.org/attachments/download/7081/0001-thread_pthread.c-make-get_main_stack-portable-on-lin.patch'; 	echo '3ab628a51d92fdf0d2b5835e93564857aea73e0c1de00313864a94a6255cb645 *thread-stack-fix.patch' | sha256sum --check --strict; 	patch -p1 -i thread-stack-fix.patch; 	rm thread-stack-fix.patch; 		export ac_cv_func_isnan=yes ac_cv_func_isinf=yes; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .ruby-rundeps $runDeps; 	apk del --no-network .ruby-builddeps; 		cd /; 	rm -r /usr/src/ruby; 	if 		apk --no-network list --installed 			| grep -v '^[.]ruby-rundeps' 			| grep -i ruby 	; then 		exit 1; 	fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Sep 2021 05:53:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Sep 2021 05:53:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Sep 2021 05:53:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Sep 2021 05:53:30 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Sep 2021 05:53:30 GMT
CMD ["irb"]
# Wed, 01 Sep 2021 08:00:22 GMT
RUN addgroup -S -g 1000 redmine && adduser -S -H -G redmine -u 999 redmine
# Wed, 01 Sep 2021 08:00:30 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ca-certificates 		su-exec 		tini 		tzdata 		wget 				git 		mercurial 		openssh-client 		subversion 				ghostscript 		ghostscript-fonts 		imagemagick 	;
# Wed, 01 Sep 2021 08:00:30 GMT
ENV RAILS_ENV=production
# Wed, 01 Sep 2021 08:00:30 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Sep 2021 08:00:31 GMT
ENV HOME=/home/redmine
# Wed, 01 Sep 2021 08:00:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 01 Sep 2021 08:00:32 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 01 Sep 2021 08:00:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 01 Sep 2021 08:03:39 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 01 Sep 2021 08:03:39 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Wed, 01 Sep 2021 08:05:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 01 Sep 2021 08:05:51 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 01 Sep 2021 08:05:52 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Wed, 01 Sep 2021 08:05:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 01 Sep 2021 08:05:52 GMT
EXPOSE 3000
# Wed, 01 Sep 2021 08:05:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4439708bfc17dd3e86c8b1415116fcd9de1d32330bdcc8b13fd009f7727844e9`  
		Last Modified: Wed, 01 Sep 2021 05:58:07 GMT  
		Size: 3.6 MB (3581641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88260bc7d8cd8f26c27362c4ab1698f2a3e0b0a88516cdfd73a8884747ec12ee`  
		Last Modified: Wed, 01 Sep 2021 05:58:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b385b36ad53753eb77bf737911b40c7b42d1d603a8005a53f2f2f9d3aa2a647`  
		Last Modified: Wed, 01 Sep 2021 05:58:33 GMT  
		Size: 14.0 MB (13991225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92418e596130e2278d466f8249bbfd0342dc1ed5615322250d5291980e5e711`  
		Last Modified: Wed, 01 Sep 2021 05:58:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb69d3417cce9a0cd0808740d79cad62e362f9e7780f9e847fda8698922434f8`  
		Last Modified: Wed, 01 Sep 2021 08:17:11 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff5239c638a3da1239c50061fdbda7f2ab705410a586090f90731563aebf09b`  
		Last Modified: Wed, 01 Sep 2021 08:17:21 GMT  
		Size: 69.5 MB (69527596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4595191c9d0a75afbae796393c0d8785fc677252ad2d85ab2cec624eb5f9c1cf`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be97b97c73e6fb6c46d0181b8440a11bc4bb76e361ae0d2fc5dc5829ad8c890`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2904ae75e075530bcb634aefc3d51e773208ce91e366be679351205797597f5b`  
		Last Modified: Wed, 01 Sep 2021 08:17:09 GMT  
		Size: 3.1 MB (3062876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4aa578222ef92d9141208d74301432942113f80ee6a5498fd82515c20955471`  
		Last Modified: Wed, 01 Sep 2021 08:17:14 GMT  
		Size: 56.7 MB (56720303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f3a3dc13988389eb05a94dba971d771fb9fc0e1b3ed1fd8ba96d3f39eac1c3`  
		Last Modified: Wed, 01 Sep 2021 08:17:08 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:latest`

```console
$ docker pull redmine@sha256:946ffb0d6839fa3d89d077b47d3024b103b42f905463932ea6950703489217a7
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
$ docker pull redmine@sha256:184738eb8da314459e8b41f33ffdfad41e82d466ec96843bf49cd46d1bc5109a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.5 MB (195495858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fab3b16cafa89a7d46015d66e213c5ddc798b96e35c33ae8100fc09ba1d9525e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:21:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:23:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:23:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:23:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:23:47 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:01:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:01:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:01:29 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:01:29 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:01:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 18:01:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:02:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:02:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:02:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:02:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:02:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119720cd004c3495b5cd6b8883e01df56a3438046b3ecc3198ffb3849f6f25df`  
		Last Modified: Tue, 17 Aug 2021 04:42:13 GMT  
		Size: 14.5 MB (14510198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b764bf01e480a9fff1b3e5a263f7f9f9b4fa77325f616c37cb8e2c81d51e3dd9`  
		Last Modified: Tue, 17 Aug 2021 04:42:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84946f74729ab44aaa49a9af6012e6293fb02521ca05cffaccf128e7b157cec`  
		Last Modified: Tue, 17 Aug 2021 18:09:47 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcde4d7d6d22355ecf23701bfa1a2abba49bcabfc5f4dd90c746e0143569ba`  
		Last Modified: Tue, 17 Aug 2021 18:10:07 GMT  
		Size: 94.1 MB (94087892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5742225b6ad582633258fcf1e969851dbdd33be3d03cb05cf61b1ea900d8cc`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81933ac92f0a4be0c34689c7c3035c0aa0e4d7e89153bb41cbe0821a1c2a89f7`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb927d9d1176a8bbb1d88d687d964fae4ee7e61ebd08be4d8648f21caa9299e`  
		Last Modified: Tue, 17 Aug 2021 18:09:46 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d25f4984fe7a6089fe506ca06732024aafbfe47de090d95c448ac84b589e573`  
		Last Modified: Tue, 17 Aug 2021 18:09:53 GMT  
		Size: 44.1 MB (44122772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f790489c8bf8667ba0727c9aa46fb6e9d9128bf89a9c1330b90689f04155bf`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:2e7f776816b5769bfdaa730b3d5c3d64b1025e071ad1c79a6716eff4c1041de1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196976290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed286853331cdd20528ca2dacc87e979025cee325cdd5528cc16dd1b6558987f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:51:26 GMT
ADD file:350748a564076da397b991745cd42e0688d15c72b9fd5c81f8ea0bb8938a2b3d in / 
# Fri, 03 Sep 2021 00:51:27 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 17:13:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 17:13:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 17:13:23 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 17:31:22 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 17:31:23 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 17:31:23 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 17:35:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 17:35:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 17:35:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 17:35:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 17:35:44 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 17:35:44 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 04:57:25 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 04:58:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 04:58:43 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 04:58:43 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 04:58:44 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 04:58:45 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 04:58:46 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 04:58:46 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 04:58:52 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:04:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:04:37 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:04:38 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:04:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:04:39 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:04:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:b019db4b5197128481d48d92ecacd6bb356c027a3d08393f6567a6fa183ba769`  
		Last Modified: Fri, 03 Sep 2021 01:07:12 GMT  
		Size: 24.9 MB (24879114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e8f8df1e487d27a05b0b6946a50c5bc5d13c6f0d6c7d0ce2e648c463894acb6`  
		Last Modified: Fri, 03 Sep 2021 17:59:54 GMT  
		Size: 10.3 MB (10348838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863ca6c4a66e09b6ea6dc6d707ea0bc32957f79282e4dafdf6c02743317f2dbc`  
		Last Modified: Fri, 03 Sep 2021 17:59:45 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add78f82744b7f4c8c7522adfae87214be4104b79f343add868890b00ec859d2`  
		Last Modified: Fri, 03 Sep 2021 18:01:59 GMT  
		Size: 13.9 MB (13871472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea079592f786a6bd50d8249c1ceedc638402805fe700febed7e646dd69ee642`  
		Last Modified: Fri, 03 Sep 2021 18:01:51 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6217f2b4088020d7dcc1aed89a3d8db9a8756c8bee078541881250a9dbbad1e6`  
		Last Modified: Sat, 04 Sep 2021 05:20:20 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5101e0f6c49b2df1f4b08067b3c1b135fe25243c4054b5868f953bc3f37490bf`  
		Last Modified: Sat, 04 Sep 2021 05:21:21 GMT  
		Size: 89.6 MB (89576088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398ae1568de59acec6c4cb2932be2397e122fea3950b3104ce626623970d75f5`  
		Last Modified: Sat, 04 Sep 2021 05:20:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e297238097a4d3b15fbadef5aa4d865ab9cef981d1cae1bb633f216dd4c9dad`  
		Last Modified: Sat, 04 Sep 2021 05:20:18 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6628563efc672886d9ef6550835ad5efa230a1e39f41e8e612ad2af2c4e7ba99`  
		Last Modified: Sat, 04 Sep 2021 05:20:21 GMT  
		Size: 3.1 MB (3061924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0be986223cb5256d684c7602b705f39bd686a8ffb95e92c116f1db188b1da6`  
		Last Modified: Sat, 04 Sep 2021 05:20:43 GMT  
		Size: 55.2 MB (55234623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcee35bd3d5db50a493ba5105b6272ef59dc2eb800bb91c4eef2c100309638c`  
		Last Modified: Sat, 04 Sep 2021 05:20:18 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cd7275a7d34b3290a919f94e8e29ca61a913d0427cd2718ed49e354450b9eb2e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f0f96d1f050b7bd3415163fa63302bbaf4443e8741688fdcbbe19819f034e55`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 02:14:25 GMT
ADD file:ca8cc4b509e305fa07662fbf2234ed78f0056569f6ca047305dc02bcd60f1558 in / 
# Tue, 17 Aug 2021 02:14:26 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:30:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:30:30 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:30:30 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 09:44:16 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 09:44:17 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 09:44:17 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 09:48:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 09:48:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 09:48:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 09:48:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 09:48:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 09:48:25 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 08:32:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 08:33:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 08:33:59 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 08:33:59 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 08:34:00 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 08:34:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 08:34:02 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 18 Aug 2021 08:34:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 18 Aug 2021 08:34:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 08:39:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 08:39:27 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 08:39:27 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 08:39:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 08:39:28 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 08:39:29 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:13e3f03410ff211945a725435c13065288d48a8cb740f0530e7588012c2679a4`  
		Last Modified: Tue, 17 Aug 2021 02:30:58 GMT  
		Size: 22.7 MB (22746254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79875132dbc48a8386eb9079eb8b50d17399ed33c29a51ac8d7b2f943f3b1ac`  
		Last Modified: Tue, 17 Aug 2021 10:24:54 GMT  
		Size: 9.9 MB (9872248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ce2d51bf7561cb7c360e69499b42694c2e474b2f24d969e4250ac389dd4bec`  
		Last Modified: Tue, 17 Aug 2021 10:24:46 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6910fec61b3de474c201c0eaae12d42336d748c8d6c55e7b06571adfef449ac`  
		Last Modified: Tue, 17 Aug 2021 10:26:58 GMT  
		Size: 13.8 MB (13767304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376804c80b6dffd48a9a1ce10f9ae6e593d25030de692dfc17341be078eaad9f`  
		Last Modified: Tue, 17 Aug 2021 10:26:51 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d2abf0978eca4cf58f5136adb1c1db17ff192b414feb932d7a524feb862a06`  
		Last Modified: Wed, 18 Aug 2021 08:54:19 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d25cf090ed21d7e7a084b69c43bc419fc12838e33b344eba331171fc2868d53d`  
		Last Modified: Wed, 18 Aug 2021 08:54:58 GMT  
		Size: 85.6 MB (85590672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782c9d20468a0cc0f8d38101ddc7ef218d18c48ecbeda7932121ed297886d697`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9eab3d69b805b2536e4dd6b587ff8eb27d96f2df1057e5e31d91410e872d74f`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1b22a54dbdc1d4adfc0f8ae626f1aed9ec9010d827a989cf4af007f1126801d`  
		Last Modified: Wed, 18 Aug 2021 08:54:20 GMT  
		Size: 3.1 MB (3061921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2005224b6c07acc4bbabc1a0bb15ec249509c15fcfd8d777031ad7050b6ce1ac`  
		Last Modified: Wed, 18 Aug 2021 08:54:34 GMT  
		Size: 55.1 MB (55073085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1537e502cf0def19348a8406f66144d8986698047998e80c0a8ce7c1759735`  
		Last Modified: Wed, 18 Aug 2021 08:54:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:54281b02713340086f8270560a0a6f34bd50ef111b8136870436e66a36c494b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203249301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41c7d37a5bf5a362ddcdb750e1beba28d0362bd1632eaf9ed4bea0913ac529f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:58 GMT
ADD file:4a1d7f2d989aee6bd83da076b6e9dd3da2da97cf5654bd37568e9baec30ac4b1 in / 
# Fri, 03 Sep 2021 00:40:58 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 12:01:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 12:01:36 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 12:01:36 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 12:10:44 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 12:12:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 12:12:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 12:12:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 12:12:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 12:12:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 12:12:43 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 05:04:14 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 05:04:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 05:04:38 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 05:04:38 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 05:04:39 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 05:04:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 05:04:39 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 05:04:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 05:04:43 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 05:07:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 05:07:20 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 05:07:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 05:07:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 05:07:21 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 05:07:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d10c227306ce3db344a8399cbc02bbf0dcb36519318efbde3c6027c00be8b40e`  
		Last Modified: Fri, 03 Sep 2021 00:49:47 GMT  
		Size: 25.9 MB (25914860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f19eba765a6899923dd50bf6c4c106baa13650bb0c41770d08be1ff969a12bf`  
		Last Modified: Fri, 03 Sep 2021 12:26:54 GMT  
		Size: 11.3 MB (11264405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e990790fb0b00dbc1b9eb90bac6e9cfc19c66241dd3bd75a25639cda36ce7b7e`  
		Last Modified: Fri, 03 Sep 2021 12:26:51 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee312ced32893df36a25a76149db554574daaeb35128bcfb8c1d9d5bbc1fe73d`  
		Last Modified: Fri, 03 Sep 2021 12:28:34 GMT  
		Size: 14.4 MB (14356717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719ff35ff5b1cf24bc8a71ce6e567a505fbb6fcf0e9c141d8bdc230f164a57a0`  
		Last Modified: Fri, 03 Sep 2021 12:28:32 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd82b0673245cfbd7fe883e89fb55be7bd3e805e26de6ef17064f507f3df13c`  
		Last Modified: Sat, 04 Sep 2021 05:13:30 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d090f849a4da11b63677dfaff64f9709e15e9a24e740bcfbbca2545dc3f6395`  
		Last Modified: Sat, 04 Sep 2021 05:13:46 GMT  
		Size: 92.6 MB (92609378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9748bdee2b0b6d123ea99593dc5ff47d2b23dc011f52aef631f6eff5be900547`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d454a0d8da53bfccd39f515fb93989777b3b6ebfc7c78bcb00be2b2e831683de`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:323cf17e748812ba32fb6ed26e50ba83a1ddc4ec3eb22dc3674a4ddfc7ab2674`  
		Last Modified: Sat, 04 Sep 2021 05:13:29 GMT  
		Size: 3.1 MB (3061917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f679bdbfd5dafda429d92ba97d958576ee482d6c7e7ef09611df897a8af86ee7`  
		Last Modified: Sat, 04 Sep 2021 05:13:34 GMT  
		Size: 56.0 MB (56037790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080fea9fe34c2c40a03359a1c3402d684badf754bb190a6f22679e53c3d25c08`  
		Last Modified: Sat, 04 Sep 2021 05:13:28 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:ebc552d443096692ec50b0c4279d2cfef5098651e51fab433fa57a8859e864c2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202126624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02c6ceb9f5cc0c343839ed2f1ed0ac64ccf12847ac4939e863d82309c42e9ec3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:40:24 GMT
ADD file:6bf4b6f4aa28306610ef10c68f422a7210ff2fbd5345cec07bc5f76d54a4c8bc in / 
# Fri, 03 Sep 2021 00:40:24 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 11:21:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 11:21:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 11:21:09 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 11:39:26 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 11:39:27 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 11:39:27 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 11:43:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 11:43:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 11:43:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 11:43:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 11:43:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 11:43:41 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 06:05:01 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 06:05:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 06:05:58 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 06:05:59 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 06:05:59 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 06:06:01 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 06:06:01 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 06:06:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 06:06:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 06:07:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 06:07:41 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 06:07:42 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 06:07:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 06:07:42 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 06:07:43 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7e87f600658a0c0d3bd8b82b9c645b5ec2763492ec627c1c1c1183c2ad3c45d5`  
		Last Modified: Fri, 03 Sep 2021 00:49:06 GMT  
		Size: 27.8 MB (27797513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3423e5cbd2a0657c56efff2a92252eba56c2ea1dcf18251bc253f0c5b45d80`  
		Last Modified: Fri, 03 Sep 2021 12:08:35 GMT  
		Size: 17.2 MB (17226971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b80f06d576699b2289ef93783544e8963f3280b94908fa6cd4f0826d5a5023`  
		Last Modified: Fri, 03 Sep 2021 12:08:26 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ab3f959a8410b96952c0ab29ff5376ff960f0c46619b9da4de191c3e631a2e`  
		Last Modified: Fri, 03 Sep 2021 12:10:29 GMT  
		Size: 14.0 MB (13992725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b213d5105e1a800ff597002681646442fd6df3b46274ee545c1825df025af800`  
		Last Modified: Fri, 03 Sep 2021 12:10:25 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26fa640c55779f987dc35c6cc6766cb5f2fa277c85a28f8b096f1276dedc45ba`  
		Last Modified: Sat, 04 Sep 2021 06:16:20 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae199078f5eaaf3ea967d1448f821631d10ea7afd47dcb79a7701e0fe24ed70`  
		Last Modified: Sat, 04 Sep 2021 06:16:43 GMT  
		Size: 95.7 MB (95703257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f61de99b7f1e5da0063d2955ec7a01f01d7ed345b8b6dd804aada111402bf9f`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ba76c31dcad016bf941f0e0be2694f0fa339e5c24d7ef5ee4916be74697f0a`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70e46e86bb38bc42f7060c39fbbc233ea20e6f7089b73e2335d3440c1c33d1`  
		Last Modified: Sat, 04 Sep 2021 06:16:18 GMT  
		Size: 3.1 MB (3061914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb99b00b084c4a0e83a272f225159c4cbf6214c81fe2f8571dfaf4276978ce97`  
		Last Modified: Sat, 04 Sep 2021 06:16:25 GMT  
		Size: 44.3 MB (44340016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cbcc1c6467ba9477359f3f850d4c4535ba281eea1e75124bb96d94ba91c2fa`  
		Last Modified: Sat, 04 Sep 2021 06:16:17 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:750c649c6ed54a1bc79c41c44b1bfb009a38e130ca51356a0a5637a77b452f5e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219650978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3733a5127a682e88605681a10a6637a271090e9dddd1ecb6d71d7b4e0b6d2c82`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:34:13 GMT
ADD file:8b9b12a994a2519f725d1ed1f4ab5a444665262678fd8e6c42cf78f32dacb7fa in / 
# Tue, 17 Aug 2021 01:34:20 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 09:32:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 09:32:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 09:32:18 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 09:53:38 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 09:53:41 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 09:53:43 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 10:00:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 10:00:52 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 10:00:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 10:01:01 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 10:01:19 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 10:01:28 GMT
CMD ["irb"]
# Wed, 18 Aug 2021 06:54:16 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 18 Aug 2021 06:59:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 07:00:07 GMT
ENV RAILS_ENV=production
# Wed, 18 Aug 2021 07:00:21 GMT
WORKDIR /usr/src/redmine
# Wed, 18 Aug 2021 07:00:26 GMT
ENV HOME=/home/redmine
# Wed, 18 Aug 2021 07:00:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 Aug 2021 07:00:43 GMT
ENV REDMINE_VERSION=4.2.2
# Wed, 18 Aug 2021 07:00:47 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Wed, 18 Aug 2021 07:01:09 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 Aug 2021 07:07:09 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 Aug 2021 07:07:18 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 Aug 2021 07:07:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 Aug 2021 07:07:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 Aug 2021 07:07:39 GMT
EXPOSE 3000
# Wed, 18 Aug 2021 07:07:49 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c3e09f0e3e7f6fcb741a4c9214b63e341e1d9b53d7689a5ad6ff640b61a82541`  
		Last Modified: Tue, 17 Aug 2021 01:48:22 GMT  
		Size: 30.6 MB (30553721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6540cca707f751654267130c5ff13338c730506cf900ab70cbba8eb8f0774f4`  
		Last Modified: Tue, 17 Aug 2021 10:35:53 GMT  
		Size: 12.7 MB (12704229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5cb3d072ea667e9971932f23c9c5ddffe4a2d7c9a645aa1f53235dc8c2e2ae5`  
		Last Modified: Tue, 17 Aug 2021 10:35:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29445a92f99df6ece2c68fdd21d13b23e28c76507ae5fc4497cbf9272cd41e91`  
		Last Modified: Tue, 17 Aug 2021 10:37:15 GMT  
		Size: 15.0 MB (14997282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee87ac0f307c59470977ad0b974013269088413f9061698138c7f01175ec9982`  
		Last Modified: Tue, 17 Aug 2021 10:37:12 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfb261039caaf3d27ac4757a6a0ca770e695ac15e72cce135badcdf8d17b060`  
		Last Modified: Wed, 18 Aug 2021 07:40:45 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfa4557b0838e19c4cd9f385a4b5ea0972af6fba31e8bcc39e77336887cd48ee`  
		Last Modified: Wed, 18 Aug 2021 07:41:48 GMT  
		Size: 101.3 MB (101328471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5cb4e6a472bc1f6140175c495cf2115da58206520a01bca00638227f2370ea`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c4789be342e86d5f2793092f064c41fde923d87fb85f130d8100b4c88af3474`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2190284052685dcbf10a7e8e39410965a72be33c4c924cedc97130de22e6c8f4`  
		Last Modified: Wed, 18 Aug 2021 07:40:52 GMT  
		Size: 3.1 MB (3061910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b6fa0cc2de623e70d74216ebe78d7dfccc76bda34aae287ec61259ff3f54ce`  
		Last Modified: Wed, 18 Aug 2021 07:41:17 GMT  
		Size: 57.0 MB (57001117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2164f878c998618c80d1e4d55973b954723ba05120f5a4984c112bc210edd8c6`  
		Last Modified: Wed, 18 Aug 2021 07:40:40 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:f764e6f237dd0b4ccc459c4a58872d66f5d9015fa61828ef337cc1aba2dde405
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202557142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:182cde8e814a22a30968ac8996e2499e862f311f0c6cd3a5d1db75334c1b9dce`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Fri, 03 Sep 2021 00:44:44 GMT
ADD file:b8ec865f1745d5948e8a6d734df344bcc6aa076754554241a2d12c6d738199b0 in / 
# Fri, 03 Sep 2021 00:44:47 GMT
CMD ["bash"]
# Fri, 03 Sep 2021 13:10:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 03 Sep 2021 13:10:16 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 03 Sep 2021 13:10:17 GMT
ENV LANG=C.UTF-8
# Fri, 03 Sep 2021 13:38:11 GMT
ENV RUBY_MAJOR=2.7
# Fri, 03 Sep 2021 13:38:11 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 03 Sep 2021 13:38:12 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 03 Sep 2021 13:41:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 03 Sep 2021 13:41:41 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 03 Sep 2021 13:41:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 03 Sep 2021 13:41:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 03 Sep 2021 13:41:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 03 Sep 2021 13:41:45 GMT
CMD ["irb"]
# Sat, 04 Sep 2021 02:39:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Sep 2021 02:40:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Sep 2021 02:40:18 GMT
ENV RAILS_ENV=production
# Sat, 04 Sep 2021 02:40:18 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Sep 2021 02:40:19 GMT
ENV HOME=/home/redmine
# Sat, 04 Sep 2021 02:40:19 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Sep 2021 02:40:19 GMT
ENV REDMINE_VERSION=4.2.2
# Sat, 04 Sep 2021 02:40:19 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Sat, 04 Sep 2021 02:40:23 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Sep 2021 02:42:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Sep 2021 02:42:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Sep 2021 02:42:50 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 04 Sep 2021 02:42:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Sep 2021 02:42:51 GMT
EXPOSE 3000
# Sat, 04 Sep 2021 02:42:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:65229990cda1bd6e6b517c67238f245d103190c9a170014e2c22a40b96dd47ec`  
		Last Modified: Fri, 03 Sep 2021 00:53:39 GMT  
		Size: 25.8 MB (25760757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e55b0a8e76b8c8ba454df09641bdbe40933447efcccf296655a2be3f293524`  
		Last Modified: Fri, 03 Sep 2021 14:13:12 GMT  
		Size: 10.8 MB (10815285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5729b29e02ee2d0574eb5fbd2a208b539cf69fcfc45190860f5ac7d98b04f282`  
		Last Modified: Fri, 03 Sep 2021 14:13:10 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ea6888b61e31cb5b4a8f014006c7cb8fa8a3b7224b7ad3f0b4af257229c789`  
		Last Modified: Fri, 03 Sep 2021 14:14:23 GMT  
		Size: 14.7 MB (14697502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ef0cfb1210ec8b5dff947c27988590a3931cf76a1437a6fe10f30aae9f813`  
		Last Modified: Fri, 03 Sep 2021 14:14:21 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a04f5ff5ec2ee8dd1b21974adff7bf0e6fdb70338e190c6094eed2747ceb117`  
		Last Modified: Sat, 04 Sep 2021 02:50:16 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf9140fc0de2f47daa7719c6c1cbbf193066ad2a67f60c95d78b7baf3626508`  
		Last Modified: Sat, 04 Sep 2021 02:50:29 GMT  
		Size: 91.8 MB (91790843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d640980eb96fb9f7eef22043b3c502898b8cc3f7b1447f1f19055222d3a3bf`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80df1a5482c5309af87986c42c45a6cd4c0cfbce1535792b2c1ba652e2c2a304`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9bc3013aec1061db002a07fa5ae39181287f086837e8c8c53c5814049c837d`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 3.1 MB (3061916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b9caa222bcb2e88202afcfdf166e5a0613fe99bc55cc9b416dda1e1e2484c4`  
		Last Modified: Sat, 04 Sep 2021 02:50:19 GMT  
		Size: 56.4 MB (56426601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff0983c6ea2bc0e811104db8303487a7286daf0ee17c051de72eb5e75dbbc32`  
		Last Modified: Sat, 04 Sep 2021 02:50:15 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:passenger`

```console
$ docker pull redmine@sha256:dc1fa7ae440292befc3702f68fd45e6167a13086847d9c4151f3e7fddab3d679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:1384ea37efaf431cdff585a3d29cc018cacfc671a3c5e723b8f2880fa480659f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221546741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65d69f1c7954cffcb45c23d12731b72e27472b5d6ae629622df20fcda3a4d414`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 17 Aug 2021 01:24:06 GMT
ADD file:87b4e60fe3af680c6815448374365a44e9ea461bc8ade2960b4639c25aed3ba9 in / 
# Tue, 17 Aug 2021 01:24:06 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:21:01 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:21:02 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:23:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:23:44 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:44 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:23:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:23:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:23:47 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 18:01:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 18:01:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 18:01:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 18:01:29 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 18:01:29 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 18:01:30 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 18:01:30 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 18:01:34 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 18:02:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 18:02:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 18:02:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 18:02:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 18:02:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 17 Aug 2021 18:02:25 GMT
ENV PASSENGER_VERSION=6.0.10
# Tue, 17 Aug 2021 18:02:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 18:02:45 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 17 Aug 2021 18:02:45 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 17 Aug 2021 18:02:45 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:e1acddbe380c63f0de4b77d3f287b7c81cd9d89563a230692378126b46ea6546`  
		Last Modified: Tue, 17 Aug 2021 01:30:21 GMT  
		Size: 27.1 MB (27145985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519bcd5a2736ec3ef72e993f0b61da7051957f407d190a0d83f9369d915c4d98`  
		Last Modified: Tue, 17 Aug 2021 04:41:05 GMT  
		Size: 12.6 MB (12562846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119720cd004c3495b5cd6b8883e01df56a3438046b3ecc3198ffb3849f6f25df`  
		Last Modified: Tue, 17 Aug 2021 04:42:13 GMT  
		Size: 14.5 MB (14510198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b764bf01e480a9fff1b3e5a263f7f9f9b4fa77325f616c37cb8e2c81d51e3dd9`  
		Last Modified: Tue, 17 Aug 2021 04:42:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84946f74729ab44aaa49a9af6012e6293fb02521ca05cffaccf128e7b157cec`  
		Last Modified: Tue, 17 Aug 2021 18:09:47 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdcde4d7d6d22355ecf23701bfa1a2abba49bcabfc5f4dd90c746e0143569ba`  
		Last Modified: Tue, 17 Aug 2021 18:10:07 GMT  
		Size: 94.1 MB (94087892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5742225b6ad582633258fcf1e969851dbdd33be3d03cb05cf61b1ea900d8cc`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81933ac92f0a4be0c34689c7c3035c0aa0e4d7e89153bb41cbe0821a1c2a89f7`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb927d9d1176a8bbb1d88d687d964fae4ee7e61ebd08be4d8648f21caa9299e`  
		Last Modified: Tue, 17 Aug 2021 18:09:46 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d25f4984fe7a6089fe506ca06732024aafbfe47de090d95c448ac84b589e573`  
		Last Modified: Tue, 17 Aug 2021 18:09:53 GMT  
		Size: 44.1 MB (44122772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74f790489c8bf8667ba0727c9aa46fb6e9d9128bf89a9c1330b90689f04155bf`  
		Last Modified: Tue, 17 Aug 2021 18:09:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b74d84a329f08033107c147b415d461e38428d975adc347ea34654240ab09e`  
		Last Modified: Tue, 17 Aug 2021 18:10:30 GMT  
		Size: 21.1 MB (21131600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235136ff85630baea96544cddd34b782c51fbd5824839b6264d7ac17db683c0a`  
		Last Modified: Tue, 17 Aug 2021 18:10:27 GMT  
		Size: 4.9 MB (4919283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
