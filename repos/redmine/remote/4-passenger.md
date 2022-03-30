## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:565e859332667790cf53cc1d26a94d4d751df862dbb0747518690dd9d630e1b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:2062a1d50f390031d3404d9df5068dcb379f09c4ef0d8751ff8922c70296f90d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (231047959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc3ca18d727d81af42e8da37c1712792077b2af0f164085861a011298f99aeb3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:18 GMT
ADD file:966d3669b40f5fbaecee1ecbeb58debe19001076da5d94717080d55efbc25971 in / 
# Tue, 29 Mar 2022 00:22:19 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 10:28:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 10:28:51 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 29 Mar 2022 10:28:51 GMT
ENV LANG=C.UTF-8
# Tue, 29 Mar 2022 10:56:25 GMT
ENV RUBY_MAJOR=2.7
# Tue, 29 Mar 2022 10:56:25 GMT
ENV RUBY_VERSION=2.7.5
# Tue, 29 Mar 2022 10:56:25 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Tue, 29 Mar 2022 10:58:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 29 Mar 2022 10:58:39 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 29 Mar 2022 10:58:39 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 29 Mar 2022 10:58:40 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:58:40 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 29 Mar 2022 10:58:40 GMT
CMD ["irb"]
# Wed, 30 Mar 2022 13:09:45 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 30 Mar 2022 13:10:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 13:10:10 GMT
ENV RAILS_ENV=production
# Wed, 30 Mar 2022 13:10:10 GMT
WORKDIR /usr/src/redmine
# Wed, 30 Mar 2022 13:10:10 GMT
ENV HOME=/home/redmine
# Wed, 30 Mar 2022 13:10:10 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 30 Mar 2022 13:10:10 GMT
ENV REDMINE_VERSION=4.2.5
# Wed, 30 Mar 2022 13:10:11 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Wed, 30 Mar 2022 13:10:11 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Wed, 30 Mar 2022 13:10:13 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 30 Mar 2022 13:10:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 30 Mar 2022 13:10:57 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 30 Mar 2022 13:10:57 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 30 Mar 2022 13:10:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 30 Mar 2022 13:10:57 GMT
EXPOSE 3000
# Wed, 30 Mar 2022 13:10:57 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 30 Mar 2022 13:11:07 GMT
ENV PASSENGER_VERSION=6.0.12
# Wed, 30 Mar 2022 13:11:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 30 Mar 2022 13:11:25 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 30 Mar 2022 13:11:26 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 30 Mar 2022 13:11:26 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:c229119241af7b23b121052a1cae4c03e0a477a72ea6a7f463ad7623ff8f274b`  
		Last Modified: Tue, 29 Mar 2022 00:27:16 GMT  
		Size: 31.4 MB (31378457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c14a196c62ee705bf37cfab91ea1d171f7b636ffd65269877b758f726189872e`  
		Last Modified: Tue, 29 Mar 2022 11:19:01 GMT  
		Size: 10.0 MB (9990916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365bbf24384cc62b2e96112071ead0fb9d34bb8f42158306d2b628b641fc0068`  
		Last Modified: Tue, 29 Mar 2022 11:18:59 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c8e5ac1ab836c79588b46fd4dada30f9549cda829483d85d263eb41cc30e3f`  
		Last Modified: Tue, 29 Mar 2022 11:21:31 GMT  
		Size: 14.6 MB (14580588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3950ef24b9c6d1f46c1a9399378746b41818e25e7843e659690bdf217d717b83`  
		Last Modified: Tue, 29 Mar 2022 11:21:29 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223868cc38e81c703135f56f4b7556cbd22667dc11c3f8c41a668fa0d49700a2`  
		Last Modified: Wed, 30 Mar 2022 13:20:44 GMT  
		Size: 1.7 KB (1746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7441c4e405f6070bcb37810210101e744146e8cde60fb181f006a78ab72dd7b5`  
		Last Modified: Wed, 30 Mar 2022 13:20:59 GMT  
		Size: 102.0 MB (101987455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cc672d77fe91d18da554f24dc37fe7cf7efb5468522ee609190001f4f4eb78`  
		Last Modified: Wed, 30 Mar 2022 13:20:41 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:911aef45251bcf86ce5784107a75808f98f8dd7d495b83ce4d897e6fb8a6fe19`  
		Last Modified: Wed, 30 Mar 2022 13:20:41 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55af035b90c108ec6df11815724caedd9d1b73340c2f8f526493f012e263d260`  
		Last Modified: Wed, 30 Mar 2022 13:20:42 GMT  
		Size: 3.1 MB (3064892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad60e0fa3e2e3c8440f7af717002ce9402a642862b518565fe136cda6e41a7b5`  
		Last Modified: Wed, 30 Mar 2022 13:20:47 GMT  
		Size: 43.9 MB (43884847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f8b09c8a14753d1bdcee619101ce5f2a55865995727f931b120bc5db8845ab`  
		Last Modified: Wed, 30 Mar 2022 13:20:42 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1465051b5e7aaa1f0dfe05438d66ebd111f18c82b225e7ed2105f3f8435536cc`  
		Last Modified: Wed, 30 Mar 2022 13:21:24 GMT  
		Size: 21.2 MB (21231920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d7156449c187314ef9a6ae91aa55036c0ad54d543c4da50f30988f90a397321`  
		Last Modified: Wed, 30 Mar 2022 13:21:23 GMT  
		Size: 4.9 MB (4924637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
