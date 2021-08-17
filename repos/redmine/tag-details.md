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
$ docker pull redmine@sha256:e09ada96ab20fcef1ba9247b23d9c451ef65719d98e25922c2c11226840af94a
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
$ docker pull redmine@sha256:2ba20de8f2d5813171b6b38d1e727aba839ab6cdd974c966ed2b8cd016b97c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196974835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2290c3ececd51c95738415fab07fc46dcc63d3a61e8099fb6c45e290ec3f0d91`
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
# Mon, 02 Aug 2021 20:58:44 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 20:58:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 20:58:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 21:04:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 21:04:31 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 21:04:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 21:04:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:04:32 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 21:04:32 GMT
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
	-	`sha256:7342031318accab10946b43b34804e02f1e0c107a6af3af5a4ebb766152ee509`  
		Last Modified: Mon, 02 Aug 2021 21:11:42 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648b6a3dac4889e5f68f30776a664fe9d62256592f37d6d2912163da56f265fa`  
		Last Modified: Mon, 02 Aug 2021 21:12:04 GMT  
		Size: 55.2 MB (55235555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5a29c2452fcab6625565bca85ff5fccfbee37e09b6f1e8455655c2735c166a`  
		Last Modified: Mon, 02 Aug 2021 21:11:38 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cac694ac7078f02298b587000698d84cb3bb69637d30c724bd0bcac087c22f41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3187fd285a60bd484a8586f3ee1dc8896c0c94e433a102025bf0dae4c344c1b7`
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
# Tue, 03 Aug 2021 00:00:45 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 03 Aug 2021 00:00:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 03 Aug 2021 00:00:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 03 Aug 2021 00:06:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 03 Aug 2021 00:06:06 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 03 Aug 2021 00:06:07 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 03 Aug 2021 00:06:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 03 Aug 2021 00:06:08 GMT
EXPOSE 3000
# Tue, 03 Aug 2021 00:06:08 GMT
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
	-	`sha256:fc2c8055fd9194f59346984cbb7941b37a40023edc25ab3dec3e42e9b8c01287`  
		Last Modified: Tue, 03 Aug 2021 00:12:46 GMT  
		Size: 3.1 MB (3061917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836246f3dcf57e23a39d002b3b9d9a09fedb40b5b6accc7268b28ae167eca128`  
		Last Modified: Tue, 03 Aug 2021 00:13:05 GMT  
		Size: 55.1 MB (55073644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63001a72a77f002e6a9f105ba97f4e5cb147287597ca1e71c8670c6b0e768390`  
		Last Modified: Tue, 03 Aug 2021 00:12:42 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:168d7ed49573c2aaecf2d0d8adcc21280d9e2c18dc1ddb19848393c9847211e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203243298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a980ba1133cf226e557df7c34d75d5c5e7bfb359db4c611a013f2dd737ac6dc4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:20:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:20:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:20:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:20:13 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 14:17:02 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 14:17:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:17:25 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 14:17:26 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 14:17:26 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 14:17:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 14:17:27 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 14:17:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 14:17:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 14:19:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 14:19:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 14:19:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 14:19:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 14:19:48 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 14:19:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ab80b058f00336b15786a8d20ce50706c5277560dc1ddb487b7e5c9d24b10`  
		Last Modified: Tue, 17 Aug 2021 04:34:12 GMT  
		Size: 11.3 MB (11263042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2cb28558c1dd6c31a020484f10c613185335d6d30e7c7a81d3e6ffd0f374f0`  
		Last Modified: Tue, 17 Aug 2021 04:35:35 GMT  
		Size: 14.4 MB (14356587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49391d2e67bfbf4fd993b49c9be1225f0a09d4177c605548f82d49cbcfe78b99`  
		Last Modified: Tue, 17 Aug 2021 04:35:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9307e85455464623a9445ee9314b11fd777c561cefed9b38e6f9067bd30653a`  
		Last Modified: Tue, 17 Aug 2021 14:26:18 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba598bababc240a9c29cf82ac1a0b01837945e37b3cb2b17a3a55ba776227b76`  
		Last Modified: Tue, 17 Aug 2021 14:26:34 GMT  
		Size: 92.6 MB (92611086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dc88258ae8d8cf36219a3b41b130d1e21bf4c2dfb6e1cf9c3f6b3ae2395817`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c9b592ea00c036970d3b4b7baf687de5e9394670884daa30890ab191cfe5bb`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8230053e3f65d96319f5f2351fc906de79749654a83811bf21ea7b34f3bee`  
		Last Modified: Tue, 17 Aug 2021 14:26:17 GMT  
		Size: 3.1 MB (3061920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe117b5c157b62194a629b77cf9c9b15c6821516a74c96470c098adba14546ba`  
		Last Modified: Tue, 17 Aug 2021 14:26:22 GMT  
		Size: 56.0 MB (56031346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9fc675e51cbab5a7a0574bbd10f6ebdc614381aa4a451a98f5884e386b455`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; 386

```console
$ docker pull redmine@sha256:8b2bacb3a529c3a9da30411ee264532f973e5f07226b10f40cca6d31db43a621
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202125065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20cd127add6f4bd712d08c14e2b3a570aa6216ac3e81f7498d128b38ad693d1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:26:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:26:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 07:26:09 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:43:14 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 07:43:14 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 07:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 07:46:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 07:46:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 07:46:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 07:46:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 07:46:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 07:46:43 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 20:44:09 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 20:44:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:44:42 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 20:44:42 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 20:44:42 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 20:44:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 20:44:43 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 20:44:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 20:44:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 20:45:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 20:45:39 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 20:45:39 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 20:45:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 20:45:39 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 20:45:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7c2f28f15bebb2e6e5879bcd2a3c085881fda52f32380a12c8a0248d474ff`  
		Last Modified: Tue, 17 Aug 2021 08:14:57 GMT  
		Size: 17.2 MB (17227368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd3eff60b8a459154279d9ea96f6e521d033e44faf88a091ecf6aef5ebd4888`  
		Last Modified: Tue, 17 Aug 2021 08:14:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d6e92558e2e9952c84a3effe46c647bb2ec5c677559440a30b3472898d5ca2`  
		Last Modified: Tue, 17 Aug 2021 08:16:53 GMT  
		Size: 14.0 MB (13992678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149425e111bee81e3749bcd1a01f973bdea53d5107f36b0ce5ab6f24a5d26bd0`  
		Last Modified: Tue, 17 Aug 2021 08:16:50 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba2aa95ab76e668ab9334a63f10abb5c9cc72b5ce42c0288b8e258d2421de4c`  
		Last Modified: Tue, 17 Aug 2021 20:50:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e3c06b49e4b7fdda9acea36456b2c0c69f0f52f0d50724e55b0f5cdc42ce93`  
		Last Modified: Tue, 17 Aug 2021 20:51:14 GMT  
		Size: 95.7 MB (95702973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d658498d2e116af9d55f933669635cd567034d03d7c862e5be6b2affa43ef371`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d6e976830ca03935c308924157582258b4599ff1a78443efeef21cc6e0c4e5`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db706ca27afe38d047ff274c96b1d95fc75f4512bfd5967afd3854127d17087d`  
		Last Modified: Tue, 17 Aug 2021 20:50:51 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1417c9a42064182a2e270bd603d1fa078906a8999616843228fd988741802494`  
		Last Modified: Tue, 17 Aug 2021 20:50:58 GMT  
		Size: 44.3 MB (44338264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eed6830dcebdb2ec5236d072e5b78c805b2ad7749fa0de197a129adb76a2abf`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; ppc64le

```console
$ docker pull redmine@sha256:ecdb00827fcf83f2f12c122af3ffc2420a6faa270cd7b048c9756f927f7c77fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219650618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57391c1536ff89c22d27544dc68890a924a8d455796c92bdc28721108b71a53c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:33:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 00:33:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 00:52:18 GMT
ENV RUBY_MAJOR=2.7
# Fri, 23 Jul 2021 00:52:28 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 23 Jul 2021 00:52:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 23 Jul 2021 01:01:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 01:01:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 01:01:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 01:01:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 01:01:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 01:01:58 GMT
CMD ["irb"]
# Sat, 24 Jul 2021 02:42:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 24 Jul 2021 02:46:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Jul 2021 02:46:14 GMT
ENV RAILS_ENV=production
# Sat, 24 Jul 2021 02:46:17 GMT
WORKDIR /usr/src/redmine
# Sat, 24 Jul 2021 02:46:19 GMT
ENV HOME=/home/redmine
# Sat, 24 Jul 2021 02:46:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 02 Aug 2021 23:16:59 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 23:17:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 23:17:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 23:23:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 23:23:26 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 23:23:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 23:23:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:23:37 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 23:23:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f17b372a9c9122b881c2d22680e91d78ef4c329094595c61f5acb2523f41b7`  
		Last Modified: Fri, 23 Jul 2021 01:35:00 GMT  
		Size: 12.7 MB (12704330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c16cae6894266abd8c9d33cfb671a4ebb2705d8b8bb7495bafc50c3dcd344`  
		Last Modified: Fri, 23 Jul 2021 01:34:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76d2032e7e646d23109ea1a55abb581c169350b85836914155a6837d64eb757`  
		Last Modified: Fri, 23 Jul 2021 01:36:48 GMT  
		Size: 15.0 MB (14997545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f996a3088f8cd5e20b9f19c3aebdd4a6228a85b6c0a83f9dde8e2a5ec82976d3`  
		Last Modified: Fri, 23 Jul 2021 01:36:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acdc172d0fc27092df5794b7a17e2c42e7f2497e85086076f490e273db428fe`  
		Last Modified: Sat, 24 Jul 2021 03:36:05 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe4ded3f0db610cc9dca87e98b2305c850cbaf595886ccb44e3492ad727b18`  
		Last Modified: Sat, 24 Jul 2021 03:36:28 GMT  
		Size: 101.3 MB (101327533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14617640fcda340a6bc04fd1c65d4183ad0dd01a4e3b44fb313d164071471e95`  
		Last Modified: Sat, 24 Jul 2021 03:36:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1b361a5633d0ca044cc644bddc99329645edadfff1cbb48e966deb9b0d079a`  
		Last Modified: Sat, 24 Jul 2021 03:36:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bfbd857622d0239bfa521d75318f40925e9e4608a62a4be7abc2bc89801ec3`  
		Last Modified: Mon, 02 Aug 2021 23:30:32 GMT  
		Size: 3.1 MB (3061921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4b836dd92fc0980e6e61a697cc881ceb76ca811af742788283ab3211698e1`  
		Last Modified: Mon, 02 Aug 2021 23:30:38 GMT  
		Size: 57.0 MB (57001331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2976222796409af9d080f03664b07bc2a177c8b37d29e7937c0620ba5f908d03`  
		Last Modified: Mon, 02 Aug 2021 23:30:31 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4` - linux; s390x

```console
$ docker pull redmine@sha256:33d5a2369e443a1bb092e9da696586fae6988113fc4ef99bf98b5af5e03135f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202554693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f13509159fb8e3ef52d7620d4ef325ebe2d7a388fec2faf172536b64ee9ae9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:21:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:21:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:37:51 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:37:51 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:37:52 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:40:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:40:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:40:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:40:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:40:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:40:24 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 13:32:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 13:33:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:33:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 13:33:28 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 13:33:28 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 13:33:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 13:33:29 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 13:33:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 13:33:32 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 13:35:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:35:38 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 13:35:38 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 13:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 13:35:39 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 13:35:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c03f413a15f7a98caaa2b027613636c576e3d98d8e1a98805c5978f2cc985f`  
		Last Modified: Tue, 17 Aug 2021 05:03:55 GMT  
		Size: 10.8 MB (10814401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ded0951dc51ddc1b38edf558277fec87d4169c1607312f67af2c4ffb9c4f19`  
		Last Modified: Tue, 17 Aug 2021 05:03:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d49ef1e1c8f0247bfa63924e738fc94dc0c4a81ec0e4b2b73df09f08d080005`  
		Last Modified: Tue, 17 Aug 2021 05:04:49 GMT  
		Size: 14.7 MB (14697415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54919ecbd2a42d851761e24bb9a1e9e71346c6ecd753a4c6b7868679823367b`  
		Last Modified: Tue, 17 Aug 2021 05:04:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159f1e20f87d626bb303eea037968c316700fdd1fd9fa734e8ebacf14608ab2`  
		Last Modified: Tue, 17 Aug 2021 13:42:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223675cd45b3e6a43e45f6ad1a699c278dc5effe72583bec3657746c84a2a692`  
		Last Modified: Tue, 17 Aug 2021 13:42:24 GMT  
		Size: 91.8 MB (91792621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e74adea5c6a7d4c0be869fe00b2451a51e188e2c0e1466d72eaad06cc9d`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cd2e454b71a3aea72543018a9596e611b94ee88301b3d5971854daab02981`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885ccd7ef756fbf397809a3541c6cadba886972a35c3f9d9d00cc920b16ef2`  
		Last Modified: Tue, 17 Aug 2021 13:42:11 GMT  
		Size: 3.1 MB (3061920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde4808141553382cd3c73078af6ba86889e806ed72c6251287678fbce48b5ea`  
		Last Modified: Tue, 17 Aug 2021 13:42:15 GMT  
		Size: 56.4 MB (56423232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed18e7c147f9b19d7cb774a6462749d36a61882e80d34fff6912e4ed7990252d`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4-alpine`

```console
$ docker pull redmine@sha256:34362d64f5cac220ecf3058a2982583ec0e2cba35273960105a4cff3dc0c4a5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:429416f2012459eaa042fe2879ae170f0d1ee68b283059b2e4f855edcaae0101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150082289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a3f4194f1bef28b7e8c9cb584331cfe9876976fd1c68e194837191b82282e8`
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
# Mon, 02 Aug 2021 19:27:15 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 19:27:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 19:27:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 19:27:19 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 02 Aug 2021 19:29:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 02 Aug 2021 19:29:21 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 19:29:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 02 Aug 2021 19:29:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 19:29:22 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 19:29:22 GMT
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
	-	`sha256:e98c03ed41f8aa891bcd79e61fbb88cda198d71f5a8de4f510950e7f58aa1a15`  
		Last Modified: Mon, 02 Aug 2021 19:34:04 GMT  
		Size: 3.1 MB (3062843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08d14dd9ea01201645da35bc3855c4b0a6270b9d4ae9510f9da35fb4150e833`  
		Last Modified: Mon, 02 Aug 2021 19:34:08 GMT  
		Size: 56.7 MB (56722754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bee94fd486f4fb693e4765ade966dd49ee96cd0aff32109f156b9a2511d1af3`  
		Last Modified: Mon, 02 Aug 2021 19:34:03 GMT  
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
$ docker pull redmine@sha256:523dbe7c2377f1ddde372bd9cc238803cbe0ed1b03e2380d8a2f6169ac1be595
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
$ docker pull redmine@sha256:b88759af15842d0592a9ea5f67a803fd6ac33252a035ab554e88098f02574b52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200850483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43460e0a84b844270c94cae84bf674b95dd7fc307754fe931011e927e98abd47`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:25:18 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:25:19 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:25:19 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:27:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:27:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:27:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:27:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:27:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:27:26 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 14:19:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 14:23:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:23:16 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 14:23:16 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 14:23:16 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 14:23:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 14:23:17 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 14:23:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 14:23:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 14:25:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 14:25:43 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 14:25:43 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 14:25:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 14:25:44 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 14:25:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ab80b058f00336b15786a8d20ce50706c5277560dc1ddb487b7e5c9d24b10`  
		Last Modified: Tue, 17 Aug 2021 04:34:12 GMT  
		Size: 11.3 MB (11263042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a741dfbe27573196b9f78f97eb7f35b06eaff990866fb7f894987974bd3f6d`  
		Last Modified: Tue, 17 Aug 2021 04:36:41 GMT  
		Size: 21.3 MB (21309045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991754b0a79718bf8ab6c058b0ca4e091450b59072ac29e34401525b4337cc2`  
		Last Modified: Tue, 17 Aug 2021 04:36:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b2d6fcce3e7c045cbcf366963f15eecf60f206a0f9affdb4be5f3e1cdb8e58`  
		Last Modified: Tue, 17 Aug 2021 14:26:56 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39391463d0169869babe67051e72a4badb5e6538463aa13476d59709b2d1627a`  
		Last Modified: Tue, 17 Aug 2021 14:27:39 GMT  
		Size: 79.7 MB (79749184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bd4702d9b260665631a6e852231aba7fd3ba3322e443a969edb1d5f08f7196`  
		Last Modified: Tue, 17 Aug 2021 14:27:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93416b8e64e921655341d941d209345e030b91a533d8ffb233ece46312f04886`  
		Last Modified: Tue, 17 Aug 2021 14:27:24 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a29700d7f8864656fe98ec815952adea82a0cc692c4d47e68902625234b455f`  
		Last Modified: Tue, 17 Aug 2021 14:27:25 GMT  
		Size: 2.5 MB (2542545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb789346c1b22068ac9ec84aa33e715bb1529ef95da7ab381f8775aadeb83ff`  
		Last Modified: Tue, 17 Aug 2021 14:27:32 GMT  
		Size: 60.1 MB (60067351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd11b2bf406e2bdcdb6a7e80ab2722c7b56c44677f10548b9d342d2c88669302`  
		Last Modified: Tue, 17 Aug 2021 14:27:24 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; 386

```console
$ docker pull redmine@sha256:8c83d6bd8cfe0be39ef2e2a9dd50ae0e619f1542fa8c6ae5a2a94e4603d111f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210333363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75899d8b07373e9e067086f942d862750a196223f78a23d19ccfe63e36e6306`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:26:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:26:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 07:26:09 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:59:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 07:59:10 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 07:59:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 08:03:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 08:03:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 08:03:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 08:03:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 08:03:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 08:03:22 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 20:45:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 20:47:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:47:58 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 20:47:59 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 20:47:59 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 20:48:00 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 20:48:00 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 20:48:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 20:48:05 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 20:50:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 20:50:17 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 20:50:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 20:50:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 20:50:18 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 20:50:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7c2f28f15bebb2e6e5879bcd2a3c085881fda52f32380a12c8a0248d474ff`  
		Last Modified: Tue, 17 Aug 2021 08:14:57 GMT  
		Size: 17.2 MB (17227368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd3eff60b8a459154279d9ea96f6e521d033e44faf88a091ecf6aef5ebd4888`  
		Last Modified: Tue, 17 Aug 2021 08:14:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abeae1db7691d99592122ca161df7a8e8cbfedddac486774e69cf9accd392d7`  
		Last Modified: Tue, 17 Aug 2021 08:18:31 GMT  
		Size: 20.9 MB (20910066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22694e209a608abf489b2dfa2c8d19ad0b9b4aef685bdd0e434f84177151f294`  
		Last Modified: Tue, 17 Aug 2021 08:18:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02bf98207b296a2375e26993ab2fcdc880bece959660400f358e1406d008cb5`  
		Last Modified: Tue, 17 Aug 2021 20:51:37 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e6bcb07e3ffd3b72e7aab32366362451af02c519f0407b9b9fec93778f08bc`  
		Last Modified: Tue, 17 Aug 2021 20:52:32 GMT  
		Size: 82.6 MB (82599581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85f95ba4350c7eec72c4702fea439d12cc72409bb1e0fe4480174f46a84384`  
		Last Modified: Tue, 17 Aug 2021 20:52:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cb8e2111c230f411d5ec1adab33ac2dbd29a73e40944b15c0636f0e7f55e42`  
		Last Modified: Tue, 17 Aug 2021 20:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7612204977ea1b0d80a47f652eec00a30f11c670955d73bdd0fbdb819ba6da42`  
		Last Modified: Tue, 17 Aug 2021 20:52:11 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0379a97522d76f257cdbc5c4daae2e5df37bcf297e0cfa2dcab80b87a644a26c`  
		Last Modified: Tue, 17 Aug 2021 20:52:20 GMT  
		Size: 59.3 MB (59251943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb29324642ef7593e8f165e527bd0c4a6f4060ef4797fbfa86113d53024fca9`  
		Last Modified: Tue, 17 Aug 2021 20:52:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; ppc64le

```console
$ docker pull redmine@sha256:f66f4634bf1585887b6cadeb8646989343e1ee4c44a136cd20edbe611d29e44d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216453624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9be8237ffe8a0fb25d3069a58c72db83381976bcc3b21b0c9815de1b8edca92`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:33:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 00:33:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 01:11:31 GMT
ENV RUBY_MAJOR=2.6
# Fri, 23 Jul 2021 01:11:38 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 23 Jul 2021 01:11:44 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 23 Jul 2021 01:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 01:26:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 01:26:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 01:26:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 01:26:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 01:26:59 GMT
CMD ["irb"]
# Sat, 24 Jul 2021 02:51:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 24 Jul 2021 03:14:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Jul 2021 03:14:23 GMT
ENV RAILS_ENV=production
# Sat, 24 Jul 2021 03:14:25 GMT
WORKDIR /usr/src/redmine
# Sat, 24 Jul 2021 03:14:30 GMT
ENV HOME=/home/redmine
# Sat, 24 Jul 2021 03:14:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 24 Jul 2021 03:14:46 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 24 Jul 2021 03:14:52 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 24 Jul 2021 03:15:07 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 24 Jul 2021 03:35:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 24 Jul 2021 03:35:13 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 24 Jul 2021 03:35:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 24 Jul 2021 03:35:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 24 Jul 2021 03:35:27 GMT
EXPOSE 3000
# Sat, 24 Jul 2021 03:35:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f17b372a9c9122b881c2d22680e91d78ef4c329094595c61f5acb2523f41b7`  
		Last Modified: Fri, 23 Jul 2021 01:35:00 GMT  
		Size: 12.7 MB (12704330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c16cae6894266abd8c9d33cfb671a4ebb2705d8b8bb7495bafc50c3dcd344`  
		Last Modified: Fri, 23 Jul 2021 01:34:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33960675014a7e56a0cf9f85e256ec6cce1c710723a7cd8f64935709d00e323d`  
		Last Modified: Fri, 23 Jul 2021 01:38:17 GMT  
		Size: 22.0 MB (21985713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047ee7c416fdfdb76a18bc7d50d5c00c1568b5e197242760391ce18bec14da13`  
		Last Modified: Fri, 23 Jul 2021 01:38:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c93f3da9b7a0eaf5df16b7b32a686296eaa146856420c2ce2d9ee2ad916121`  
		Last Modified: Sat, 24 Jul 2021 03:36:52 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf10994c116f970b482c990a6b89a17d4292257aa8d4c8f112785b16d9683b77`  
		Last Modified: Sat, 24 Jul 2021 03:37:45 GMT  
		Size: 87.9 MB (87901004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc18e39a895f554cc9e72fb3f4f8fd6e3f14b8ba82bd4e555e33eab6e1e53c`  
		Last Modified: Sat, 24 Jul 2021 03:37:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e987abb4c826ab5b57ae49bcd75a9f15613c83d87e0677a62c4a11a1e60997`  
		Last Modified: Sat, 24 Jul 2021 03:37:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70618bee2d6cbdd87a9143949d8b3b252e21aa336af80a651853bfeac299ccb1`  
		Last Modified: Sat, 24 Jul 2021 03:37:26 GMT  
		Size: 2.5 MB (2542542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a66220dec1e7b2bd2bdba148f204920c16e19c11be7ac1000b3a337d3b3f0b`  
		Last Modified: Sat, 24 Jul 2021 03:37:35 GMT  
		Size: 60.8 MB (60762081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2192580103ba2e9b41655dfdbd0ed3800350febf95cbdba890bb38b2f9d12bc0`  
		Last Modified: Sat, 24 Jul 2021 03:37:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0` - linux; s390x

```console
$ docker pull redmine@sha256:d328d900e9b6cb797ed448f67b29841ed5cf8a4c3832bba7fc865e60bd8eaacb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200270811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c1f10c0616a1c38940f42bed4e642ccdd9226b8d89fc62b6e3e4dabcc41355e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:21:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:21:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:54:27 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:54:28 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:54:29 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:57:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:57:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:57:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:57:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:57:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:57:43 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 13:35:57 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 13:38:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:39:00 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 13:39:01 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 13:39:01 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 13:39:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 13:39:03 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 13:39:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 13:39:07 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 13:41:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:41:36 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 13:41:36 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 13:41:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 13:41:36 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 13:41:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c03f413a15f7a98caaa2b027613636c576e3d98d8e1a98805c5978f2cc985f`  
		Last Modified: Tue, 17 Aug 2021 05:03:55 GMT  
		Size: 10.8 MB (10814401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ded0951dc51ddc1b38edf558277fec87d4169c1607312f67af2c4ffb9c4f19`  
		Last Modified: Tue, 17 Aug 2021 05:03:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b5f065983b815df03f5d378b737ce8b8950a6f775907f64c8d9413edfec507`  
		Last Modified: Tue, 17 Aug 2021 05:05:31 GMT  
		Size: 21.6 MB (21620194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c23b68c30a72cdc95043eff33b8ac51682c16759a2f483c8f4255db0f287c2`  
		Last Modified: Tue, 17 Aug 2021 05:05:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04534d357d558a08a4aea1da302e17954529ebf3804b4a0fe94cff2edac70b48`  
		Last Modified: Tue, 17 Aug 2021 13:42:39 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218be0290ec79b3f04e7f77dfe8f8ac8cbd9201826ad01308fcbadb25a5e6a77`  
		Last Modified: Tue, 17 Aug 2021 13:43:11 GMT  
		Size: 78.9 MB (78942684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fac95700e00653babfdc8d8adf7f68e3bad29e80fa48749640f683e194389`  
		Last Modified: Tue, 17 Aug 2021 13:43:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ced46f2f9e40ad3ad2fbf664f2e2e2602d4d28bfe90a309a0f825cf0fca8b5`  
		Last Modified: Tue, 17 Aug 2021 13:43:00 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f2b73b065f8dcb4e9e6dffcbe73867f941480ca0a5d80811e345039ff4105e`  
		Last Modified: Tue, 17 Aug 2021 13:43:00 GMT  
		Size: 2.5 MB (2542549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28def5e72cbe09aa3df74f8671867014e00dbab04acaaf0216d648662c3ced87`  
		Last Modified: Tue, 17 Aug 2021 13:43:06 GMT  
		Size: 60.6 MB (60585884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902db45741704beb098e03501c7e36acd54a48c9891229a213037876e70978d7`  
		Last Modified: Tue, 17 Aug 2021 13:42:59 GMT  
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
$ docker pull redmine@sha256:523dbe7c2377f1ddde372bd9cc238803cbe0ed1b03e2380d8a2f6169ac1be595
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
$ docker pull redmine@sha256:b88759af15842d0592a9ea5f67a803fd6ac33252a035ab554e88098f02574b52
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.9 MB (200850483 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43460e0a84b844270c94cae84bf674b95dd7fc307754fe931011e927e98abd47`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:25:18 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:25:19 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:25:19 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:27:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:27:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:27:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:27:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:27:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:27:26 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 14:19:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 14:23:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:23:16 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 14:23:16 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 14:23:16 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 14:23:17 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 14:23:17 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 14:23:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 14:23:26 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 14:25:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 14:25:43 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 14:25:43 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 14:25:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 14:25:44 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 14:25:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ab80b058f00336b15786a8d20ce50706c5277560dc1ddb487b7e5c9d24b10`  
		Last Modified: Tue, 17 Aug 2021 04:34:12 GMT  
		Size: 11.3 MB (11263042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a741dfbe27573196b9f78f97eb7f35b06eaff990866fb7f894987974bd3f6d`  
		Last Modified: Tue, 17 Aug 2021 04:36:41 GMT  
		Size: 21.3 MB (21309045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991754b0a79718bf8ab6c058b0ca4e091450b59072ac29e34401525b4337cc2`  
		Last Modified: Tue, 17 Aug 2021 04:36:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b2d6fcce3e7c045cbcf366963f15eecf60f206a0f9affdb4be5f3e1cdb8e58`  
		Last Modified: Tue, 17 Aug 2021 14:26:56 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39391463d0169869babe67051e72a4badb5e6538463aa13476d59709b2d1627a`  
		Last Modified: Tue, 17 Aug 2021 14:27:39 GMT  
		Size: 79.7 MB (79749184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76bd4702d9b260665631a6e852231aba7fd3ba3322e443a969edb1d5f08f7196`  
		Last Modified: Tue, 17 Aug 2021 14:27:24 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93416b8e64e921655341d941d209345e030b91a533d8ffb233ece46312f04886`  
		Last Modified: Tue, 17 Aug 2021 14:27:24 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a29700d7f8864656fe98ec815952adea82a0cc692c4d47e68902625234b455f`  
		Last Modified: Tue, 17 Aug 2021 14:27:25 GMT  
		Size: 2.5 MB (2542545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb789346c1b22068ac9ec84aa33e715bb1529ef95da7ab381f8775aadeb83ff`  
		Last Modified: Tue, 17 Aug 2021 14:27:32 GMT  
		Size: 60.1 MB (60067351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd11b2bf406e2bdcdb6a7e80ab2722c7b56c44677f10548b9d342d2c88669302`  
		Last Modified: Tue, 17 Aug 2021 14:27:24 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; 386

```console
$ docker pull redmine@sha256:8c83d6bd8cfe0be39ef2e2a9dd50ae0e619f1542fa8c6ae5a2a94e4603d111f3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.3 MB (210333363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75899d8b07373e9e067086f942d862750a196223f78a23d19ccfe63e36e6306`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:26:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:26:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 07:26:09 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:59:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 07:59:10 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 07:59:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 08:03:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 08:03:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 08:03:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 08:03:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 08:03:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 08:03:22 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 20:45:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 20:47:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:47:58 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 20:47:59 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 20:47:59 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 20:48:00 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 20:48:00 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 20:48:00 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 20:48:05 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 20:50:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 20:50:17 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 20:50:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 20:50:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 20:50:18 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 20:50:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7c2f28f15bebb2e6e5879bcd2a3c085881fda52f32380a12c8a0248d474ff`  
		Last Modified: Tue, 17 Aug 2021 08:14:57 GMT  
		Size: 17.2 MB (17227368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd3eff60b8a459154279d9ea96f6e521d033e44faf88a091ecf6aef5ebd4888`  
		Last Modified: Tue, 17 Aug 2021 08:14:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abeae1db7691d99592122ca161df7a8e8cbfedddac486774e69cf9accd392d7`  
		Last Modified: Tue, 17 Aug 2021 08:18:31 GMT  
		Size: 20.9 MB (20910066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22694e209a608abf489b2dfa2c8d19ad0b9b4aef685bdd0e434f84177151f294`  
		Last Modified: Tue, 17 Aug 2021 08:18:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02bf98207b296a2375e26993ab2fcdc880bece959660400f358e1406d008cb5`  
		Last Modified: Tue, 17 Aug 2021 20:51:37 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e6bcb07e3ffd3b72e7aab32366362451af02c519f0407b9b9fec93778f08bc`  
		Last Modified: Tue, 17 Aug 2021 20:52:32 GMT  
		Size: 82.6 MB (82599581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca85f95ba4350c7eec72c4702fea439d12cc72409bb1e0fe4480174f46a84384`  
		Last Modified: Tue, 17 Aug 2021 20:52:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cb8e2111c230f411d5ec1adab33ac2dbd29a73e40944b15c0636f0e7f55e42`  
		Last Modified: Tue, 17 Aug 2021 20:52:10 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7612204977ea1b0d80a47f652eec00a30f11c670955d73bdd0fbdb819ba6da42`  
		Last Modified: Tue, 17 Aug 2021 20:52:11 GMT  
		Size: 2.5 MB (2542543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0379a97522d76f257cdbc5c4daae2e5df37bcf297e0cfa2dcab80b87a644a26c`  
		Last Modified: Tue, 17 Aug 2021 20:52:20 GMT  
		Size: 59.3 MB (59251943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb29324642ef7593e8f165e527bd0c4a6f4060ef4797fbfa86113d53024fca9`  
		Last Modified: Tue, 17 Aug 2021 20:52:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; ppc64le

```console
$ docker pull redmine@sha256:f66f4634bf1585887b6cadeb8646989343e1ee4c44a136cd20edbe611d29e44d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.5 MB (216453624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9be8237ffe8a0fb25d3069a58c72db83381976bcc3b21b0c9815de1b8edca92`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:33:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 00:33:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 01:11:31 GMT
ENV RUBY_MAJOR=2.6
# Fri, 23 Jul 2021 01:11:38 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 23 Jul 2021 01:11:44 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 23 Jul 2021 01:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 01:26:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 01:26:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 01:26:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 01:26:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 01:26:59 GMT
CMD ["irb"]
# Sat, 24 Jul 2021 02:51:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 24 Jul 2021 03:14:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Jul 2021 03:14:23 GMT
ENV RAILS_ENV=production
# Sat, 24 Jul 2021 03:14:25 GMT
WORKDIR /usr/src/redmine
# Sat, 24 Jul 2021 03:14:30 GMT
ENV HOME=/home/redmine
# Sat, 24 Jul 2021 03:14:38 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 24 Jul 2021 03:14:46 GMT
ENV REDMINE_VERSION=4.0.9
# Sat, 24 Jul 2021 03:14:52 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Sat, 24 Jul 2021 03:15:07 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 24 Jul 2021 03:35:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 24 Jul 2021 03:35:13 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 24 Jul 2021 03:35:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sat, 24 Jul 2021 03:35:23 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 24 Jul 2021 03:35:27 GMT
EXPOSE 3000
# Sat, 24 Jul 2021 03:35:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f17b372a9c9122b881c2d22680e91d78ef4c329094595c61f5acb2523f41b7`  
		Last Modified: Fri, 23 Jul 2021 01:35:00 GMT  
		Size: 12.7 MB (12704330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c16cae6894266abd8c9d33cfb671a4ebb2705d8b8bb7495bafc50c3dcd344`  
		Last Modified: Fri, 23 Jul 2021 01:34:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33960675014a7e56a0cf9f85e256ec6cce1c710723a7cd8f64935709d00e323d`  
		Last Modified: Fri, 23 Jul 2021 01:38:17 GMT  
		Size: 22.0 MB (21985713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047ee7c416fdfdb76a18bc7d50d5c00c1568b5e197242760391ce18bec14da13`  
		Last Modified: Fri, 23 Jul 2021 01:38:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c93f3da9b7a0eaf5df16b7b32a686296eaa146856420c2ce2d9ee2ad916121`  
		Last Modified: Sat, 24 Jul 2021 03:36:52 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf10994c116f970b482c990a6b89a17d4292257aa8d4c8f112785b16d9683b77`  
		Last Modified: Sat, 24 Jul 2021 03:37:45 GMT  
		Size: 87.9 MB (87901004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbc18e39a895f554cc9e72fb3f4f8fd6e3f14b8ba82bd4e555e33eab6e1e53c`  
		Last Modified: Sat, 24 Jul 2021 03:37:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e987abb4c826ab5b57ae49bcd75a9f15613c83d87e0677a62c4a11a1e60997`  
		Last Modified: Sat, 24 Jul 2021 03:37:25 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70618bee2d6cbdd87a9143949d8b3b252e21aa336af80a651853bfeac299ccb1`  
		Last Modified: Sat, 24 Jul 2021 03:37:26 GMT  
		Size: 2.5 MB (2542542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a66220dec1e7b2bd2bdba148f204920c16e19c11be7ac1000b3a337d3b3f0b`  
		Last Modified: Sat, 24 Jul 2021 03:37:35 GMT  
		Size: 60.8 MB (60762081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2192580103ba2e9b41655dfdbd0ed3800350febf95cbdba890bb38b2f9d12bc0`  
		Last Modified: Sat, 24 Jul 2021 03:37:25 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.0.9` - linux; s390x

```console
$ docker pull redmine@sha256:d328d900e9b6cb797ed448f67b29841ed5cf8a4c3832bba7fc865e60bd8eaacb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.3 MB (200270811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c1f10c0616a1c38940f42bed4e642ccdd9226b8d89fc62b6e3e4dabcc41355e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:21:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:21:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:54:27 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:54:28 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:54:29 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:57:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:57:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:57:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:57:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:57:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:57:43 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 13:35:57 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 13:38:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 		gosu 		tini 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:39:00 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 13:39:01 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 13:39:01 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 13:39:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 13:39:03 GMT
ENV REDMINE_VERSION=4.0.9
# Tue, 17 Aug 2021 13:39:03 GMT
ENV REDMINE_DOWNLOAD_SHA256=04a772b0b8f8ce6493614a7cb22ed82cb9b43c75dcdbeb5c2f925bae98e0d5df
# Tue, 17 Aug 2021 13:39:07 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 13:41:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 		libmagickcore-dev libmagickwand-dev 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:41:36 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 13:41:36 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 13:41:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 13:41:36 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 13:41:37 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c03f413a15f7a98caaa2b027613636c576e3d98d8e1a98805c5978f2cc985f`  
		Last Modified: Tue, 17 Aug 2021 05:03:55 GMT  
		Size: 10.8 MB (10814401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ded0951dc51ddc1b38edf558277fec87d4169c1607312f67af2c4ffb9c4f19`  
		Last Modified: Tue, 17 Aug 2021 05:03:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b5f065983b815df03f5d378b737ce8b8950a6f775907f64c8d9413edfec507`  
		Last Modified: Tue, 17 Aug 2021 05:05:31 GMT  
		Size: 21.6 MB (21620194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c23b68c30a72cdc95043eff33b8ac51682c16759a2f483c8f4255db0f287c2`  
		Last Modified: Tue, 17 Aug 2021 05:05:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04534d357d558a08a4aea1da302e17954529ebf3804b4a0fe94cff2edac70b48`  
		Last Modified: Tue, 17 Aug 2021 13:42:39 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218be0290ec79b3f04e7f77dfe8f8ac8cbd9201826ad01308fcbadb25a5e6a77`  
		Last Modified: Tue, 17 Aug 2021 13:43:11 GMT  
		Size: 78.9 MB (78942684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb2fac95700e00653babfdc8d8adf7f68e3bad29e80fa48749640f683e194389`  
		Last Modified: Tue, 17 Aug 2021 13:43:00 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ced46f2f9e40ad3ad2fbf664f2e2e2602d4d28bfe90a309a0f825cf0fca8b5`  
		Last Modified: Tue, 17 Aug 2021 13:43:00 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f2b73b065f8dcb4e9e6dffcbe73867f941480ca0a5d80811e345039ff4105e`  
		Last Modified: Tue, 17 Aug 2021 13:43:00 GMT  
		Size: 2.5 MB (2542549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28def5e72cbe09aa3df74f8671867014e00dbab04acaaf0216d648662c3ced87`  
		Last Modified: Tue, 17 Aug 2021 13:43:06 GMT  
		Size: 60.6 MB (60585884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902db45741704beb098e03501c7e36acd54a48c9891229a213037876e70978d7`  
		Last Modified: Tue, 17 Aug 2021 13:42:59 GMT  
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
$ docker pull redmine@sha256:29ffe9263d1106c9e1dc2c854516bd360c926e8644652f2c04b7125a8cd8ad1e
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
$ docker pull redmine@sha256:4bdd1675075975131a250540a53f8880f1e0fae8b29cfbc67ddab10f6586177b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210666390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfcbb5833331e6445ac71ddc434c6a915315e32f215e0d6bc5929c81cd521053`
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
# Mon, 02 Aug 2021 21:04:50 GMT
ENV REDMINE_VERSION=4.1.4
# Mon, 02 Aug 2021 21:04:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Mon, 02 Aug 2021 21:04:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 21:10:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 21:10:36 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 21:10:37 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 21:10:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:10:38 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 21:10:38 GMT
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
	-	`sha256:a5f864c8ca3715d87914498c4905365f0ed5cbf5e0cb26b9c639534a5511833b`  
		Last Modified: Mon, 02 Aug 2021 21:12:29 GMT  
		Size: 2.7 MB (2749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4019d3cb4be9309f4cb0baa969bf37dfa6c525ade166c631d7b406cd8a3e59e4`  
		Last Modified: Mon, 02 Aug 2021 21:12:55 GMT  
		Size: 62.4 MB (62378250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2b0e0b86ccd1d38a66825b3d86b65542b19b9b749dd197dcf78fa771f039`  
		Last Modified: Mon, 02 Aug 2021 21:12:26 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm variant v7

```console
$ docker pull redmine@sha256:be260e0859e1639be25cf06cbe19352b4fb385c4942632e35f1558ddda888805
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203843857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f5b264322abd1cb8a7edae6550cf4a9952aa25db98c9a76125dd5ca9d1a94a`
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
# Tue, 03 Aug 2021 00:06:22 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 03 Aug 2021 00:06:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 03 Aug 2021 00:06:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 03 Aug 2021 00:11:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 03 Aug 2021 00:11:46 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 03 Aug 2021 00:11:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 03 Aug 2021 00:11:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 03 Aug 2021 00:11:48 GMT
EXPOSE 3000
# Tue, 03 Aug 2021 00:11:48 GMT
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
	-	`sha256:c129690336fa4b91fdd3354d450f70c1d503241b4f996e45a06f6cc7c5c33c8e`  
		Last Modified: Tue, 03 Aug 2021 00:13:31 GMT  
		Size: 2.7 MB (2749050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fe83cafb9bc610bb800a4c85956caaac9219e0f8a9d3c4c4951568fbaf45a4`  
		Last Modified: Tue, 03 Aug 2021 00:13:56 GMT  
		Size: 62.2 MB (62238188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8821dd99090d5f0c3476a0eabbcb4ec9b51cd0954272e8f5443c04ab694180f`  
		Last Modified: Tue, 03 Aug 2021 00:13:27 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:4d2eef074194f45decdf5b1b4a3166169b18038058b325f0d0862dbf58e89de1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217544129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f43f88150f3bd00e9b27ca2fb50ae014489a41818c5674b2166dabae0c267a69`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:25:18 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:25:19 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:25:19 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:27:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:27:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:27:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:27:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:27:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:27:26 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 14:19:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 14:20:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:20:21 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 14:20:21 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 14:20:21 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 14:20:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 14:20:22 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 14:20:22 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 14:20:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 14:22:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 14:22:50 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 14:22:50 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 14:22:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 14:22:50 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 14:22:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ab80b058f00336b15786a8d20ce50706c5277560dc1ddb487b7e5c9d24b10`  
		Last Modified: Tue, 17 Aug 2021 04:34:12 GMT  
		Size: 11.3 MB (11263042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a741dfbe27573196b9f78f97eb7f35b06eaff990866fb7f894987974bd3f6d`  
		Last Modified: Tue, 17 Aug 2021 04:36:41 GMT  
		Size: 21.3 MB (21309045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991754b0a79718bf8ab6c058b0ca4e091450b59072ac29e34401525b4337cc2`  
		Last Modified: Tue, 17 Aug 2021 04:36:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b2d6fcce3e7c045cbcf366963f15eecf60f206a0f9affdb4be5f3e1cdb8e58`  
		Last Modified: Tue, 17 Aug 2021 14:26:56 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fb70beab3eb9f346f19baeada6ab2ab16b85603c8269cd25ef07d34d7d3bbd`  
		Last Modified: Tue, 17 Aug 2021 14:27:12 GMT  
		Size: 92.6 MB (92610850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88949e39e9bf16adf106d42b5c92a9aa9f223ed09de640620dab986a37998467`  
		Last Modified: Tue, 17 Aug 2021 14:26:54 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8b01342158e6f70c8d6a1fb0a08d898843a76e9eaac116f8be7bf1cd5dc0ab`  
		Last Modified: Tue, 17 Aug 2021 14:26:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a92eed4532a610d931b5637079bd2beaf67787995446f363d81a4e9afb7304c`  
		Last Modified: Tue, 17 Aug 2021 14:26:55 GMT  
		Size: 2.7 MB (2749057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4658a1e88f9cf77366e04fc9ccacb6815390e8e23e32ba77a0e63a1307a797d5`  
		Last Modified: Tue, 17 Aug 2021 14:27:02 GMT  
		Size: 63.7 MB (63692816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd3201c15e0230dd813392cedf5401f39cafe6d75e2649301390105577ef545`  
		Last Modified: Tue, 17 Aug 2021 14:26:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; 386

```console
$ docker pull redmine@sha256:83a453ae4bbf1d595a804d4917f72203fe31ec05b31aabf7000f4944077d6f99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213004573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9d2327537f88c856b9493b788df02f70b77b9bd5ae85a1de424a2bebe50008b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:26:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:26:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 07:26:09 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:59:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 07:59:10 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 07:59:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 08:03:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 08:03:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 08:03:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 08:03:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 08:03:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 08:03:22 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 20:45:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 20:46:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:20 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 20:46:21 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 20:46:21 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 20:46:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 20:46:22 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 20:46:22 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 20:46:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 20:47:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 20:47:17 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 20:47:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 20:47:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 20:47:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 20:47:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7c2f28f15bebb2e6e5879bcd2a3c085881fda52f32380a12c8a0248d474ff`  
		Last Modified: Tue, 17 Aug 2021 08:14:57 GMT  
		Size: 17.2 MB (17227368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd3eff60b8a459154279d9ea96f6e521d033e44faf88a091ecf6aef5ebd4888`  
		Last Modified: Tue, 17 Aug 2021 08:14:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abeae1db7691d99592122ca161df7a8e8cbfedddac486774e69cf9accd392d7`  
		Last Modified: Tue, 17 Aug 2021 08:18:31 GMT  
		Size: 20.9 MB (20910066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22694e209a608abf489b2dfa2c8d19ad0b9b4aef685bdd0e434f84177151f294`  
		Last Modified: Tue, 17 Aug 2021 08:18:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02bf98207b296a2375e26993ab2fcdc880bece959660400f358e1406d008cb5`  
		Last Modified: Tue, 17 Aug 2021 20:51:37 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0fb83dd3cb0b73c265cf433f1d91678ff089db984581dae7d1d453428a4fa7`  
		Last Modified: Tue, 17 Aug 2021 20:51:58 GMT  
		Size: 95.7 MB (95702221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8aea4e8357af00f5e991b04f26cba26fddc61098311960a753c628cd6caf4d`  
		Last Modified: Tue, 17 Aug 2021 20:51:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7343a3f4ffbe1dc86cf06987657ba61d467312f4e1f0073c8f5083107bb61f`  
		Last Modified: Tue, 17 Aug 2021 20:51:34 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfcd2641c5e1d3517b131c15aebea35b673a2a3da30ae1c7079ad0866f428e6`  
		Last Modified: Tue, 17 Aug 2021 20:51:35 GMT  
		Size: 2.7 MB (2749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a908197d3bc3d78feee785857c237cb4b55cf44ba30ce9f8de5f3a2d5fabbe10`  
		Last Modified: Tue, 17 Aug 2021 20:51:42 GMT  
		Size: 48.6 MB (48614002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc72195bffc42f284d34d626b447571a03853bdeef6de99476dd0e0982b4ec5e`  
		Last Modified: Tue, 17 Aug 2021 20:51:35 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; ppc64le

```console
$ docker pull redmine@sha256:6efef148967595e8835c7ce456bbd96854bc5b5bde0f00aa661936d90794159d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234101779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537c3d32f7d409d0c29fbdb569f953787339bc40657e734c3348a1fb9679b5f8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:33:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 00:33:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 01:11:31 GMT
ENV RUBY_MAJOR=2.6
# Fri, 23 Jul 2021 01:11:38 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 23 Jul 2021 01:11:44 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 23 Jul 2021 01:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 01:26:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 01:26:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 01:26:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 01:26:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 01:26:59 GMT
CMD ["irb"]
# Sat, 24 Jul 2021 02:51:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 24 Jul 2021 02:58:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Jul 2021 02:58:12 GMT
ENV RAILS_ENV=production
# Sat, 24 Jul 2021 02:58:18 GMT
WORKDIR /usr/src/redmine
# Sat, 24 Jul 2021 02:58:23 GMT
ENV HOME=/home/redmine
# Sat, 24 Jul 2021 02:58:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 02 Aug 2021 23:23:57 GMT
ENV REDMINE_VERSION=4.1.4
# Mon, 02 Aug 2021 23:24:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Mon, 02 Aug 2021 23:24:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 23:29:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 23:29:32 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 23:29:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 23:29:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:29:42 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 23:29:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f17b372a9c9122b881c2d22680e91d78ef4c329094595c61f5acb2523f41b7`  
		Last Modified: Fri, 23 Jul 2021 01:35:00 GMT  
		Size: 12.7 MB (12704330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c16cae6894266abd8c9d33cfb671a4ebb2705d8b8bb7495bafc50c3dcd344`  
		Last Modified: Fri, 23 Jul 2021 01:34:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33960675014a7e56a0cf9f85e256ec6cce1c710723a7cd8f64935709d00e323d`  
		Last Modified: Fri, 23 Jul 2021 01:38:17 GMT  
		Size: 22.0 MB (21985713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047ee7c416fdfdb76a18bc7d50d5c00c1568b5e197242760391ce18bec14da13`  
		Last Modified: Fri, 23 Jul 2021 01:38:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c93f3da9b7a0eaf5df16b7b32a686296eaa146856420c2ce2d9ee2ad916121`  
		Last Modified: Sat, 24 Jul 2021 03:36:52 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77867ad228284b5163a25c4a76739b9c38ecbf8984bbc696c8e354141fe6b00`  
		Last Modified: Sat, 24 Jul 2021 03:37:11 GMT  
		Size: 101.3 MB (101328215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1ee06db11cacc9daf59c75cefc28c1d232ac1e928afa7a6f43d367e10bd1f1`  
		Last Modified: Sat, 24 Jul 2021 03:36:48 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85237d5d99063036b3bb2790b12d7cbce41850c87c2bfbff1db63e7f5c0aa`  
		Last Modified: Sat, 24 Jul 2021 03:36:48 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b41fd52ae5e75f49d10d154992d46e779d973647edbfc7cc463b8c08b43cf95`  
		Last Modified: Mon, 02 Aug 2021 23:30:58 GMT  
		Size: 2.7 MB (2749055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9579a8a24f91bac1182097cd9218c6eb23b0e16728c8a7fb9a8386b58daf180`  
		Last Modified: Mon, 02 Aug 2021 23:31:07 GMT  
		Size: 64.8 MB (64776514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fea5dde6960e18005f909bc4dcaff30bd2eff3054518e9b24d2fc72f25038e`  
		Last Modified: Mon, 02 Aug 2021 23:30:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1` - linux; s390x

```console
$ docker pull redmine@sha256:5c79bd1a8590ca5bf82ec50e92e21512b07940797a1463edc9ddcf5fa9b56609
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216904122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d385d903de9e3d8df431fcda401c63ff60e7c93ecd4adc587a0f18c0cec4b352`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:21:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:21:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:54:27 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:54:28 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:54:29 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:57:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:57:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:57:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:57:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:57:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:57:43 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 13:35:57 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 13:36:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:36:30 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 13:36:31 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 13:36:31 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 13:36:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 13:36:32 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 13:36:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 13:36:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 13:38:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:38:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 13:38:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 13:38:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 13:38:20 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 13:38:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c03f413a15f7a98caaa2b027613636c576e3d98d8e1a98805c5978f2cc985f`  
		Last Modified: Tue, 17 Aug 2021 05:03:55 GMT  
		Size: 10.8 MB (10814401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ded0951dc51ddc1b38edf558277fec87d4169c1607312f67af2c4ffb9c4f19`  
		Last Modified: Tue, 17 Aug 2021 05:03:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b5f065983b815df03f5d378b737ce8b8950a6f775907f64c8d9413edfec507`  
		Last Modified: Tue, 17 Aug 2021 05:05:31 GMT  
		Size: 21.6 MB (21620194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c23b68c30a72cdc95043eff33b8ac51682c16759a2f483c8f4255db0f287c2`  
		Last Modified: Tue, 17 Aug 2021 05:05:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04534d357d558a08a4aea1da302e17954529ebf3804b4a0fe94cff2edac70b48`  
		Last Modified: Tue, 17 Aug 2021 13:42:39 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f89f5346ffb70bc7a8b15f07817f963fb0d00122dacff743cb5c1af76d9479`  
		Last Modified: Tue, 17 Aug 2021 13:42:51 GMT  
		Size: 91.8 MB (91789175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad842e06b48edaf468d80d1505a6ee1be7be796415dc006ca2d231db55e6b6a6`  
		Last Modified: Tue, 17 Aug 2021 13:42:37 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b320e5d26dc0c91fa46241087be2cc7e455bf87e055af14800bf2489c38c2452`  
		Last Modified: Tue, 17 Aug 2021 13:42:37 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6636b36120f102a30afdee3f007c4c76c804f392476d0db0dfec249f4c7b8a7f`  
		Last Modified: Tue, 17 Aug 2021 13:42:37 GMT  
		Size: 2.7 MB (2749060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ccb25470f9adf5b849f9a3d8fdd2393db99a602df8f5a9df60ddf284f94dd`  
		Last Modified: Tue, 17 Aug 2021 13:42:43 GMT  
		Size: 64.2 MB (64166193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126aa5be9c0306e584899b0604d54804c8fb7792dedca7cfce8c6a063d0cab14`  
		Last Modified: Tue, 17 Aug 2021 13:42:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1-alpine`

```console
$ docker pull redmine@sha256:75724ab6c055e0fb9d5c001b3e2ea96933739a169effd4d9dff712e0beec5c0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:704c3fa30632908b58ecbb9d7dfddcbbd1729a16f5d17ce4f7fc3be03b731265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161073890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4c81718646cb9796cc83de16cb4c5cb35512859b54704d82c2d2c2aad4028d3`
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
# Mon, 02 Aug 2021 19:30:38 GMT
ENV REDMINE_VERSION=4.1.4
# Mon, 02 Aug 2021 19:30:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Mon, 02 Aug 2021 19:30:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 19:30:41 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 02 Aug 2021 19:32:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 02 Aug 2021 19:32:43 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 19:32:43 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 02 Aug 2021 19:32:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 19:32:43 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 19:32:43 GMT
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
	-	`sha256:9c82c1c8b2f323e74c94315a3f2612cfb3ccc41eb9f247db68ff0821e0e089ba`  
		Last Modified: Mon, 02 Aug 2021 19:34:56 GMT  
		Size: 2.7 MB (2749721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7662a67f83cd246151d8c35ba66c66751655e34aad0846285c1dfb5a0c63284a`  
		Last Modified: Mon, 02 Aug 2021 19:35:01 GMT  
		Size: 62.5 MB (62511071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8798eb314975e00365c070021fed0c5fcb4587d78e6a72432cef4f1f7974426a`  
		Last Modified: Mon, 02 Aug 2021 19:34:55 GMT  
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
$ docker pull redmine@sha256:29ffe9263d1106c9e1dc2c854516bd360c926e8644652f2c04b7125a8cd8ad1e
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
$ docker pull redmine@sha256:4bdd1675075975131a250540a53f8880f1e0fae8b29cfbc67ddab10f6586177b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210666390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfcbb5833331e6445ac71ddc434c6a915315e32f215e0d6bc5929c81cd521053`
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
# Mon, 02 Aug 2021 21:04:50 GMT
ENV REDMINE_VERSION=4.1.4
# Mon, 02 Aug 2021 21:04:50 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Mon, 02 Aug 2021 21:04:56 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 21:10:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 21:10:36 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 21:10:37 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 21:10:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:10:38 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 21:10:38 GMT
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
	-	`sha256:a5f864c8ca3715d87914498c4905365f0ed5cbf5e0cb26b9c639534a5511833b`  
		Last Modified: Mon, 02 Aug 2021 21:12:29 GMT  
		Size: 2.7 MB (2749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4019d3cb4be9309f4cb0baa969bf37dfa6c525ade166c631d7b406cd8a3e59e4`  
		Last Modified: Mon, 02 Aug 2021 21:12:55 GMT  
		Size: 62.4 MB (62378250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564d2b0e0b86ccd1d38a66825b3d86b65542b19b9b749dd197dcf78fa771f039`  
		Last Modified: Mon, 02 Aug 2021 21:12:26 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; arm variant v7

```console
$ docker pull redmine@sha256:be260e0859e1639be25cf06cbe19352b4fb385c4942632e35f1558ddda888805
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.8 MB (203843857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f5b264322abd1cb8a7edae6550cf4a9952aa25db98c9a76125dd5ca9d1a94a`
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
# Tue, 03 Aug 2021 00:06:22 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 03 Aug 2021 00:06:23 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 03 Aug 2021 00:06:29 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 03 Aug 2021 00:11:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 03 Aug 2021 00:11:46 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 03 Aug 2021 00:11:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 03 Aug 2021 00:11:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 03 Aug 2021 00:11:48 GMT
EXPOSE 3000
# Tue, 03 Aug 2021 00:11:48 GMT
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
	-	`sha256:c129690336fa4b91fdd3354d450f70c1d503241b4f996e45a06f6cc7c5c33c8e`  
		Last Modified: Tue, 03 Aug 2021 00:13:31 GMT  
		Size: 2.7 MB (2749050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fe83cafb9bc610bb800a4c85956caaac9219e0f8a9d3c4c4951568fbaf45a4`  
		Last Modified: Tue, 03 Aug 2021 00:13:56 GMT  
		Size: 62.2 MB (62238188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8821dd99090d5f0c3476a0eabbcb4ec9b51cd0954272e8f5443c04ab694180f`  
		Last Modified: Tue, 03 Aug 2021 00:13:27 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:4d2eef074194f45decdf5b1b4a3166169b18038058b325f0d0862dbf58e89de1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.5 MB (217544129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f43f88150f3bd00e9b27ca2fb50ae014489a41818c5674b2166dabae0c267a69`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:25:18 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:25:19 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:25:19 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:27:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:27:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:27:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:27:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:27:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:27:26 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 14:19:59 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 14:20:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:20:21 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 14:20:21 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 14:20:21 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 14:20:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 14:20:22 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 14:20:22 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 14:20:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 14:22:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 14:22:50 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 14:22:50 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 14:22:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 14:22:50 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 14:22:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ab80b058f00336b15786a8d20ce50706c5277560dc1ddb487b7e5c9d24b10`  
		Last Modified: Tue, 17 Aug 2021 04:34:12 GMT  
		Size: 11.3 MB (11263042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a741dfbe27573196b9f78f97eb7f35b06eaff990866fb7f894987974bd3f6d`  
		Last Modified: Tue, 17 Aug 2021 04:36:41 GMT  
		Size: 21.3 MB (21309045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6991754b0a79718bf8ab6c058b0ca4e091450b59072ac29e34401525b4337cc2`  
		Last Modified: Tue, 17 Aug 2021 04:36:38 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b2d6fcce3e7c045cbcf366963f15eecf60f206a0f9affdb4be5f3e1cdb8e58`  
		Last Modified: Tue, 17 Aug 2021 14:26:56 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fb70beab3eb9f346f19baeada6ab2ab16b85603c8269cd25ef07d34d7d3bbd`  
		Last Modified: Tue, 17 Aug 2021 14:27:12 GMT  
		Size: 92.6 MB (92610850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88949e39e9bf16adf106d42b5c92a9aa9f223ed09de640620dab986a37998467`  
		Last Modified: Tue, 17 Aug 2021 14:26:54 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8b01342158e6f70c8d6a1fb0a08d898843a76e9eaac116f8be7bf1cd5dc0ab`  
		Last Modified: Tue, 17 Aug 2021 14:26:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a92eed4532a610d931b5637079bd2beaf67787995446f363d81a4e9afb7304c`  
		Last Modified: Tue, 17 Aug 2021 14:26:55 GMT  
		Size: 2.7 MB (2749057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4658a1e88f9cf77366e04fc9ccacb6815390e8e23e32ba77a0e63a1307a797d5`  
		Last Modified: Tue, 17 Aug 2021 14:27:02 GMT  
		Size: 63.7 MB (63692816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd3201c15e0230dd813392cedf5401f39cafe6d75e2649301390105577ef545`  
		Last Modified: Tue, 17 Aug 2021 14:26:54 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; 386

```console
$ docker pull redmine@sha256:83a453ae4bbf1d595a804d4917f72203fe31ec05b31aabf7000f4944077d6f99
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.0 MB (213004573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9d2327537f88c856b9493b788df02f70b77b9bd5ae85a1de424a2bebe50008b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:26:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:26:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 07:26:09 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:59:09 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 07:59:10 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 07:59:10 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 08:03:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 08:03:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 08:03:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 08:03:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 08:03:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 08:03:22 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 20:45:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 20:46:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:46:20 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 20:46:21 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 20:46:21 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 20:46:22 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 20:46:22 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 20:46:22 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 20:46:27 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 20:47:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 20:47:17 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 20:47:17 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 20:47:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 20:47:17 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 20:47:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7c2f28f15bebb2e6e5879bcd2a3c085881fda52f32380a12c8a0248d474ff`  
		Last Modified: Tue, 17 Aug 2021 08:14:57 GMT  
		Size: 17.2 MB (17227368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd3eff60b8a459154279d9ea96f6e521d033e44faf88a091ecf6aef5ebd4888`  
		Last Modified: Tue, 17 Aug 2021 08:14:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abeae1db7691d99592122ca161df7a8e8cbfedddac486774e69cf9accd392d7`  
		Last Modified: Tue, 17 Aug 2021 08:18:31 GMT  
		Size: 20.9 MB (20910066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22694e209a608abf489b2dfa2c8d19ad0b9b4aef685bdd0e434f84177151f294`  
		Last Modified: Tue, 17 Aug 2021 08:18:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02bf98207b296a2375e26993ab2fcdc880bece959660400f358e1406d008cb5`  
		Last Modified: Tue, 17 Aug 2021 20:51:37 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f0fb83dd3cb0b73c265cf433f1d91678ff089db984581dae7d1d453428a4fa7`  
		Last Modified: Tue, 17 Aug 2021 20:51:58 GMT  
		Size: 95.7 MB (95702221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f8aea4e8357af00f5e991b04f26cba26fddc61098311960a753c628cd6caf4d`  
		Last Modified: Tue, 17 Aug 2021 20:51:34 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7343a3f4ffbe1dc86cf06987657ba61d467312f4e1f0073c8f5083107bb61f`  
		Last Modified: Tue, 17 Aug 2021 20:51:34 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfcd2641c5e1d3517b131c15aebea35b673a2a3da30ae1c7079ad0866f428e6`  
		Last Modified: Tue, 17 Aug 2021 20:51:35 GMT  
		Size: 2.7 MB (2749054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a908197d3bc3d78feee785857c237cb4b55cf44ba30ce9f8de5f3a2d5fabbe10`  
		Last Modified: Tue, 17 Aug 2021 20:51:42 GMT  
		Size: 48.6 MB (48614002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc72195bffc42f284d34d626b447571a03853bdeef6de99476dd0e0982b4ec5e`  
		Last Modified: Tue, 17 Aug 2021 20:51:35 GMT  
		Size: 1.8 KB (1794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; ppc64le

```console
$ docker pull redmine@sha256:6efef148967595e8835c7ce456bbd96854bc5b5bde0f00aa661936d90794159d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234101779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537c3d32f7d409d0c29fbdb569f953787339bc40657e734c3348a1fb9679b5f8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:33:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 00:33:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 01:11:31 GMT
ENV RUBY_MAJOR=2.6
# Fri, 23 Jul 2021 01:11:38 GMT
ENV RUBY_VERSION=2.6.8
# Fri, 23 Jul 2021 01:11:44 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Fri, 23 Jul 2021 01:26:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 01:26:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 01:26:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 01:26:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 01:26:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 01:26:59 GMT
CMD ["irb"]
# Sat, 24 Jul 2021 02:51:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 24 Jul 2021 02:58:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Jul 2021 02:58:12 GMT
ENV RAILS_ENV=production
# Sat, 24 Jul 2021 02:58:18 GMT
WORKDIR /usr/src/redmine
# Sat, 24 Jul 2021 02:58:23 GMT
ENV HOME=/home/redmine
# Sat, 24 Jul 2021 02:58:31 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 02 Aug 2021 23:23:57 GMT
ENV REDMINE_VERSION=4.1.4
# Mon, 02 Aug 2021 23:24:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Mon, 02 Aug 2021 23:24:16 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 23:29:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 23:29:32 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 23:29:34 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 23:29:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:29:42 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 23:29:47 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f17b372a9c9122b881c2d22680e91d78ef4c329094595c61f5acb2523f41b7`  
		Last Modified: Fri, 23 Jul 2021 01:35:00 GMT  
		Size: 12.7 MB (12704330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c16cae6894266abd8c9d33cfb671a4ebb2705d8b8bb7495bafc50c3dcd344`  
		Last Modified: Fri, 23 Jul 2021 01:34:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33960675014a7e56a0cf9f85e256ec6cce1c710723a7cd8f64935709d00e323d`  
		Last Modified: Fri, 23 Jul 2021 01:38:17 GMT  
		Size: 22.0 MB (21985713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047ee7c416fdfdb76a18bc7d50d5c00c1568b5e197242760391ce18bec14da13`  
		Last Modified: Fri, 23 Jul 2021 01:38:09 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c93f3da9b7a0eaf5df16b7b32a686296eaa146856420c2ce2d9ee2ad916121`  
		Last Modified: Sat, 24 Jul 2021 03:36:52 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77867ad228284b5163a25c4a76739b9c38ecbf8984bbc696c8e354141fe6b00`  
		Last Modified: Sat, 24 Jul 2021 03:37:11 GMT  
		Size: 101.3 MB (101328215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1ee06db11cacc9daf59c75cefc28c1d232ac1e928afa7a6f43d367e10bd1f1`  
		Last Modified: Sat, 24 Jul 2021 03:36:48 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17f85237d5d99063036b3bb2790b12d7cbce41850c87c2bfbff1db63e7f5c0aa`  
		Last Modified: Sat, 24 Jul 2021 03:36:48 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b41fd52ae5e75f49d10d154992d46e779d973647edbfc7cc463b8c08b43cf95`  
		Last Modified: Mon, 02 Aug 2021 23:30:58 GMT  
		Size: 2.7 MB (2749055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9579a8a24f91bac1182097cd9218c6eb23b0e16728c8a7fb9a8386b58daf180`  
		Last Modified: Mon, 02 Aug 2021 23:31:07 GMT  
		Size: 64.8 MB (64776514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90fea5dde6960e18005f909bc4dcaff30bd2eff3054518e9b24d2fc72f25038e`  
		Last Modified: Mon, 02 Aug 2021 23:30:57 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.1.4` - linux; s390x

```console
$ docker pull redmine@sha256:5c79bd1a8590ca5bf82ec50e92e21512b07940797a1463edc9ddcf5fa9b56609
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216904122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d385d903de9e3d8df431fcda401c63ff60e7c93ecd4adc587a0f18c0cec4b352`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:21:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:21:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:54:27 GMT
ENV RUBY_MAJOR=2.6
# Tue, 17 Aug 2021 04:54:28 GMT
ENV RUBY_VERSION=2.6.8
# Tue, 17 Aug 2021 04:54:29 GMT
ENV RUBY_DOWNLOAD_SHA256=8262e4663169c85787fdc9bfbd04d9eb86eb2a4b56d7f98373a8fcaa18e593eb
# Tue, 17 Aug 2021 04:57:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:57:40 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:57:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:57:41 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:57:42 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:57:43 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 13:35:57 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 13:36:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:36:30 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 13:36:31 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 13:36:31 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 13:36:32 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 13:36:32 GMT
ENV REDMINE_VERSION=4.1.4
# Tue, 17 Aug 2021 13:36:32 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Tue, 17 Aug 2021 13:36:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 13:38:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:38:20 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 13:38:20 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 13:38:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 13:38:20 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 13:38:21 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c03f413a15f7a98caaa2b027613636c576e3d98d8e1a98805c5978f2cc985f`  
		Last Modified: Tue, 17 Aug 2021 05:03:55 GMT  
		Size: 10.8 MB (10814401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ded0951dc51ddc1b38edf558277fec87d4169c1607312f67af2c4ffb9c4f19`  
		Last Modified: Tue, 17 Aug 2021 05:03:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b5f065983b815df03f5d378b737ce8b8950a6f775907f64c8d9413edfec507`  
		Last Modified: Tue, 17 Aug 2021 05:05:31 GMT  
		Size: 21.6 MB (21620194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c23b68c30a72cdc95043eff33b8ac51682c16759a2f483c8f4255db0f287c2`  
		Last Modified: Tue, 17 Aug 2021 05:05:28 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04534d357d558a08a4aea1da302e17954529ebf3804b4a0fe94cff2edac70b48`  
		Last Modified: Tue, 17 Aug 2021 13:42:39 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f89f5346ffb70bc7a8b15f07817f963fb0d00122dacff743cb5c1af76d9479`  
		Last Modified: Tue, 17 Aug 2021 13:42:51 GMT  
		Size: 91.8 MB (91789175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad842e06b48edaf468d80d1505a6ee1be7be796415dc006ca2d231db55e6b6a6`  
		Last Modified: Tue, 17 Aug 2021 13:42:37 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b320e5d26dc0c91fa46241087be2cc7e455bf87e055af14800bf2489c38c2452`  
		Last Modified: Tue, 17 Aug 2021 13:42:37 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6636b36120f102a30afdee3f007c4c76c804f392476d0db0dfec249f4c7b8a7f`  
		Last Modified: Tue, 17 Aug 2021 13:42:37 GMT  
		Size: 2.7 MB (2749060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55ccb25470f9adf5b849f9a3d8fdd2393db99a602df8f5a9df60ddf284f94dd`  
		Last Modified: Tue, 17 Aug 2021 13:42:43 GMT  
		Size: 64.2 MB (64166193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126aa5be9c0306e584899b0604d54804c8fb7792dedca7cfce8c6a063d0cab14`  
		Last Modified: Tue, 17 Aug 2021 13:42:37 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.1.4-alpine`

```console
$ docker pull redmine@sha256:75724ab6c055e0fb9d5c001b3e2ea96933739a169effd4d9dff712e0beec5c0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.1.4-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:704c3fa30632908b58ecbb9d7dfddcbbd1729a16f5d17ce4f7fc3be03b731265
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.1 MB (161073890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4c81718646cb9796cc83de16cb4c5cb35512859b54704d82c2d2c2aad4028d3`
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
# Mon, 02 Aug 2021 19:30:38 GMT
ENV REDMINE_VERSION=4.1.4
# Mon, 02 Aug 2021 19:30:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=beaf6e51bb6a0c7655d73410afdf50c24091ee5f11eda0c9e96f38dfa7a3ab9f
# Mon, 02 Aug 2021 19:30:41 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 19:30:41 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 02 Aug 2021 19:32:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 02 Aug 2021 19:32:43 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 19:32:43 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 02 Aug 2021 19:32:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 19:32:43 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 19:32:43 GMT
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
	-	`sha256:9c82c1c8b2f323e74c94315a3f2612cfb3ccc41eb9f247db68ff0821e0e089ba`  
		Last Modified: Mon, 02 Aug 2021 19:34:56 GMT  
		Size: 2.7 MB (2749721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7662a67f83cd246151d8c35ba66c66751655e34aad0846285c1dfb5a0c63284a`  
		Last Modified: Mon, 02 Aug 2021 19:35:01 GMT  
		Size: 62.5 MB (62511071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8798eb314975e00365c070021fed0c5fcb4587d78e6a72432cef4f1f7974426a`  
		Last Modified: Mon, 02 Aug 2021 19:34:55 GMT  
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
$ docker pull redmine@sha256:e09ada96ab20fcef1ba9247b23d9c451ef65719d98e25922c2c11226840af94a
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
$ docker pull redmine@sha256:2ba20de8f2d5813171b6b38d1e727aba839ab6cdd974c966ed2b8cd016b97c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196974835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2290c3ececd51c95738415fab07fc46dcc63d3a61e8099fb6c45e290ec3f0d91`
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
# Mon, 02 Aug 2021 20:58:44 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 20:58:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 20:58:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 21:04:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 21:04:31 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 21:04:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 21:04:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:04:32 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 21:04:32 GMT
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
	-	`sha256:7342031318accab10946b43b34804e02f1e0c107a6af3af5a4ebb766152ee509`  
		Last Modified: Mon, 02 Aug 2021 21:11:42 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648b6a3dac4889e5f68f30776a664fe9d62256592f37d6d2912163da56f265fa`  
		Last Modified: Mon, 02 Aug 2021 21:12:04 GMT  
		Size: 55.2 MB (55235555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5a29c2452fcab6625565bca85ff5fccfbee37e09b6f1e8455655c2735c166a`  
		Last Modified: Mon, 02 Aug 2021 21:11:38 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cac694ac7078f02298b587000698d84cb3bb69637d30c724bd0bcac087c22f41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3187fd285a60bd484a8586f3ee1dc8896c0c94e433a102025bf0dae4c344c1b7`
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
# Tue, 03 Aug 2021 00:00:45 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 03 Aug 2021 00:00:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 03 Aug 2021 00:00:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 03 Aug 2021 00:06:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 03 Aug 2021 00:06:06 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 03 Aug 2021 00:06:07 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 03 Aug 2021 00:06:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 03 Aug 2021 00:06:08 GMT
EXPOSE 3000
# Tue, 03 Aug 2021 00:06:08 GMT
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
	-	`sha256:fc2c8055fd9194f59346984cbb7941b37a40023edc25ab3dec3e42e9b8c01287`  
		Last Modified: Tue, 03 Aug 2021 00:12:46 GMT  
		Size: 3.1 MB (3061917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836246f3dcf57e23a39d002b3b9d9a09fedb40b5b6accc7268b28ae167eca128`  
		Last Modified: Tue, 03 Aug 2021 00:13:05 GMT  
		Size: 55.1 MB (55073644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63001a72a77f002e6a9f105ba97f4e5cb147287597ca1e71c8670c6b0e768390`  
		Last Modified: Tue, 03 Aug 2021 00:12:42 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:168d7ed49573c2aaecf2d0d8adcc21280d9e2c18dc1ddb19848393c9847211e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203243298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a980ba1133cf226e557df7c34d75d5c5e7bfb359db4c611a013f2dd737ac6dc4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:20:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:20:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:20:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:20:13 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 14:17:02 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 14:17:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:17:25 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 14:17:26 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 14:17:26 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 14:17:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 14:17:27 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 14:17:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 14:17:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 14:19:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 14:19:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 14:19:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 14:19:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 14:19:48 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 14:19:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ab80b058f00336b15786a8d20ce50706c5277560dc1ddb487b7e5c9d24b10`  
		Last Modified: Tue, 17 Aug 2021 04:34:12 GMT  
		Size: 11.3 MB (11263042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2cb28558c1dd6c31a020484f10c613185335d6d30e7c7a81d3e6ffd0f374f0`  
		Last Modified: Tue, 17 Aug 2021 04:35:35 GMT  
		Size: 14.4 MB (14356587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49391d2e67bfbf4fd993b49c9be1225f0a09d4177c605548f82d49cbcfe78b99`  
		Last Modified: Tue, 17 Aug 2021 04:35:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9307e85455464623a9445ee9314b11fd777c561cefed9b38e6f9067bd30653a`  
		Last Modified: Tue, 17 Aug 2021 14:26:18 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba598bababc240a9c29cf82ac1a0b01837945e37b3cb2b17a3a55ba776227b76`  
		Last Modified: Tue, 17 Aug 2021 14:26:34 GMT  
		Size: 92.6 MB (92611086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dc88258ae8d8cf36219a3b41b130d1e21bf4c2dfb6e1cf9c3f6b3ae2395817`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c9b592ea00c036970d3b4b7baf687de5e9394670884daa30890ab191cfe5bb`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8230053e3f65d96319f5f2351fc906de79749654a83811bf21ea7b34f3bee`  
		Last Modified: Tue, 17 Aug 2021 14:26:17 GMT  
		Size: 3.1 MB (3061920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe117b5c157b62194a629b77cf9c9b15c6821516a74c96470c098adba14546ba`  
		Last Modified: Tue, 17 Aug 2021 14:26:22 GMT  
		Size: 56.0 MB (56031346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9fc675e51cbab5a7a0574bbd10f6ebdc614381aa4a451a98f5884e386b455`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; 386

```console
$ docker pull redmine@sha256:8b2bacb3a529c3a9da30411ee264532f973e5f07226b10f40cca6d31db43a621
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202125065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20cd127add6f4bd712d08c14e2b3a570aa6216ac3e81f7498d128b38ad693d1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:26:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:26:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 07:26:09 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:43:14 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 07:43:14 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 07:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 07:46:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 07:46:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 07:46:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 07:46:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 07:46:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 07:46:43 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 20:44:09 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 20:44:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:44:42 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 20:44:42 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 20:44:42 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 20:44:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 20:44:43 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 20:44:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 20:44:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 20:45:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 20:45:39 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 20:45:39 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 20:45:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 20:45:39 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 20:45:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7c2f28f15bebb2e6e5879bcd2a3c085881fda52f32380a12c8a0248d474ff`  
		Last Modified: Tue, 17 Aug 2021 08:14:57 GMT  
		Size: 17.2 MB (17227368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd3eff60b8a459154279d9ea96f6e521d033e44faf88a091ecf6aef5ebd4888`  
		Last Modified: Tue, 17 Aug 2021 08:14:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d6e92558e2e9952c84a3effe46c647bb2ec5c677559440a30b3472898d5ca2`  
		Last Modified: Tue, 17 Aug 2021 08:16:53 GMT  
		Size: 14.0 MB (13992678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149425e111bee81e3749bcd1a01f973bdea53d5107f36b0ce5ab6f24a5d26bd0`  
		Last Modified: Tue, 17 Aug 2021 08:16:50 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba2aa95ab76e668ab9334a63f10abb5c9cc72b5ce42c0288b8e258d2421de4c`  
		Last Modified: Tue, 17 Aug 2021 20:50:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e3c06b49e4b7fdda9acea36456b2c0c69f0f52f0d50724e55b0f5cdc42ce93`  
		Last Modified: Tue, 17 Aug 2021 20:51:14 GMT  
		Size: 95.7 MB (95702973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d658498d2e116af9d55f933669635cd567034d03d7c862e5be6b2affa43ef371`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d6e976830ca03935c308924157582258b4599ff1a78443efeef21cc6e0c4e5`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db706ca27afe38d047ff274c96b1d95fc75f4512bfd5967afd3854127d17087d`  
		Last Modified: Tue, 17 Aug 2021 20:50:51 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1417c9a42064182a2e270bd603d1fa078906a8999616843228fd988741802494`  
		Last Modified: Tue, 17 Aug 2021 20:50:58 GMT  
		Size: 44.3 MB (44338264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eed6830dcebdb2ec5236d072e5b78c805b2ad7749fa0de197a129adb76a2abf`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; ppc64le

```console
$ docker pull redmine@sha256:ecdb00827fcf83f2f12c122af3ffc2420a6faa270cd7b048c9756f927f7c77fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219650618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57391c1536ff89c22d27544dc68890a924a8d455796c92bdc28721108b71a53c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:33:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 00:33:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 00:52:18 GMT
ENV RUBY_MAJOR=2.7
# Fri, 23 Jul 2021 00:52:28 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 23 Jul 2021 00:52:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 23 Jul 2021 01:01:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 01:01:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 01:01:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 01:01:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 01:01:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 01:01:58 GMT
CMD ["irb"]
# Sat, 24 Jul 2021 02:42:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 24 Jul 2021 02:46:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Jul 2021 02:46:14 GMT
ENV RAILS_ENV=production
# Sat, 24 Jul 2021 02:46:17 GMT
WORKDIR /usr/src/redmine
# Sat, 24 Jul 2021 02:46:19 GMT
ENV HOME=/home/redmine
# Sat, 24 Jul 2021 02:46:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 02 Aug 2021 23:16:59 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 23:17:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 23:17:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 23:23:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 23:23:26 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 23:23:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 23:23:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:23:37 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 23:23:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f17b372a9c9122b881c2d22680e91d78ef4c329094595c61f5acb2523f41b7`  
		Last Modified: Fri, 23 Jul 2021 01:35:00 GMT  
		Size: 12.7 MB (12704330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c16cae6894266abd8c9d33cfb671a4ebb2705d8b8bb7495bafc50c3dcd344`  
		Last Modified: Fri, 23 Jul 2021 01:34:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76d2032e7e646d23109ea1a55abb581c169350b85836914155a6837d64eb757`  
		Last Modified: Fri, 23 Jul 2021 01:36:48 GMT  
		Size: 15.0 MB (14997545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f996a3088f8cd5e20b9f19c3aebdd4a6228a85b6c0a83f9dde8e2a5ec82976d3`  
		Last Modified: Fri, 23 Jul 2021 01:36:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acdc172d0fc27092df5794b7a17e2c42e7f2497e85086076f490e273db428fe`  
		Last Modified: Sat, 24 Jul 2021 03:36:05 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe4ded3f0db610cc9dca87e98b2305c850cbaf595886ccb44e3492ad727b18`  
		Last Modified: Sat, 24 Jul 2021 03:36:28 GMT  
		Size: 101.3 MB (101327533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14617640fcda340a6bc04fd1c65d4183ad0dd01a4e3b44fb313d164071471e95`  
		Last Modified: Sat, 24 Jul 2021 03:36:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1b361a5633d0ca044cc644bddc99329645edadfff1cbb48e966deb9b0d079a`  
		Last Modified: Sat, 24 Jul 2021 03:36:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bfbd857622d0239bfa521d75318f40925e9e4608a62a4be7abc2bc89801ec3`  
		Last Modified: Mon, 02 Aug 2021 23:30:32 GMT  
		Size: 3.1 MB (3061921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4b836dd92fc0980e6e61a697cc881ceb76ca811af742788283ab3211698e1`  
		Last Modified: Mon, 02 Aug 2021 23:30:38 GMT  
		Size: 57.0 MB (57001331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2976222796409af9d080f03664b07bc2a177c8b37d29e7937c0620ba5f908d03`  
		Last Modified: Mon, 02 Aug 2021 23:30:31 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2` - linux; s390x

```console
$ docker pull redmine@sha256:33d5a2369e443a1bb092e9da696586fae6988113fc4ef99bf98b5af5e03135f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202554693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f13509159fb8e3ef52d7620d4ef325ebe2d7a388fec2faf172536b64ee9ae9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:21:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:21:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:37:51 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:37:51 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:37:52 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:40:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:40:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:40:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:40:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:40:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:40:24 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 13:32:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 13:33:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:33:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 13:33:28 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 13:33:28 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 13:33:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 13:33:29 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 13:33:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 13:33:32 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 13:35:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:35:38 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 13:35:38 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 13:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 13:35:39 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 13:35:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c03f413a15f7a98caaa2b027613636c576e3d98d8e1a98805c5978f2cc985f`  
		Last Modified: Tue, 17 Aug 2021 05:03:55 GMT  
		Size: 10.8 MB (10814401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ded0951dc51ddc1b38edf558277fec87d4169c1607312f67af2c4ffb9c4f19`  
		Last Modified: Tue, 17 Aug 2021 05:03:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d49ef1e1c8f0247bfa63924e738fc94dc0c4a81ec0e4b2b73df09f08d080005`  
		Last Modified: Tue, 17 Aug 2021 05:04:49 GMT  
		Size: 14.7 MB (14697415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54919ecbd2a42d851761e24bb9a1e9e71346c6ecd753a4c6b7868679823367b`  
		Last Modified: Tue, 17 Aug 2021 05:04:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159f1e20f87d626bb303eea037968c316700fdd1fd9fa734e8ebacf14608ab2`  
		Last Modified: Tue, 17 Aug 2021 13:42:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223675cd45b3e6a43e45f6ad1a699c278dc5effe72583bec3657746c84a2a692`  
		Last Modified: Tue, 17 Aug 2021 13:42:24 GMT  
		Size: 91.8 MB (91792621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e74adea5c6a7d4c0be869fe00b2451a51e188e2c0e1466d72eaad06cc9d`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cd2e454b71a3aea72543018a9596e611b94ee88301b3d5971854daab02981`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885ccd7ef756fbf397809a3541c6cadba886972a35c3f9d9d00cc920b16ef2`  
		Last Modified: Tue, 17 Aug 2021 13:42:11 GMT  
		Size: 3.1 MB (3061920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde4808141553382cd3c73078af6ba86889e806ed72c6251287678fbce48b5ea`  
		Last Modified: Tue, 17 Aug 2021 13:42:15 GMT  
		Size: 56.4 MB (56423232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed18e7c147f9b19d7cb774a6462749d36a61882e80d34fff6912e4ed7990252d`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2-alpine`

```console
$ docker pull redmine@sha256:34362d64f5cac220ecf3058a2982583ec0e2cba35273960105a4cff3dc0c4a5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:429416f2012459eaa042fe2879ae170f0d1ee68b283059b2e4f855edcaae0101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150082289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a3f4194f1bef28b7e8c9cb584331cfe9876976fd1c68e194837191b82282e8`
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
# Mon, 02 Aug 2021 19:27:15 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 19:27:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 19:27:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 19:27:19 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 02 Aug 2021 19:29:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 02 Aug 2021 19:29:21 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 19:29:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 02 Aug 2021 19:29:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 19:29:22 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 19:29:22 GMT
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
	-	`sha256:e98c03ed41f8aa891bcd79e61fbb88cda198d71f5a8de4f510950e7f58aa1a15`  
		Last Modified: Mon, 02 Aug 2021 19:34:04 GMT  
		Size: 3.1 MB (3062843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08d14dd9ea01201645da35bc3855c4b0a6270b9d4ae9510f9da35fb4150e833`  
		Last Modified: Mon, 02 Aug 2021 19:34:08 GMT  
		Size: 56.7 MB (56722754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bee94fd486f4fb693e4765ade966dd49ee96cd0aff32109f156b9a2511d1af3`  
		Last Modified: Mon, 02 Aug 2021 19:34:03 GMT  
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
$ docker pull redmine@sha256:e09ada96ab20fcef1ba9247b23d9c451ef65719d98e25922c2c11226840af94a
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
$ docker pull redmine@sha256:2ba20de8f2d5813171b6b38d1e727aba839ab6cdd974c966ed2b8cd016b97c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196974835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2290c3ececd51c95738415fab07fc46dcc63d3a61e8099fb6c45e290ec3f0d91`
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
# Mon, 02 Aug 2021 20:58:44 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 20:58:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 20:58:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 21:04:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 21:04:31 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 21:04:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 21:04:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:04:32 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 21:04:32 GMT
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
	-	`sha256:7342031318accab10946b43b34804e02f1e0c107a6af3af5a4ebb766152ee509`  
		Last Modified: Mon, 02 Aug 2021 21:11:42 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648b6a3dac4889e5f68f30776a664fe9d62256592f37d6d2912163da56f265fa`  
		Last Modified: Mon, 02 Aug 2021 21:12:04 GMT  
		Size: 55.2 MB (55235555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5a29c2452fcab6625565bca85ff5fccfbee37e09b6f1e8455655c2735c166a`  
		Last Modified: Mon, 02 Aug 2021 21:11:38 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cac694ac7078f02298b587000698d84cb3bb69637d30c724bd0bcac087c22f41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3187fd285a60bd484a8586f3ee1dc8896c0c94e433a102025bf0dae4c344c1b7`
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
# Tue, 03 Aug 2021 00:00:45 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 03 Aug 2021 00:00:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 03 Aug 2021 00:00:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 03 Aug 2021 00:06:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 03 Aug 2021 00:06:06 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 03 Aug 2021 00:06:07 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 03 Aug 2021 00:06:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 03 Aug 2021 00:06:08 GMT
EXPOSE 3000
# Tue, 03 Aug 2021 00:06:08 GMT
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
	-	`sha256:fc2c8055fd9194f59346984cbb7941b37a40023edc25ab3dec3e42e9b8c01287`  
		Last Modified: Tue, 03 Aug 2021 00:12:46 GMT  
		Size: 3.1 MB (3061917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836246f3dcf57e23a39d002b3b9d9a09fedb40b5b6accc7268b28ae167eca128`  
		Last Modified: Tue, 03 Aug 2021 00:13:05 GMT  
		Size: 55.1 MB (55073644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63001a72a77f002e6a9f105ba97f4e5cb147287597ca1e71c8670c6b0e768390`  
		Last Modified: Tue, 03 Aug 2021 00:12:42 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:168d7ed49573c2aaecf2d0d8adcc21280d9e2c18dc1ddb19848393c9847211e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203243298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a980ba1133cf226e557df7c34d75d5c5e7bfb359db4c611a013f2dd737ac6dc4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:20:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:20:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:20:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:20:13 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 14:17:02 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 14:17:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:17:25 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 14:17:26 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 14:17:26 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 14:17:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 14:17:27 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 14:17:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 14:17:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 14:19:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 14:19:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 14:19:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 14:19:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 14:19:48 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 14:19:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ab80b058f00336b15786a8d20ce50706c5277560dc1ddb487b7e5c9d24b10`  
		Last Modified: Tue, 17 Aug 2021 04:34:12 GMT  
		Size: 11.3 MB (11263042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2cb28558c1dd6c31a020484f10c613185335d6d30e7c7a81d3e6ffd0f374f0`  
		Last Modified: Tue, 17 Aug 2021 04:35:35 GMT  
		Size: 14.4 MB (14356587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49391d2e67bfbf4fd993b49c9be1225f0a09d4177c605548f82d49cbcfe78b99`  
		Last Modified: Tue, 17 Aug 2021 04:35:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9307e85455464623a9445ee9314b11fd777c561cefed9b38e6f9067bd30653a`  
		Last Modified: Tue, 17 Aug 2021 14:26:18 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba598bababc240a9c29cf82ac1a0b01837945e37b3cb2b17a3a55ba776227b76`  
		Last Modified: Tue, 17 Aug 2021 14:26:34 GMT  
		Size: 92.6 MB (92611086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dc88258ae8d8cf36219a3b41b130d1e21bf4c2dfb6e1cf9c3f6b3ae2395817`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c9b592ea00c036970d3b4b7baf687de5e9394670884daa30890ab191cfe5bb`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8230053e3f65d96319f5f2351fc906de79749654a83811bf21ea7b34f3bee`  
		Last Modified: Tue, 17 Aug 2021 14:26:17 GMT  
		Size: 3.1 MB (3061920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe117b5c157b62194a629b77cf9c9b15c6821516a74c96470c098adba14546ba`  
		Last Modified: Tue, 17 Aug 2021 14:26:22 GMT  
		Size: 56.0 MB (56031346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9fc675e51cbab5a7a0574bbd10f6ebdc614381aa4a451a98f5884e386b455`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; 386

```console
$ docker pull redmine@sha256:8b2bacb3a529c3a9da30411ee264532f973e5f07226b10f40cca6d31db43a621
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202125065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20cd127add6f4bd712d08c14e2b3a570aa6216ac3e81f7498d128b38ad693d1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:26:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:26:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 07:26:09 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:43:14 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 07:43:14 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 07:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 07:46:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 07:46:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 07:46:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 07:46:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 07:46:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 07:46:43 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 20:44:09 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 20:44:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:44:42 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 20:44:42 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 20:44:42 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 20:44:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 20:44:43 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 20:44:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 20:44:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 20:45:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 20:45:39 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 20:45:39 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 20:45:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 20:45:39 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 20:45:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7c2f28f15bebb2e6e5879bcd2a3c085881fda52f32380a12c8a0248d474ff`  
		Last Modified: Tue, 17 Aug 2021 08:14:57 GMT  
		Size: 17.2 MB (17227368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd3eff60b8a459154279d9ea96f6e521d033e44faf88a091ecf6aef5ebd4888`  
		Last Modified: Tue, 17 Aug 2021 08:14:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d6e92558e2e9952c84a3effe46c647bb2ec5c677559440a30b3472898d5ca2`  
		Last Modified: Tue, 17 Aug 2021 08:16:53 GMT  
		Size: 14.0 MB (13992678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149425e111bee81e3749bcd1a01f973bdea53d5107f36b0ce5ab6f24a5d26bd0`  
		Last Modified: Tue, 17 Aug 2021 08:16:50 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba2aa95ab76e668ab9334a63f10abb5c9cc72b5ce42c0288b8e258d2421de4c`  
		Last Modified: Tue, 17 Aug 2021 20:50:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e3c06b49e4b7fdda9acea36456b2c0c69f0f52f0d50724e55b0f5cdc42ce93`  
		Last Modified: Tue, 17 Aug 2021 20:51:14 GMT  
		Size: 95.7 MB (95702973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d658498d2e116af9d55f933669635cd567034d03d7c862e5be6b2affa43ef371`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d6e976830ca03935c308924157582258b4599ff1a78443efeef21cc6e0c4e5`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db706ca27afe38d047ff274c96b1d95fc75f4512bfd5967afd3854127d17087d`  
		Last Modified: Tue, 17 Aug 2021 20:50:51 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1417c9a42064182a2e270bd603d1fa078906a8999616843228fd988741802494`  
		Last Modified: Tue, 17 Aug 2021 20:50:58 GMT  
		Size: 44.3 MB (44338264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eed6830dcebdb2ec5236d072e5b78c805b2ad7749fa0de197a129adb76a2abf`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; ppc64le

```console
$ docker pull redmine@sha256:ecdb00827fcf83f2f12c122af3ffc2420a6faa270cd7b048c9756f927f7c77fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219650618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57391c1536ff89c22d27544dc68890a924a8d455796c92bdc28721108b71a53c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:33:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 00:33:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 00:52:18 GMT
ENV RUBY_MAJOR=2.7
# Fri, 23 Jul 2021 00:52:28 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 23 Jul 2021 00:52:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 23 Jul 2021 01:01:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 01:01:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 01:01:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 01:01:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 01:01:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 01:01:58 GMT
CMD ["irb"]
# Sat, 24 Jul 2021 02:42:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 24 Jul 2021 02:46:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Jul 2021 02:46:14 GMT
ENV RAILS_ENV=production
# Sat, 24 Jul 2021 02:46:17 GMT
WORKDIR /usr/src/redmine
# Sat, 24 Jul 2021 02:46:19 GMT
ENV HOME=/home/redmine
# Sat, 24 Jul 2021 02:46:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 02 Aug 2021 23:16:59 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 23:17:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 23:17:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 23:23:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 23:23:26 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 23:23:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 23:23:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:23:37 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 23:23:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f17b372a9c9122b881c2d22680e91d78ef4c329094595c61f5acb2523f41b7`  
		Last Modified: Fri, 23 Jul 2021 01:35:00 GMT  
		Size: 12.7 MB (12704330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c16cae6894266abd8c9d33cfb671a4ebb2705d8b8bb7495bafc50c3dcd344`  
		Last Modified: Fri, 23 Jul 2021 01:34:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76d2032e7e646d23109ea1a55abb581c169350b85836914155a6837d64eb757`  
		Last Modified: Fri, 23 Jul 2021 01:36:48 GMT  
		Size: 15.0 MB (14997545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f996a3088f8cd5e20b9f19c3aebdd4a6228a85b6c0a83f9dde8e2a5ec82976d3`  
		Last Modified: Fri, 23 Jul 2021 01:36:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acdc172d0fc27092df5794b7a17e2c42e7f2497e85086076f490e273db428fe`  
		Last Modified: Sat, 24 Jul 2021 03:36:05 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe4ded3f0db610cc9dca87e98b2305c850cbaf595886ccb44e3492ad727b18`  
		Last Modified: Sat, 24 Jul 2021 03:36:28 GMT  
		Size: 101.3 MB (101327533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14617640fcda340a6bc04fd1c65d4183ad0dd01a4e3b44fb313d164071471e95`  
		Last Modified: Sat, 24 Jul 2021 03:36:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1b361a5633d0ca044cc644bddc99329645edadfff1cbb48e966deb9b0d079a`  
		Last Modified: Sat, 24 Jul 2021 03:36:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bfbd857622d0239bfa521d75318f40925e9e4608a62a4be7abc2bc89801ec3`  
		Last Modified: Mon, 02 Aug 2021 23:30:32 GMT  
		Size: 3.1 MB (3061921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4b836dd92fc0980e6e61a697cc881ceb76ca811af742788283ab3211698e1`  
		Last Modified: Mon, 02 Aug 2021 23:30:38 GMT  
		Size: 57.0 MB (57001331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2976222796409af9d080f03664b07bc2a177c8b37d29e7937c0620ba5f908d03`  
		Last Modified: Mon, 02 Aug 2021 23:30:31 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:4.2.2` - linux; s390x

```console
$ docker pull redmine@sha256:33d5a2369e443a1bb092e9da696586fae6988113fc4ef99bf98b5af5e03135f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202554693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f13509159fb8e3ef52d7620d4ef325ebe2d7a388fec2faf172536b64ee9ae9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:21:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:21:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:37:51 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:37:51 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:37:52 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:40:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:40:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:40:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:40:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:40:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:40:24 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 13:32:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 13:33:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:33:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 13:33:28 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 13:33:28 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 13:33:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 13:33:29 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 13:33:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 13:33:32 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 13:35:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:35:38 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 13:35:38 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 13:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 13:35:39 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 13:35:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c03f413a15f7a98caaa2b027613636c576e3d98d8e1a98805c5978f2cc985f`  
		Last Modified: Tue, 17 Aug 2021 05:03:55 GMT  
		Size: 10.8 MB (10814401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ded0951dc51ddc1b38edf558277fec87d4169c1607312f67af2c4ffb9c4f19`  
		Last Modified: Tue, 17 Aug 2021 05:03:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d49ef1e1c8f0247bfa63924e738fc94dc0c4a81ec0e4b2b73df09f08d080005`  
		Last Modified: Tue, 17 Aug 2021 05:04:49 GMT  
		Size: 14.7 MB (14697415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54919ecbd2a42d851761e24bb9a1e9e71346c6ecd753a4c6b7868679823367b`  
		Last Modified: Tue, 17 Aug 2021 05:04:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159f1e20f87d626bb303eea037968c316700fdd1fd9fa734e8ebacf14608ab2`  
		Last Modified: Tue, 17 Aug 2021 13:42:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223675cd45b3e6a43e45f6ad1a699c278dc5effe72583bec3657746c84a2a692`  
		Last Modified: Tue, 17 Aug 2021 13:42:24 GMT  
		Size: 91.8 MB (91792621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e74adea5c6a7d4c0be869fe00b2451a51e188e2c0e1466d72eaad06cc9d`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cd2e454b71a3aea72543018a9596e611b94ee88301b3d5971854daab02981`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885ccd7ef756fbf397809a3541c6cadba886972a35c3f9d9d00cc920b16ef2`  
		Last Modified: Tue, 17 Aug 2021 13:42:11 GMT  
		Size: 3.1 MB (3061920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde4808141553382cd3c73078af6ba86889e806ed72c6251287678fbce48b5ea`  
		Last Modified: Tue, 17 Aug 2021 13:42:15 GMT  
		Size: 56.4 MB (56423232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed18e7c147f9b19d7cb774a6462749d36a61882e80d34fff6912e4ed7990252d`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:4.2.2-alpine`

```console
$ docker pull redmine@sha256:34362d64f5cac220ecf3058a2982583ec0e2cba35273960105a4cff3dc0c4a5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4.2.2-alpine` - linux; amd64

```console
$ docker pull redmine@sha256:429416f2012459eaa042fe2879ae170f0d1ee68b283059b2e4f855edcaae0101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150082289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a3f4194f1bef28b7e8c9cb584331cfe9876976fd1c68e194837191b82282e8`
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
# Mon, 02 Aug 2021 19:27:15 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 19:27:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 19:27:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 19:27:19 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 02 Aug 2021 19:29:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 02 Aug 2021 19:29:21 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 19:29:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 02 Aug 2021 19:29:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 19:29:22 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 19:29:22 GMT
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
	-	`sha256:e98c03ed41f8aa891bcd79e61fbb88cda198d71f5a8de4f510950e7f58aa1a15`  
		Last Modified: Mon, 02 Aug 2021 19:34:04 GMT  
		Size: 3.1 MB (3062843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08d14dd9ea01201645da35bc3855c4b0a6270b9d4ae9510f9da35fb4150e833`  
		Last Modified: Mon, 02 Aug 2021 19:34:08 GMT  
		Size: 56.7 MB (56722754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bee94fd486f4fb693e4765ade966dd49ee96cd0aff32109f156b9a2511d1af3`  
		Last Modified: Mon, 02 Aug 2021 19:34:03 GMT  
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
$ docker pull redmine@sha256:34362d64f5cac220ecf3058a2982583ec0e2cba35273960105a4cff3dc0c4a5e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:alpine` - linux; amd64

```console
$ docker pull redmine@sha256:429416f2012459eaa042fe2879ae170f0d1ee68b283059b2e4f855edcaae0101
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.1 MB (150082289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00a3f4194f1bef28b7e8c9cb584331cfe9876976fd1c68e194837191b82282e8`
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
# Mon, 02 Aug 2021 19:27:15 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 19:27:15 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 19:27:19 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 19:27:19 GMT
ENV BUNDLE_FORCE_RUBY_PLATFORM=1
# Mon, 02 Aug 2021 19:29:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetds-dev 		gcc 		make 		mariadb-dev 		musl-dev 		patch 		postgresql-dev 		sqlite-dev 		ttf2ufm 		zlib-dev 	; 		su-exec redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	su-exec redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		rm /usr/local/bundle/gems/rbpdf-font-1.19.*/lib/fonts/ttf2ufm/ttf2ufm; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/bundle/gems 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .redmine-rundeps $runDeps; 	apk del --no-network .build-deps
# Mon, 02 Aug 2021 19:29:21 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 19:29:22 GMT
COPY file:d7d49d1509d97205d05405670ad206509bb871741a17d5270a1b8842b05afc0f in / 
# Mon, 02 Aug 2021 19:29:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 19:29:22 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 19:29:22 GMT
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
	-	`sha256:e98c03ed41f8aa891bcd79e61fbb88cda198d71f5a8de4f510950e7f58aa1a15`  
		Last Modified: Mon, 02 Aug 2021 19:34:04 GMT  
		Size: 3.1 MB (3062843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08d14dd9ea01201645da35bc3855c4b0a6270b9d4ae9510f9da35fb4150e833`  
		Last Modified: Mon, 02 Aug 2021 19:34:08 GMT  
		Size: 56.7 MB (56722754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bee94fd486f4fb693e4765ade966dd49ee96cd0aff32109f156b9a2511d1af3`  
		Last Modified: Mon, 02 Aug 2021 19:34:03 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `redmine:latest`

```console
$ docker pull redmine@sha256:e09ada96ab20fcef1ba9247b23d9c451ef65719d98e25922c2c11226840af94a
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
$ docker pull redmine@sha256:2ba20de8f2d5813171b6b38d1e727aba839ab6cdd974c966ed2b8cd016b97c70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.0 MB (196974835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2290c3ececd51c95738415fab07fc46dcc63d3a61e8099fb6c45e290ec3f0d91`
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
# Mon, 02 Aug 2021 20:58:44 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 20:58:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 20:58:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 21:04:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 21:04:31 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 21:04:31 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 21:04:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 21:04:32 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 21:04:32 GMT
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
	-	`sha256:7342031318accab10946b43b34804e02f1e0c107a6af3af5a4ebb766152ee509`  
		Last Modified: Mon, 02 Aug 2021 21:11:42 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648b6a3dac4889e5f68f30776a664fe9d62256592f37d6d2912163da56f265fa`  
		Last Modified: Mon, 02 Aug 2021 21:12:04 GMT  
		Size: 55.2 MB (55235555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5a29c2452fcab6625565bca85ff5fccfbee37e09b6f1e8455655c2735c166a`  
		Last Modified: Mon, 02 Aug 2021 21:11:38 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cac694ac7078f02298b587000698d84cb3bb69637d30c724bd0bcac087c22f41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **190.1 MB (190115136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3187fd285a60bd484a8586f3ee1dc8896c0c94e433a102025bf0dae4c344c1b7`
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
# Tue, 03 Aug 2021 00:00:45 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 03 Aug 2021 00:00:45 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 03 Aug 2021 00:00:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 03 Aug 2021 00:06:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 03 Aug 2021 00:06:06 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 03 Aug 2021 00:06:07 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 03 Aug 2021 00:06:07 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 03 Aug 2021 00:06:08 GMT
EXPOSE 3000
# Tue, 03 Aug 2021 00:06:08 GMT
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
	-	`sha256:fc2c8055fd9194f59346984cbb7941b37a40023edc25ab3dec3e42e9b8c01287`  
		Last Modified: Tue, 03 Aug 2021 00:12:46 GMT  
		Size: 3.1 MB (3061917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836246f3dcf57e23a39d002b3b9d9a09fedb40b5b6accc7268b28ae167eca128`  
		Last Modified: Tue, 03 Aug 2021 00:13:05 GMT  
		Size: 55.1 MB (55073644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63001a72a77f002e6a9f105ba97f4e5cb147287597ca1e71c8670c6b0e768390`  
		Last Modified: Tue, 03 Aug 2021 00:12:42 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:168d7ed49573c2aaecf2d0d8adcc21280d9e2c18dc1ddb19848393c9847211e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **203.2 MB (203243298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a980ba1133cf226e557df7c34d75d5c5e7bfb359db4c611a013f2dd737ac6dc4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:31 GMT
ADD file:a62249c8d6f38120ba61478f35ce3cc947234ac504859ced66532a60de786609 in / 
# Tue, 17 Aug 2021 01:46:31 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:11:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:11:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:11:11 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:18:12 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:20:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:20:12 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:12 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:20:12 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:20:13 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:20:13 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 14:17:02 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 14:17:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 14:17:25 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 14:17:26 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 14:17:26 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 14:17:26 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 14:17:27 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 14:17:27 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 14:17:35 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 14:19:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 14:19:47 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 14:19:47 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 14:19:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 14:19:48 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 14:19:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:64ac1a72c06aa20e6c3b2e37ce66ddf902187eb683a427a477895f158a930e31`  
		Last Modified: Tue, 17 Aug 2021 01:54:22 GMT  
		Size: 25.9 MB (25915072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025ab80b058f00336b15786a8d20ce50706c5277560dc1ddb487b7e5c9d24b10`  
		Last Modified: Tue, 17 Aug 2021 04:34:12 GMT  
		Size: 11.3 MB (11263042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6eb72cd750a3e09673b73506f2a2ce24b3006d1773293eb65b72c9a2cdf7190`  
		Last Modified: Tue, 17 Aug 2021 04:34:09 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb2cb28558c1dd6c31a020484f10c613185335d6d30e7c7a81d3e6ffd0f374f0`  
		Last Modified: Tue, 17 Aug 2021 04:35:35 GMT  
		Size: 14.4 MB (14356587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49391d2e67bfbf4fd993b49c9be1225f0a09d4177c605548f82d49cbcfe78b99`  
		Last Modified: Tue, 17 Aug 2021 04:35:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9307e85455464623a9445ee9314b11fd777c561cefed9b38e6f9067bd30653a`  
		Last Modified: Tue, 17 Aug 2021 14:26:18 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba598bababc240a9c29cf82ac1a0b01837945e37b3cb2b17a3a55ba776227b76`  
		Last Modified: Tue, 17 Aug 2021 14:26:34 GMT  
		Size: 92.6 MB (92611086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dc88258ae8d8cf36219a3b41b130d1e21bf4c2dfb6e1cf9c3f6b3ae2395817`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41c9b592ea00c036970d3b4b7baf687de5e9394670884daa30890ab191cfe5bb`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e8230053e3f65d96319f5f2351fc906de79749654a83811bf21ea7b34f3bee`  
		Last Modified: Tue, 17 Aug 2021 14:26:17 GMT  
		Size: 3.1 MB (3061920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe117b5c157b62194a629b77cf9c9b15c6821516a74c96470c098adba14546ba`  
		Last Modified: Tue, 17 Aug 2021 14:26:22 GMT  
		Size: 56.0 MB (56031346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff9fc675e51cbab5a7a0574bbd10f6ebdc614381aa4a451a98f5884e386b455`  
		Last Modified: Tue, 17 Aug 2021 14:26:16 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:8b2bacb3a529c3a9da30411ee264532f973e5f07226b10f40cca6d31db43a621
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.1 MB (202125065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20cd127add6f4bd712d08c14e2b3a570aa6216ac3e81f7498d128b38ad693d1f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:41:16 GMT
ADD file:0418032b55cd0a6dd515ac277fb9f92354397503cab212d446d3a3d8c647a60f in / 
# Tue, 17 Aug 2021 01:41:17 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:26:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:26:09 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 07:26:09 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 07:43:14 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 07:43:14 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 07:43:15 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 07:46:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 07:46:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 07:46:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 07:46:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 07:46:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 07:46:43 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 20:44:09 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 20:44:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 20:44:42 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 20:44:42 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 20:44:42 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 20:44:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 20:44:43 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 20:44:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 20:44:48 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 20:45:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 20:45:39 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 20:45:39 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 20:45:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 20:45:39 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 20:45:40 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c1c94e1f2523d69effaa463d64fc9962cfc67e2a956f0476c94200e7cf19edf0`  
		Last Modified: Tue, 17 Aug 2021 01:50:57 GMT  
		Size: 27.8 MB (27797627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7c2f28f15bebb2e6e5879bcd2a3c085881fda52f32380a12c8a0248d474ff`  
		Last Modified: Tue, 17 Aug 2021 08:14:57 GMT  
		Size: 17.2 MB (17227368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd3eff60b8a459154279d9ea96f6e521d033e44faf88a091ecf6aef5ebd4888`  
		Last Modified: Tue, 17 Aug 2021 08:14:49 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4d6e92558e2e9952c84a3effe46c647bb2ec5c677559440a30b3472898d5ca2`  
		Last Modified: Tue, 17 Aug 2021 08:16:53 GMT  
		Size: 14.0 MB (13992678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149425e111bee81e3749bcd1a01f973bdea53d5107f36b0ce5ab6f24a5d26bd0`  
		Last Modified: Tue, 17 Aug 2021 08:16:50 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba2aa95ab76e668ab9334a63f10abb5c9cc72b5ce42c0288b8e258d2421de4c`  
		Last Modified: Tue, 17 Aug 2021 20:50:52 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75e3c06b49e4b7fdda9acea36456b2c0c69f0f52f0d50724e55b0f5cdc42ce93`  
		Last Modified: Tue, 17 Aug 2021 20:51:14 GMT  
		Size: 95.7 MB (95702973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d658498d2e116af9d55f933669635cd567034d03d7c862e5be6b2affa43ef371`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d6e976830ca03935c308924157582258b4599ff1a78443efeef21cc6e0c4e5`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db706ca27afe38d047ff274c96b1d95fc75f4512bfd5967afd3854127d17087d`  
		Last Modified: Tue, 17 Aug 2021 20:50:51 GMT  
		Size: 3.1 MB (3061919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1417c9a42064182a2e270bd603d1fa078906a8999616843228fd988741802494`  
		Last Modified: Tue, 17 Aug 2021 20:50:58 GMT  
		Size: 44.3 MB (44338264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eed6830dcebdb2ec5236d072e5b78c805b2ad7749fa0de197a129adb76a2abf`  
		Last Modified: Tue, 17 Aug 2021 20:50:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:ecdb00827fcf83f2f12c122af3ffc2420a6faa270cd7b048c9756f927f7c77fa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **219.7 MB (219650618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57391c1536ff89c22d27544dc68890a924a8d455796c92bdc28721108b71a53c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 22 Jul 2021 00:19:04 GMT
ADD file:3a6bd6ce3eff98b88a13de5d0f26cff0b026f876674204dbad6f84fafcf145b1 in / 
# Thu, 22 Jul 2021 00:19:13 GMT
CMD ["bash"]
# Fri, 23 Jul 2021 00:32:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 00:33:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 23 Jul 2021 00:33:06 GMT
ENV LANG=C.UTF-8
# Fri, 23 Jul 2021 00:52:18 GMT
ENV RUBY_MAJOR=2.7
# Fri, 23 Jul 2021 00:52:28 GMT
ENV RUBY_VERSION=2.7.4
# Fri, 23 Jul 2021 00:52:37 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Fri, 23 Jul 2021 01:01:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 23 Jul 2021 01:01:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 23 Jul 2021 01:01:41 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 23 Jul 2021 01:01:45 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 23 Jul 2021 01:01:53 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 23 Jul 2021 01:01:58 GMT
CMD ["irb"]
# Sat, 24 Jul 2021 02:42:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 24 Jul 2021 02:46:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 24 Jul 2021 02:46:14 GMT
ENV RAILS_ENV=production
# Sat, 24 Jul 2021 02:46:17 GMT
WORKDIR /usr/src/redmine
# Sat, 24 Jul 2021 02:46:19 GMT
ENV HOME=/home/redmine
# Sat, 24 Jul 2021 02:46:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 02 Aug 2021 23:16:59 GMT
ENV REDMINE_VERSION=4.2.2
# Mon, 02 Aug 2021 23:17:01 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Mon, 02 Aug 2021 23:17:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 02 Aug 2021 23:23:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 02 Aug 2021 23:23:26 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 02 Aug 2021 23:23:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Mon, 02 Aug 2021 23:23:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 02 Aug 2021 23:23:37 GMT
EXPOSE 3000
# Mon, 02 Aug 2021 23:23:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1130517d52da84a09f9465006bddab5e49afd398860890eab6274fd0bff32371`  
		Last Modified: Thu, 22 Jul 2021 00:27:49 GMT  
		Size: 30.6 MB (30553709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f17b372a9c9122b881c2d22680e91d78ef4c329094595c61f5acb2523f41b7`  
		Last Modified: Fri, 23 Jul 2021 01:35:00 GMT  
		Size: 12.7 MB (12704330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064c16cae6894266abd8c9d33cfb671a4ebb2705d8b8bb7495bafc50c3dcd344`  
		Last Modified: Fri, 23 Jul 2021 01:34:57 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76d2032e7e646d23109ea1a55abb581c169350b85836914155a6837d64eb757`  
		Last Modified: Fri, 23 Jul 2021 01:36:48 GMT  
		Size: 15.0 MB (14997545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f996a3088f8cd5e20b9f19c3aebdd4a6228a85b6c0a83f9dde8e2a5ec82976d3`  
		Last Modified: Fri, 23 Jul 2021 01:36:46 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acdc172d0fc27092df5794b7a17e2c42e7f2497e85086076f490e273db428fe`  
		Last Modified: Sat, 24 Jul 2021 03:36:05 GMT  
		Size: 1.8 KB (1754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe4ded3f0db610cc9dca87e98b2305c850cbaf595886ccb44e3492ad727b18`  
		Last Modified: Sat, 24 Jul 2021 03:36:28 GMT  
		Size: 101.3 MB (101327533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14617640fcda340a6bc04fd1c65d4183ad0dd01a4e3b44fb313d164071471e95`  
		Last Modified: Sat, 24 Jul 2021 03:36:01 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1b361a5633d0ca044cc644bddc99329645edadfff1cbb48e966deb9b0d079a`  
		Last Modified: Sat, 24 Jul 2021 03:36:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bfbd857622d0239bfa521d75318f40925e9e4608a62a4be7abc2bc89801ec3`  
		Last Modified: Mon, 02 Aug 2021 23:30:32 GMT  
		Size: 3.1 MB (3061921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e4b836dd92fc0980e6e61a697cc881ceb76ca811af742788283ab3211698e1`  
		Last Modified: Mon, 02 Aug 2021 23:30:38 GMT  
		Size: 57.0 MB (57001331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2976222796409af9d080f03664b07bc2a177c8b37d29e7937c0620ba5f908d03`  
		Last Modified: Mon, 02 Aug 2021 23:30:31 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:33d5a2369e443a1bb092e9da696586fae6988113fc4ef99bf98b5af5e03135f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **202.6 MB (202554693 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36f13509159fb8e3ef52d7620d4ef325ebe2d7a388fec2faf172536b64ee9ae9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 17 Aug 2021 01:49:55 GMT
ADD file:f99acf07eb8c42cc90080a195bbcdb18850a1d7a333b385d5d8ebe31c9e9f783 in / 
# Tue, 17 Aug 2021 01:49:59 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 04:21:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 04:21:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 17 Aug 2021 04:21:08 GMT
ENV LANG=C.UTF-8
# Tue, 17 Aug 2021 04:37:51 GMT
ENV RUBY_MAJOR=2.7
# Tue, 17 Aug 2021 04:37:51 GMT
ENV RUBY_VERSION=2.7.4
# Tue, 17 Aug 2021 04:37:52 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Tue, 17 Aug 2021 04:40:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 17 Aug 2021 04:40:20 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 17 Aug 2021 04:40:21 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 17 Aug 2021 04:40:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 17 Aug 2021 04:40:23 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 17 Aug 2021 04:40:24 GMT
CMD ["irb"]
# Tue, 17 Aug 2021 13:32:53 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 17 Aug 2021 13:33:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 13:33:28 GMT
ENV RAILS_ENV=production
# Tue, 17 Aug 2021 13:33:28 GMT
WORKDIR /usr/src/redmine
# Tue, 17 Aug 2021 13:33:28 GMT
ENV HOME=/home/redmine
# Tue, 17 Aug 2021 13:33:29 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 17 Aug 2021 13:33:29 GMT
ENV REDMINE_VERSION=4.2.2
# Tue, 17 Aug 2021 13:33:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=e6fbe9279939a95953d377ef76f180f204a1f3da5229a1d56055d658de7198f6
# Tue, 17 Aug 2021 13:33:32 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 17 Aug 2021 13:35:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 17 Aug 2021 13:35:38 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 17 Aug 2021 13:35:38 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Tue, 17 Aug 2021 13:35:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 17 Aug 2021 13:35:39 GMT
EXPOSE 3000
# Tue, 17 Aug 2021 13:35:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:ed4fb22ab70391b36e4b9f97e34387c33652dc2b91b5f0c7ef4ada070bfd32c3`  
		Last Modified: Tue, 17 Aug 2021 01:58:12 GMT  
		Size: 25.8 MB (25760856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c03f413a15f7a98caaa2b027613636c576e3d98d8e1a98805c5978f2cc985f`  
		Last Modified: Tue, 17 Aug 2021 05:03:55 GMT  
		Size: 10.8 MB (10814401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ded0951dc51ddc1b38edf558277fec87d4169c1607312f67af2c4ffb9c4f19`  
		Last Modified: Tue, 17 Aug 2021 05:03:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d49ef1e1c8f0247bfa63924e738fc94dc0c4a81ec0e4b2b73df09f08d080005`  
		Last Modified: Tue, 17 Aug 2021 05:04:49 GMT  
		Size: 14.7 MB (14697415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54919ecbd2a42d851761e24bb9a1e9e71346c6ecd753a4c6b7868679823367b`  
		Last Modified: Tue, 17 Aug 2021 05:04:47 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c159f1e20f87d626bb303eea037968c316700fdd1fd9fa734e8ebacf14608ab2`  
		Last Modified: Tue, 17 Aug 2021 13:42:11 GMT  
		Size: 1.7 KB (1748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223675cd45b3e6a43e45f6ad1a699c278dc5effe72583bec3657746c84a2a692`  
		Last Modified: Tue, 17 Aug 2021 13:42:24 GMT  
		Size: 91.8 MB (91792621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21f55e74adea5c6a7d4c0be869fe00b2451a51e188e2c0e1466d72eaad06cc9d`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cd2e454b71a3aea72543018a9596e611b94ee88301b3d5971854daab02981`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b885ccd7ef756fbf397809a3541c6cadba886972a35c3f9d9d00cc920b16ef2`  
		Last Modified: Tue, 17 Aug 2021 13:42:11 GMT  
		Size: 3.1 MB (3061920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde4808141553382cd3c73078af6ba86889e806ed72c6251287678fbce48b5ea`  
		Last Modified: Tue, 17 Aug 2021 13:42:15 GMT  
		Size: 56.4 MB (56423232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed18e7c147f9b19d7cb774a6462749d36a61882e80d34fff6912e4ed7990252d`  
		Last Modified: Tue, 17 Aug 2021 13:42:10 GMT  
		Size: 1.8 KB (1797 bytes)  
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
