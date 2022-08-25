## `redmine:latest`

```console
$ docker pull redmine@sha256:6faa349030d73a7342e92b43c287af567c4bac2d2400f602b6e07ddb57e57c53
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
$ docker pull redmine@sha256:4ddd035bb6eb71b0e0067aa662829e12bde432e55c5fa2e4be892f29bce333cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **237.1 MB (237136741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1de550a9ed5bdb5e1ee6d1eef978377bb26909f6bb4e4e4b5d4e20a85221f9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:22:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:22:33 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 11:22:33 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:32:17 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 Aug 2022 11:32:17 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 23 Aug 2022 11:32:17 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 23 Aug 2022 11:34:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 11:34:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 11:34:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 11:34:42 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:34:43 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 11:34:43 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 21:42:15 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 21:42:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:42:42 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 21:42:42 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 21:42:42 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 21:42:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 21:42:43 GMT
ENV REDMINE_VERSION=5.0.2
# Tue, 23 Aug 2022 21:42:43 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Tue, 23 Aug 2022 21:42:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Tue, 23 Aug 2022 21:42:46 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 21:43:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 21:43:17 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 21:43:18 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 21:43:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:43:18 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 21:43:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacae54ed9573db0b30f6991a5f5fd01a86a6f9d946f16e68df339e1f0837d12`  
		Last Modified: Tue, 23 Aug 2022 11:57:55 GMT  
		Size: 10.0 MB (9992553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc5a66b4b23b1b64c5ac2bf68f7b4d8de90c00d75eff7ae0edb392b9de1d969`  
		Last Modified: Tue, 23 Aug 2022 11:57:53 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bfdd5db1cd0d6bd990cc610608e73c780e9c54d6fe16884a83783b37d437d0`  
		Last Modified: Tue, 23 Aug 2022 11:59:08 GMT  
		Size: 32.4 MB (32436216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8a58a8f52991a119f728ca12fb996cda84c69f85eae1c6800cc36b368b5464`  
		Last Modified: Tue, 23 Aug 2022 11:59:05 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a816b83e80f19a5ca554f1fca881425218b97ffe91f6c9a168a153523b7f20`  
		Last Modified: Tue, 23 Aug 2022 21:45:46 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7545bbcfe27880c5e99bffa19837b99a8b0f13c1300388eb9b4dffe984e3c9ce`  
		Last Modified: Tue, 23 Aug 2022 21:46:02 GMT  
		Size: 102.0 MB (102021142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3facd9ba94b59a9011c0b3bfd8c7cb14dc11f726377fe882415ad0ecbb77f073`  
		Last Modified: Tue, 23 Aug 2022 21:45:44 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526d54f4d7d2c191978a5823b1d31447f063afc086b4a08ea228b1fdc458057b`  
		Last Modified: Tue, 23 Aug 2022 21:45:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53aa158f731452270fa7e65e5bc47ce04e935339ba9f4259512a54c2edaaf975`  
		Last Modified: Tue, 23 Aug 2022 21:45:45 GMT  
		Size: 3.1 MB (3129372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4f19da05f8cfb195396643d4cb5a9de4dba9ccbff2c3d463d50c9a72ec9507`  
		Last Modified: Tue, 23 Aug 2022 21:45:51 GMT  
		Size: 58.2 MB (58171668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af589970812458d34eb64a816c88913a4b8f06c724e0adeb1fb500752bf746d`  
		Last Modified: Tue, 23 Aug 2022 21:45:44 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:1871cbe1c78c2211b78d6b8cebd1cc827143269dd0c7cafb359f434ce2cf9ed9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.9 MB (236923305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:360ce0c0910d8e28365eab2a4436e8580f77f843e4722fec851d1aab6e1d6f55`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:14 GMT
ADD file:83fb076a50e935419eb0db2bd97477d7ed5f16aaac4c8cc35a4a69ac612df327 in / 
# Tue, 23 Aug 2022 01:17:14 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:58:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:58:53 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 11:58:53 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 12:09:57 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 Aug 2022 12:09:57 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 23 Aug 2022 12:09:58 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 23 Aug 2022 12:15:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 12:15:34 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 12:15:34 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 12:15:34 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 12:15:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 12:15:35 GMT
CMD ["irb"]
# Wed, 24 Aug 2022 01:21:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 24 Aug 2022 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 01:21:41 GMT
ENV RAILS_ENV=production
# Wed, 24 Aug 2022 01:21:41 GMT
WORKDIR /usr/src/redmine
# Wed, 24 Aug 2022 01:21:41 GMT
ENV HOME=/home/redmine
# Wed, 24 Aug 2022 01:21:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 24 Aug 2022 01:21:41 GMT
ENV REDMINE_VERSION=5.0.2
# Wed, 24 Aug 2022 01:21:41 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Wed, 24 Aug 2022 01:21:41 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Wed, 24 Aug 2022 01:21:45 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 24 Aug 2022 01:24:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 24 Aug 2022 01:24:10 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 24 Aug 2022 01:24:11 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Wed, 24 Aug 2022 01:24:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 24 Aug 2022 01:24:11 GMT
EXPOSE 3000
# Wed, 24 Aug 2022 01:24:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:74eb5afab626122970f8620ac001fcc4a200725acb05519b85aba47a38bf1016`  
		Last Modified: Tue, 23 Aug 2022 01:22:44 GMT  
		Size: 28.9 MB (28917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f98527654c0f97c71fec685c51d227394a931bd5ca18cee85555653d96680a`  
		Last Modified: Tue, 23 Aug 2022 12:37:42 GMT  
		Size: 8.6 MB (8634282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e6261cab4f885273b0bdc7d23546f8b164451b58fca7a1aa43c9fe3b92a236`  
		Last Modified: Tue, 23 Aug 2022 12:37:38 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63afb21d0242354d715882a342a0130ea3324425110eb79d8d8140cc006321fd`  
		Last Modified: Tue, 23 Aug 2022 12:38:51 GMT  
		Size: 31.0 MB (30985236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27d34531e1076d220bcc6a9a1588520a0fb94856f493f8b542aacc58f4ce25b1`  
		Last Modified: Tue, 23 Aug 2022 12:38:45 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bbbc3c731281f6292b2ac5d180747aeac7ba684a839d22abe688bba0d34461`  
		Last Modified: Wed, 24 Aug 2022 01:28:24 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599bc59517935a276cedcd2a494ea01ec4158d5d7e7cc027c51e99f4e76acfb1`  
		Last Modified: Wed, 24 Aug 2022 01:28:48 GMT  
		Size: 97.0 MB (96990726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d234980a4d5dfdb50454b4561a2f338b0d400268279628c1d2237c78ca5bac6`  
		Last Modified: Wed, 24 Aug 2022 01:28:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2280b941a4725810e87804dab77d33dfa8c53291a4fe9cb0f0232c2692037974`  
		Last Modified: Wed, 24 Aug 2022 01:28:21 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71aeb4da0cfcf436009bd8e8502330eea772882b635fdc79404fa907779b41c6`  
		Last Modified: Wed, 24 Aug 2022 01:28:23 GMT  
		Size: 3.1 MB (3129363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d9334f7fab0d693ae5cf36d4ccb1e36a731452b78d1daaaadb3a7a965a723d`  
		Last Modified: Wed, 24 Aug 2022 01:28:34 GMT  
		Size: 68.3 MB (68262153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7014713e6d6eb829f8595d27efff94becbcc8232090102d6fd6097d31720adc2`  
		Last Modified: Wed, 24 Aug 2022 01:28:21 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:c1b66077a71681d3a3aaffafb208be64a00e66b614faf47717ca9fe41e1e502a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.8 MB (229806094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dc9b46c6dff3c470ca93403903ea10b1b2ff1dfc3bac2d7ca50018fed84edb4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:43:01 GMT
ADD file:4cd1b4287674228db28402a76aa4f241740585448be48b5b15068d275ee9eb84 in / 
# Tue, 23 Aug 2022 01:43:01 GMT
CMD ["bash"]
# Wed, 24 Aug 2022 13:36:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 13:36:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 24 Aug 2022 13:36:15 GMT
ENV LANG=C.UTF-8
# Wed, 24 Aug 2022 13:51:13 GMT
ENV RUBY_MAJOR=3.1
# Wed, 24 Aug 2022 13:51:13 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 24 Aug 2022 13:51:13 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 24 Aug 2022 13:54:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 24 Aug 2022 13:54:49 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 24 Aug 2022 13:54:49 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 24 Aug 2022 13:54:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 24 Aug 2022 13:54:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 24 Aug 2022 13:54:49 GMT
CMD ["irb"]
# Thu, 25 Aug 2022 12:32:58 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 25 Aug 2022 12:33:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 25 Aug 2022 12:33:39 GMT
ENV RAILS_ENV=production
# Thu, 25 Aug 2022 12:33:39 GMT
WORKDIR /usr/src/redmine
# Thu, 25 Aug 2022 12:33:39 GMT
ENV HOME=/home/redmine
# Thu, 25 Aug 2022 12:33:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 25 Aug 2022 12:33:40 GMT
ENV REDMINE_VERSION=5.0.2
# Thu, 25 Aug 2022 12:33:40 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Thu, 25 Aug 2022 12:33:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Thu, 25 Aug 2022 12:33:45 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 25 Aug 2022 12:36:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 25 Aug 2022 12:36:25 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 25 Aug 2022 12:36:25 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Thu, 25 Aug 2022 12:36:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 25 Aug 2022 12:36:25 GMT
EXPOSE 3000
# Thu, 25 Aug 2022 12:36:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:051ba72559abd0cf65b34b75605580f58636ec3cb994f97de317632a85d82761`  
		Last Modified: Tue, 23 Aug 2022 01:50:05 GMT  
		Size: 26.6 MB (26571732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b939aeabdac58fed26289eddd6831a56e2a2311739a2f8f65eb1a125da1bd4c6`  
		Last Modified: Wed, 24 Aug 2022 14:31:25 GMT  
		Size: 8.1 MB (8144135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc604ffe1810141fcd49ce49f060e1a937aa4aaf063b98fa03839489a433225c`  
		Last Modified: Wed, 24 Aug 2022 14:31:22 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a471d931dd24999cd2e6850727cc9821d1dd11b7226964b1bf810be00236e0b`  
		Last Modified: Wed, 24 Aug 2022 14:33:05 GMT  
		Size: 30.8 MB (30848397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf3cbd0d5b7d2d66cb246663829553f1ecae1080c90f8ae3ece3ad5bc0e1fde`  
		Last Modified: Wed, 24 Aug 2022 14:33:02 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58fcac4b66c7907f95df2ee1403b80d473e8dc7938ff70018bec69cc64ded41`  
		Last Modified: Thu, 25 Aug 2022 12:42:05 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c794b9a3f4bd7d5b84fb4ae880318b398b424a19bbe4895a02c32b49ad05f7de`  
		Last Modified: Thu, 25 Aug 2022 12:42:36 GMT  
		Size: 93.1 MB (93132074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64958afbcf75182a5f37f649a2802dbd57285a890ec519ddcf7acf0a781a76a`  
		Last Modified: Thu, 25 Aug 2022 12:42:01 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454270eabd85ffe8fd90d7a967262d94c5e7e5f7b79224577c2ebbf46638521d`  
		Last Modified: Thu, 25 Aug 2022 12:42:01 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a28b7a58e5e22855e589d5a57516ccf28616543506056c4791a347863c17ead0`  
		Last Modified: Thu, 25 Aug 2022 12:42:05 GMT  
		Size: 3.1 MB (3129355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e2234c54aae27503495aaa48feabf2a413f9320c20d75bb2b2155c0934a3f9`  
		Last Modified: Thu, 25 Aug 2022 12:42:22 GMT  
		Size: 68.0 MB (67976103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebea4fd42331047b50e42b6cf04b5874996315fb1a6d0f4f41cd5ad14ecfc61`  
		Last Modified: Thu, 25 Aug 2022 12:42:02 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:99ed68347ef5ef778a0396196d871f97b2893001923afde9d34e998a42d92bcb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (231004597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b41cdee56df702d11952659dab7c42c45ffec979521c01a1759145b28711b12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:33:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:33:55 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 11:33:55 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 11:43:42 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 Aug 2022 11:43:43 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 23 Aug 2022 11:43:44 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 23 Aug 2022 11:45:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 11:45:54 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 11:45:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 11:45:56 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 11:45:57 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 11:45:58 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 23:17:42 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 23:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 23:18:10 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 23:18:11 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 23:18:12 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 23:18:14 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 23:18:14 GMT
ENV REDMINE_VERSION=5.0.2
# Tue, 23 Aug 2022 23:18:15 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Tue, 23 Aug 2022 23:18:16 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Tue, 23 Aug 2022 23:18:20 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 23:18:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 23:18:51 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 23:18:52 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 23:18:53 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 23:18:54 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 23:18:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6cc3550da36460a5459ebbf17d504b8c97e8e52d83db0359a8512c068d33f74`  
		Last Modified: Tue, 23 Aug 2022 12:10:18 GMT  
		Size: 9.0 MB (9036227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22d74a4c544da03abe5f36f8db322480084242dbceff103cc88b868bdbbdb7d`  
		Last Modified: Tue, 23 Aug 2022 12:10:17 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e854bad6822bdeb30f5c76f306b82536cb0bf6ed9ddfd558c409b120a540c8c`  
		Last Modified: Tue, 23 Aug 2022 12:11:50 GMT  
		Size: 31.6 MB (31589454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df809180b6b95c77d7ec9ff144e4fa5f5a01681a10c98449f2eec58b066bb2a9`  
		Last Modified: Tue, 23 Aug 2022 12:11:47 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91ce9c776b29cc0b7d2eeaee42f93876cdbb15f416cb6ff78dfa0d6586ec578`  
		Last Modified: Tue, 23 Aug 2022 23:21:53 GMT  
		Size: 1.6 KB (1623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13603ff6aabdc63cdf02f8bd6a14909897aeab62f2a1191f9541b39076fe46c1`  
		Last Modified: Tue, 23 Aug 2022 23:22:09 GMT  
		Size: 99.8 MB (99797712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4feb6f2ec8b31786adb6af92b391edf97af7048d22cb8c30e4c7a00201402f42`  
		Last Modified: Tue, 23 Aug 2022 23:21:51 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9c5f607a838e4b429c55ba85abb527eed8b58eea8ae0e6de06162c31795b05`  
		Last Modified: Tue, 23 Aug 2022 23:21:51 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f073dc38279a7d3cb1212eeee2fd73253ed1f904134204fbfe6f396199679711`  
		Last Modified: Tue, 23 Aug 2022 23:21:52 GMT  
		Size: 3.1 MB (3129409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412066b79dffa873acfc0357c78a9aa66a5c68cc7e0bca5eefa5f9d751235d02`  
		Last Modified: Tue, 23 Aug 2022 23:21:58 GMT  
		Size: 57.4 MB (57383916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:563cf697d45f1e99661797686a5f0ed9d009edc9eade7cdd3e814206fdab69a4`  
		Last Modified: Tue, 23 Aug 2022 23:21:51 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:b8f624502560c05cd77a40823042b84d50be8bdb5f7df809543ddd77e937eb27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.8 MB (238810867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:735c03d1e7bd49133044f263d8d660a933aa26c741df11fab8e5a986ba02380c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:02:40 GMT
ADD file:5ca62c98116941aaa64ec72afb689a088c46f75a3e83d5b0d4e58d65ec905ccd in / 
# Tue, 23 Aug 2022 01:02:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 15:22:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 15:22:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 15:22:19 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 15:32:06 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 Aug 2022 15:32:07 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 23 Aug 2022 15:32:08 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 23 Aug 2022 15:34:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 15:34:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 15:34:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 15:34:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 15:34:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 15:34:26 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 21:10:04 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 21:10:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:10:38 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 21:10:38 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 21:10:39 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 21:10:40 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 21:10:41 GMT
ENV REDMINE_VERSION=5.0.2
# Tue, 23 Aug 2022 21:10:42 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Tue, 23 Aug 2022 21:10:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Tue, 23 Aug 2022 21:10:47 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 21:11:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 21:11:23 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 21:11:24 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 21:11:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 21:11:25 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 21:11:26 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6b3cb4a05a891d9d8a87a2bd7247b16f79832a9d4afbad3ff5068f6fc2ba1560`  
		Last Modified: Tue, 23 Aug 2022 01:08:25 GMT  
		Size: 32.4 MB (32387317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3caacbddf1ff01b4681a908bdce5024b6fb9b342cabc00f76935eaa6c7724183`  
		Last Modified: Tue, 23 Aug 2022 16:00:29 GMT  
		Size: 11.8 MB (11789883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adcae00d7ed36ff5bf013ce67b134dee88eb5c11dc76c91340250b01d4cde31`  
		Last Modified: Tue, 23 Aug 2022 16:00:26 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a239527b2ca4d3fdb4c3506bb6758076d12f9640082fabaa19076bb5bd8889e8`  
		Last Modified: Tue, 23 Aug 2022 16:02:34 GMT  
		Size: 30.8 MB (30789175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be39991a379e4510a1e97e89601dbb17b6e49aa245c37aae47d1249a9ccafb4b`  
		Last Modified: Tue, 23 Aug 2022 16:02:30 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2edc88eb2f85eb3124281bb87996e756cf2f4ee0aeedf4f2469d7bf4bc762e0`  
		Last Modified: Tue, 23 Aug 2022 21:14:26 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673c0b9cb91473ae4d14b9d98058625f676d0e6931c4b9cfc25e31d460788062`  
		Last Modified: Tue, 23 Aug 2022 21:14:43 GMT  
		Size: 103.4 MB (103356096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378a5a0b4392f104a05781c93996daadc178d8c0c75f0f1cf6bf14ec76276325`  
		Last Modified: Tue, 23 Aug 2022 21:14:23 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ad5c559de7a79e756c3ea786879201195f9d1c622bfaa9acfe94ff0693f0370`  
		Last Modified: Tue, 23 Aug 2022 21:14:23 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8278a9bdb1931c894ded9929b224fbdf1d20f044f1490a2ae3c486ef7643011`  
		Last Modified: Tue, 23 Aug 2022 21:14:24 GMT  
		Size: 3.1 MB (3129412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e2900ab77e64bdf6e05383986508475ee26a970c95bb25db95d43d17a264e8`  
		Last Modified: Tue, 23 Aug 2022 21:14:34 GMT  
		Size: 57.4 MB (57354901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0112b639bb54791d01f98a4601f3fd1b770b9ae2333d3d51bab57d52bd081b60`  
		Last Modified: Tue, 23 Aug 2022 21:14:23 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:31c23bdf6faf151d24c1779859f0a5b77c18169642d4f92114d0ea3e21503359
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **260.1 MB (260057437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5539c0f6b079b8a1931585399c6d65023696a61d0f5e84afe88540d1a56cc5da`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 01:24:52 GMT
ADD file:d35213360d726a18e220276d33f245115c3e94a321addaa4c9127488368b0203 in / 
# Tue, 23 Aug 2022 01:24:54 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:12:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:12:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 13:12:08 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 13:19:30 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 Aug 2022 13:19:30 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 23 Aug 2022 13:19:31 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 23 Aug 2022 13:23:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 13:23:08 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 13:23:09 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 13:23:09 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 13:23:10 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 13:23:10 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 21:55:48 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 21:56:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:56:50 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 21:56:51 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 21:56:51 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 21:56:52 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 21:56:52 GMT
ENV REDMINE_VERSION=5.0.2
# Tue, 23 Aug 2022 21:56:53 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Tue, 23 Aug 2022 21:56:53 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Tue, 23 Aug 2022 21:56:58 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 22:00:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 22:00:07 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 22:00:07 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 22:00:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 22:00:08 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 22:00:09 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:698954eda09d38dd1ccc9ce777b1f6bc7f7473fc6c4c3eb634acc8d035a42eae`  
		Last Modified: Tue, 23 Aug 2022 01:30:36 GMT  
		Size: 35.3 MB (35284280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fc1d8f5a9f0c95e449312b1ebc8beaafe22f38b7609141d3368efd9efa9221f`  
		Last Modified: Tue, 23 Aug 2022 13:40:20 GMT  
		Size: 10.5 MB (10478166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410ddc095d085f2ed44ac21e69fd3d6d462bf616dfe3a0495655b10802520283`  
		Last Modified: Tue, 23 Aug 2022 13:40:16 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e70babc67f382a14cd47bb33261d0dc1e91f43c9b5fe77e4b1e91fd1683769a`  
		Last Modified: Tue, 23 Aug 2022 13:41:35 GMT  
		Size: 32.6 MB (32600314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb8a481640b6f4656f0a1ed8370a44c2d95b49e82413fdfac32f1df03b88111`  
		Last Modified: Tue, 23 Aug 2022 13:41:30 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec443e5147d71ae629aa28e00d68062a8fb1827c562febe3aaa98e621b31aa6`  
		Last Modified: Tue, 23 Aug 2022 22:06:34 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:425d593356595f97ceb6eb1b25e4571db9b75c963ca6417b650368ca6892a5e2`  
		Last Modified: Tue, 23 Aug 2022 22:07:02 GMT  
		Size: 107.5 MB (107520937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66ef6324374e0ed9ae158fdd4c5850b3f017154909f9ffe6990748150135374a`  
		Last Modified: Tue, 23 Aug 2022 22:06:31 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662327339c3615b9d29f188b7e34a200558e760b4aa3fdf0970b85765e5655b6`  
		Last Modified: Tue, 23 Aug 2022 22:06:31 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1416868608a24bd6846c65149c731665320093730a0dcd40858c0da3a4b888`  
		Last Modified: Tue, 23 Aug 2022 22:06:32 GMT  
		Size: 3.1 MB (3129360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d2b80b1981297ff0c56c65bdde1b44065466d40a146dd2e80c2e8c2611e723`  
		Last Modified: Tue, 23 Aug 2022 22:06:44 GMT  
		Size: 71.0 MB (71040075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83abef5ff2f9ca24406136f44c60f9ae16151bfa42184938d460c5a90ea83b23`  
		Last Modified: Tue, 23 Aug 2022 22:06:31 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:55f8b66d6fae6eb6d59c6fc3ebac8f27251ba75109b8cdb6fae607da71b11407
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **243.7 MB (243656862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ae72cde1a66934d39c6a7c893c00b3f369d148f9f95cd61f313b9530589a451`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:01 GMT
ADD file:7e494cf2e639edf0f0ce27e06887b8488570da37c5fce0a889687622d8cd443e in / 
# Tue, 23 Aug 2022 00:54:03 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 14:20:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 14:20:38 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 23 Aug 2022 14:20:39 GMT
ENV LANG=C.UTF-8
# Tue, 23 Aug 2022 14:25:34 GMT
ENV RUBY_MAJOR=3.1
# Tue, 23 Aug 2022 14:25:34 GMT
ENV RUBY_VERSION=3.1.2
# Tue, 23 Aug 2022 14:25:34 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Tue, 23 Aug 2022 14:27:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 23 Aug 2022 14:27:35 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 23 Aug 2022 14:27:35 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 23 Aug 2022 14:27:35 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 14:27:36 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 23 Aug 2022 14:27:36 GMT
CMD ["irb"]
# Tue, 23 Aug 2022 21:58:47 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 23 Aug 2022 21:59:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:59:36 GMT
ENV RAILS_ENV=production
# Tue, 23 Aug 2022 21:59:36 GMT
WORKDIR /usr/src/redmine
# Tue, 23 Aug 2022 21:59:37 GMT
ENV HOME=/home/redmine
# Tue, 23 Aug 2022 21:59:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 23 Aug 2022 21:59:38 GMT
ENV REDMINE_VERSION=5.0.2
# Tue, 23 Aug 2022 21:59:38 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.2.tar.gz
# Tue, 23 Aug 2022 21:59:38 GMT
ENV REDMINE_DOWNLOAD_SHA256=4e718f44ba33716faf58c8fabf5d5f55b33c93426b7a33a83b5fc1b880585d57
# Tue, 23 Aug 2022 21:59:41 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 23 Aug 2022 22:02:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 23 Aug 2022 22:02:41 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 23 Aug 2022 22:02:41 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 23 Aug 2022 22:02:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 23 Aug 2022 22:02:42 GMT
EXPOSE 3000
# Tue, 23 Aug 2022 22:02:42 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1c2e5a5a3305e50395bba8974e6c201849f83c07fb0ad036111055f59157c7ff`  
		Last Modified: Tue, 23 Aug 2022 01:04:36 GMT  
		Size: 29.7 MB (29650094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e677c697e370a8ab15d79be88b7de50f457ed2649f8b41f560c690bf836cb54`  
		Last Modified: Tue, 23 Aug 2022 14:39:50 GMT  
		Size: 8.9 MB (8861883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d882cb8d7fd78f1a0db12c31ee5670613d37182cb04cd8d99e2b8cce6e67103`  
		Last Modified: Tue, 23 Aug 2022 14:39:50 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f59c2cb6c1dbe50e32e2b8ce242cec947f030641e9e21fba5d3c6e2e8960c3`  
		Last Modified: Tue, 23 Aug 2022 14:40:39 GMT  
		Size: 32.2 MB (32249106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca24c048ec64fdf021b97cad5e5b3a2495cadddf33332301d9775bb0f34ee47`  
		Last Modified: Tue, 23 Aug 2022 14:40:36 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d5650df0777867bfaab2768c7e1d8355b0a50aa512ee0443c3c96ebfa903f5`  
		Last Modified: Tue, 23 Aug 2022 22:09:42 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad2e5465e1a3ce16c18e9cb9f37f66d080aa310db487616beb1255f0d18491`  
		Last Modified: Tue, 23 Aug 2022 22:09:38 GMT  
		Size: 99.1 MB (99149020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b9186fedb1f3e59190a68500434e9c910a2455c6b4e32ac2ce42fffcaaec6`  
		Last Modified: Tue, 23 Aug 2022 22:09:09 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d985fe785a10e183e7e4653c286b75edd1b18da80924636878a8361e59b52f6a`  
		Last Modified: Tue, 23 Aug 2022 22:09:09 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d594ca639f387bb83fdcc74813f1059c32c47e974b5acb2104fddc1902b51b1`  
		Last Modified: Tue, 23 Aug 2022 22:09:09 GMT  
		Size: 3.1 MB (3129370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59c5c0eb30756c6d2e1dc12f61afb30464bf200f5a24a6940acac87243f28efc`  
		Last Modified: Tue, 23 Aug 2022 22:09:13 GMT  
		Size: 70.6 MB (70613083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32b4cf077cfc5a2fc82299b7bb92c40e3cb15f042a160066d1ecfdfa9901dc2`  
		Last Modified: Tue, 23 Aug 2022 22:09:09 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
