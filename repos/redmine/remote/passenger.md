## `redmine:passenger`

```console
$ docker pull redmine@sha256:da5f6136fe680d5f400da5971748a6fab8852ad779211ab8ddbe838c8a55c6b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:9eae305ba3e1a41818756224ffebae3443a6eb8b8e8437eeb2cd79073eaa926a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.6 MB (235630644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee12ab1c811dc283577380a581ed62cf4f771b59af6e630b472cb25538420dd0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 12 May 2021 01:21:22 GMT
ADD file:7362e0e50f30ff45463ea38bb265cb8f6b7cd422eb2d09de7384efa0b59614be in / 
# Wed, 12 May 2021 01:21:22 GMT
CMD ["bash"]
# Wed, 12 May 2021 17:34:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 17:34:28 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 12 May 2021 17:34:28 GMT
ENV LANG=C.UTF-8
# Wed, 12 May 2021 17:42:04 GMT
ENV RUBY_MAJOR=2.7
# Wed, 12 May 2021 17:42:04 GMT
ENV RUBY_VERSION=2.7.3
# Wed, 12 May 2021 17:42:04 GMT
ENV RUBY_DOWNLOAD_SHA256=5e91d1650857d43cd6852e05ac54683351e9c301811ee0bef43a67c4605e7db1
# Wed, 12 May 2021 17:46:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 12 May 2021 17:46:18 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 12 May 2021 17:46:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 12 May 2021 17:46:19 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 12 May 2021 17:46:21 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 12 May 2021 17:46:21 GMT
CMD ["irb"]
# Thu, 13 May 2021 08:23:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 13 May 2021 08:24:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 13 May 2021 08:24:22 GMT
ENV RAILS_ENV=production
# Thu, 13 May 2021 08:24:22 GMT
WORKDIR /usr/src/redmine
# Thu, 13 May 2021 08:24:22 GMT
ENV HOME=/home/redmine
# Thu, 13 May 2021 08:24:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 13 May 2021 08:24:24 GMT
ENV REDMINE_VERSION=4.2.1
# Thu, 13 May 2021 08:24:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Thu, 13 May 2021 08:24:28 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 13 May 2021 08:25:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 13 May 2021 08:25:12 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 13 May 2021 08:25:12 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 13 May 2021 08:25:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 13 May 2021 08:25:13 GMT
EXPOSE 3000
# Thu, 13 May 2021 08:25:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Thu, 13 May 2021 08:25:20 GMT
ENV PASSENGER_VERSION=6.0.8
# Thu, 13 May 2021 08:25:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 13 May 2021 08:25:38 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Thu, 13 May 2021 08:25:39 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Thu, 13 May 2021 08:25:39 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:69692152171afee1fd341febc390747cfca2ff302f2881d8b394e786af605696`  
		Last Modified: Wed, 12 May 2021 01:27:20 GMT  
		Size: 27.1 MB (27145915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a1f774fea417076a75fe5a4e72de3c898b7208ea6e711495b40cbd6be770a14`  
		Last Modified: Wed, 12 May 2021 18:18:14 GMT  
		Size: 12.6 MB (12562350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b32b9ebaa42aaafd63deb47d7e37672fa1f7a77b5e5a969df2680616c498f7c`  
		Last Modified: Wed, 12 May 2021 18:18:11 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8115e4beca50998c01315e217f89c9c4338e865916a10f8ca7494aedc188f227`  
		Last Modified: Wed, 12 May 2021 18:19:12 GMT  
		Size: 22.9 MB (22887254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6fc87221cc8d0adafd04956ff2adf163818030a64fa2b82f3c55e824de586c1`  
		Last Modified: Wed, 12 May 2021 18:19:10 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecc3ffdf342d51d37eee2a03bd765f018cac193db66b10339aa233d8cedef1e`  
		Last Modified: Thu, 13 May 2021 08:30:51 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c0766a9fc7f5452751dd2670b3d0ebbc40f2f5b97da06a67849d5592a2e8752`  
		Last Modified: Thu, 13 May 2021 08:31:06 GMT  
		Size: 94.1 MB (94090231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9a5ea49a972a19b90d04d7c4a3e62d4fe3b1926443a03361d24e92b840772e`  
		Last Modified: Thu, 13 May 2021 08:30:49 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4aa5d089efddda4830028d9292239ee59e24d0862257d74f7e9c84a8c924ab`  
		Last Modified: Thu, 13 May 2021 08:30:49 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76af3ce3b4e95d64ef9a531d13ccd90540a377abe63f719f2a2069a589f95bfa`  
		Last Modified: Thu, 13 May 2021 08:30:50 GMT  
		Size: 3.1 MB (3058683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:996a27fc010da8a2d4718c70b1704f0bb8f8d7c662cf4e5131cb9ca312caa222`  
		Last Modified: Thu, 13 May 2021 08:30:55 GMT  
		Size: 50.6 MB (50582604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343439c2257c401930fad20bd748c1008a927dc9dc6a53b1ff1d8dd5dd3beaf2`  
		Last Modified: Thu, 13 May 2021 08:30:49 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71263b0319af9242861b0e6ae0969c4a84eae69b7b6eb0eb452cc3989a12f15`  
		Last Modified: Thu, 13 May 2021 08:31:27 GMT  
		Size: 20.4 MB (20362647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560d4007c0e1fb96a4496478a6889b106c2fbd4aa366bfd2c32482defb64904a`  
		Last Modified: Thu, 13 May 2021 08:31:25 GMT  
		Size: 4.9 MB (4936715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
