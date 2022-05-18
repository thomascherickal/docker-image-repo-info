## `redmine:bullseye`

```console
$ docker pull redmine@sha256:4800465401b7194e1f89de3618e4ebb7e353bd8f343fd106da276f099ea739ee
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

### `redmine:bullseye` - linux; amd64

```console
$ docker pull redmine@sha256:bc349cd255ee32b1bef535aadf0725370909d4416d8fe01f0355567a4bc965da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.9 MB (236905603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e302dc16390f921c2ffb52dee35256dd7e207cdd96c214a5dd5f4948de67f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 11 May 2022 01:20:16 GMT
ADD file:4a0bb88956083aa56032fdd9601d9b66c39b18c896ba35ea33594cd75621640a in / 
# Wed, 11 May 2022 01:20:16 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:28:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:28:35 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 11 May 2022 15:28:35 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 15:38:02 GMT
ENV RUBY_MAJOR=3.1
# Wed, 11 May 2022 15:38:03 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 11 May 2022 15:38:03 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 11 May 2022 15:40:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 11 May 2022 15:40:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 11 May 2022 15:40:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 11 May 2022 15:40:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 15:40:24 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 11 May 2022 15:40:24 GMT
CMD ["irb"]
# Thu, 12 May 2022 04:32:10 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 12 May 2022 04:32:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 04:32:36 GMT
ENV RAILS_ENV=production
# Thu, 12 May 2022 04:32:36 GMT
WORKDIR /usr/src/redmine
# Thu, 12 May 2022 04:32:36 GMT
ENV HOME=/home/redmine
# Thu, 12 May 2022 04:32:37 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 May 2022 01:01:37 GMT
ENV REDMINE_VERSION=5.0.1
# Wed, 18 May 2022 01:01:37 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.1.tar.gz
# Wed, 18 May 2022 01:01:37 GMT
ENV REDMINE_DOWNLOAD_SHA256=6916c5fe39d09e56921fe321464e3eb2d206d52075c61da7b8a89247e6908bb7
# Wed, 18 May 2022 01:01:40 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 May 2022 01:02:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 May 2022 01:02:12 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 May 2022 01:02:13 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 May 2022 01:02:13 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 May 2022 01:02:13 GMT
EXPOSE 3000
# Wed, 18 May 2022 01:02:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:214ca5fb90323fe769c63a12af092f2572bf1c6b300263e09883909fc865d260`  
		Last Modified: Wed, 11 May 2022 01:25:13 GMT  
		Size: 31.4 MB (31379476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78121ab1df602556d61a5738a8a7dab7d0f35b55c9bb280a6a57efa8180e1134`  
		Last Modified: Wed, 11 May 2022 16:03:17 GMT  
		Size: 10.0 MB (9992152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fbe7e8745fe998a64f0cee757d280152f7100acbe9021e34c58123f5821847`  
		Last Modified: Wed, 11 May 2022 16:03:14 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6edc84d3fe3429c82d666bcd8a6ff54e8a4fba54e6e5b2b0c86be1bf1ff8ac36`  
		Last Modified: Wed, 11 May 2022 16:04:36 GMT  
		Size: 32.4 MB (32436055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2152ead824bcdea471ba99b66e0b9951ee499dd6c73b7db08a39e0cbba5856dc`  
		Last Modified: Wed, 11 May 2022 16:04:33 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f38175b1cbb4d62a9c78bbafe26efb9e56650a494121f5b4c7b4f230ca3466`  
		Last Modified: Thu, 12 May 2022 04:35:41 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3791c21f5f9a1971ac630fe32afc1d1cbe5cb71baa2885c464500492d047ca4c`  
		Last Modified: Thu, 12 May 2022 04:35:57 GMT  
		Size: 102.0 MB (102012255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de9b324d5708627581d48410f6394ce5d465b119f0580c18aff8193039d842`  
		Last Modified: Thu, 12 May 2022 04:35:39 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:836fb1aab161be8f105486cd309cf84b8f42726c30bab9b2432e3aae5928534d`  
		Last Modified: Thu, 12 May 2022 04:35:38 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e03db3c5a0e45e8ddea546443a9f313c641686c77c30d57051f8a3aec9fd95e`  
		Last Modified: Wed, 18 May 2022 01:08:42 GMT  
		Size: 3.1 MB (3127291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eeb62e0638178c46e24728ea0b52d4ff7d8629acb2a6f02b457e2991b9df331`  
		Last Modified: Wed, 18 May 2022 01:08:47 GMT  
		Size: 58.0 MB (57954135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36d278651544a5fbdebed36dd0ce37e59fe456983037236b332531d2fde18c31`  
		Last Modified: Wed, 18 May 2022 01:08:41 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; arm variant v5

```console
$ docker pull redmine@sha256:21ae7add790ee5abc5b4706c0a53d414c756125e7a3f94e52d2daf20b55d9329
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.8 MB (205785548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b933752b6f8edf3cfc9e3f62cab83c79e69608d323c2cb4d557f17f6b3d56bc`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 05:19:45 GMT
ADD file:1eb4f937d40230354e20e28ed781234acd4be2b0dab72f87131a3eac66349719 in / 
# Thu, 17 Mar 2022 05:19:46 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:12:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:12:22 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 18:12:22 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 18:35:14 GMT
ENV RUBY_MAJOR=2.7
# Thu, 17 Mar 2022 18:35:15 GMT
ENV RUBY_VERSION=2.7.5
# Thu, 17 Mar 2022 18:35:16 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Thu, 17 Mar 2022 18:40:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 18:40:27 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 18:40:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 18:40:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 18:40:34 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 18:40:35 GMT
CMD ["irb"]
# Fri, 18 Mar 2022 06:25:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 18 Mar 2022 06:26:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:26:39 GMT
ENV RAILS_ENV=production
# Fri, 18 Mar 2022 06:26:40 GMT
WORKDIR /usr/src/redmine
# Fri, 18 Mar 2022 06:26:40 GMT
ENV HOME=/home/redmine
# Fri, 18 Mar 2022 06:26:42 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 18 Mar 2022 06:26:42 GMT
ENV REDMINE_VERSION=4.2.4
# Fri, 18 Mar 2022 06:26:43 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Fri, 18 Mar 2022 06:26:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Fri, 18 Mar 2022 06:26:49 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 18 Mar 2022 06:32:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 06:32:28 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 18 Mar 2022 06:32:29 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 18 Mar 2022 06:32:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Mar 2022 06:32:30 GMT
EXPOSE 3000
# Fri, 18 Mar 2022 06:32:30 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4da455e7774c0e977d862a56ab6d85f33ce5dd5a77d45a0a74a272e9eae6bea0`  
		Last Modified: Thu, 17 Mar 2022 05:35:01 GMT  
		Size: 28.9 MB (28919702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec0689d8bdfcc0fec586e8c48690510aa409cecfd37e461f3fc518a9b76988b`  
		Last Modified: Thu, 17 Mar 2022 19:02:47 GMT  
		Size: 8.6 MB (8630929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c035ff97c229942ee6e6869263c21925767579c2f1dca3b6235d7e30c7523d`  
		Last Modified: Thu, 17 Mar 2022 19:02:42 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c83c7bc52eef68ef61aea93f9e425714309f473a61e42876d73da980c1b4c`  
		Last Modified: Thu, 17 Mar 2022 19:05:21 GMT  
		Size: 13.9 MB (13908110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23bd3ec57b0fd653fa6deaea3b497adc92448a8cccc19fd222bbd11cf35938fe`  
		Last Modified: Thu, 17 Mar 2022 19:05:17 GMT  
		Size: 174.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b68cdff110b93cb980834e5a55b4bc5505250fc8b88f9286034996b663c9ca`  
		Last Modified: Fri, 18 Mar 2022 06:41:07 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8052e9cd460546e80959f8c9766717a7e2ba01d3019a2ed744ad0bf2157c3a3`  
		Last Modified: Fri, 18 Mar 2022 06:42:13 GMT  
		Size: 97.0 MB (96957758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc475780b793502fb114df972e0bfc556b5dad0d22b953f1e8830989af8f0764`  
		Last Modified: Fri, 18 Mar 2022 06:41:05 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bcdbc0f825358b0c38fa14f09e1807247df965df2aae1a88e1ea93a6072fef5`  
		Last Modified: Fri, 18 Mar 2022 06:41:05 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9870f95f93286f20c1c51a3233a9251ba097be6251965f12697fe9187c1c5a6`  
		Last Modified: Fri, 18 Mar 2022 06:41:09 GMT  
		Size: 3.1 MB (3064423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd4c060601a1106bf52ef6be4d2649fee89b672d4b52f4343b869c548ba1406`  
		Last Modified: Fri, 18 Mar 2022 06:41:30 GMT  
		Size: 54.3 MB (54300389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8b691b5f2c796ef085254433ee49c1286e3427f60b8207f9436e20cc57f7c8`  
		Last Modified: Fri, 18 Mar 2022 06:41:05 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; arm variant v7

```console
$ docker pull redmine@sha256:331a9bb224ab1ad805c372c1009e0ce16e940f109bbc2f0144313576984836dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.8 MB (198761834 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956fe9f6deb458bc06c1f675ce0e747be9b826260ff825db4cc2fc5d1c8a4578`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:03 GMT
ADD file:e52f9ee2dc3144d7b9eb3ec90c106aa2a094eb4c5c2aa8cbff5c520a5faaef43 in / 
# Thu, 17 Mar 2022 09:31:04 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 12:35:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 12:35:13 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 18 Mar 2022 12:35:14 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 13:14:17 GMT
ENV RUBY_MAJOR=2.7
# Fri, 18 Mar 2022 13:14:18 GMT
ENV RUBY_VERSION=2.7.5
# Fri, 18 Mar 2022 13:14:18 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Fri, 18 Mar 2022 13:18:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 18 Mar 2022 13:18:17 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 18 Mar 2022 13:18:18 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 18 Mar 2022 13:18:18 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 13:18:20 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 18 Mar 2022 13:18:20 GMT
CMD ["irb"]
# Sun, 20 Mar 2022 08:34:42 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 20 Mar 2022 08:35:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 08:35:53 GMT
ENV RAILS_ENV=production
# Sun, 20 Mar 2022 08:35:53 GMT
WORKDIR /usr/src/redmine
# Sun, 20 Mar 2022 08:35:53 GMT
ENV HOME=/home/redmine
# Sun, 20 Mar 2022 08:35:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 20 Mar 2022 08:35:55 GMT
ENV REDMINE_VERSION=4.2.4
# Sun, 20 Mar 2022 08:35:56 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Sun, 20 Mar 2022 08:35:56 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Sun, 20 Mar 2022 08:36:02 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 20 Mar 2022 08:41:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 20 Mar 2022 08:41:16 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 20 Mar 2022 08:41:16 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 20 Mar 2022 08:41:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 20 Mar 2022 08:41:17 GMT
EXPOSE 3000
# Sun, 20 Mar 2022 08:41:17 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:5e5e708ee1f9fdbc69324391f7d1f816c657e6116eff09e7d2247fa9de3a076a`  
		Last Modified: Thu, 17 Mar 2022 09:46:33 GMT  
		Size: 26.6 MB (26575097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3497ee581d2cfb66c8e24bcdd497baebe6ef22eed4d5f051041b93aa706ffd`  
		Last Modified: Fri, 18 Mar 2022 13:54:13 GMT  
		Size: 8.1 MB (8140946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb6d95c926b3b14dd8cc57ee14c6d6eee09bd97d88563df06ea05da65b4a28e`  
		Last Modified: Fri, 18 Mar 2022 13:54:07 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac5fa47201cc2427d294317049179864e093bf03876ff94471f28582b78c0fb`  
		Last Modified: Fri, 18 Mar 2022 13:58:59 GMT  
		Size: 13.8 MB (13781183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc191e2ed4b136f5831a85a9b86281d14c1ab7807fcdf88aaa839788919f0678`  
		Last Modified: Fri, 18 Mar 2022 13:58:52 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b268f89bddb30bdfab99cf1b99c439e8389c9d58b1656b66cb11248c7dde90f`  
		Last Modified: Sun, 20 Mar 2022 09:03:15 GMT  
		Size: 1.7 KB (1738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f82b2b007b32bde3a1cc79d44ad45f6ed8c00060941cb207c15900d0e4bc250`  
		Last Modified: Sun, 20 Mar 2022 09:04:15 GMT  
		Size: 93.1 MB (93105677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987239331259d33175985816cd6275d1cbac9bec5b877fdc7e1e27f1c2b20803`  
		Last Modified: Sun, 20 Mar 2022 09:03:13 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb1e9dc5a6d2bbf45f2db6cf08adfd31200150456fdbda2a4d660a05b8b0e96`  
		Last Modified: Sun, 20 Mar 2022 09:03:13 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2976299a9a77a924974e1ad13c0acca568e3a167a9a5c2afc3428d0243f0c7`  
		Last Modified: Sun, 20 Mar 2022 09:03:17 GMT  
		Size: 3.1 MB (3064422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66c115b61ad80fc860b06fd077bc187fb1f1fd4b67c6937d435cb8b78bae50cf`  
		Last Modified: Sun, 20 Mar 2022 09:03:36 GMT  
		Size: 54.1 MB (54090270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44daa1cc097b84666986b80bdfc2990f7581daa1e2089d9a4be809de85e1bbce`  
		Last Modified: Sun, 20 Mar 2022 09:03:13 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:d9a5f1092e7d5de47a80e5e2275e1659ffaa68aa25b0b7bd4218ed99f6400d28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **230.8 MB (230794159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:956ceb3dfc54bad85869978121f148f3fe67f1fb3b8fe8f9ffc1fca26ac861e0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 11 May 2022 00:46:59 GMT
ADD file:158a0e401328bd7c0d49b9e8539186098967218f1b1a8c811f4398d29b74397f in / 
# Wed, 11 May 2022 00:47:00 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:51:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 14:51:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 11 May 2022 14:51:46 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 15:01:35 GMT
ENV RUBY_MAJOR=3.1
# Wed, 11 May 2022 15:01:36 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 11 May 2022 15:01:37 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 11 May 2022 15:03:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 11 May 2022 15:03:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 11 May 2022 15:03:47 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 11 May 2022 15:03:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 15:03:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 11 May 2022 15:03:50 GMT
CMD ["irb"]
# Thu, 12 May 2022 05:17:24 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 12 May 2022 05:17:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 05:17:52 GMT
ENV RAILS_ENV=production
# Thu, 12 May 2022 05:17:53 GMT
WORKDIR /usr/src/redmine
# Thu, 12 May 2022 05:17:53 GMT
ENV HOME=/home/redmine
# Thu, 12 May 2022 05:17:55 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 May 2022 02:05:27 GMT
ENV REDMINE_VERSION=5.0.1
# Wed, 18 May 2022 02:05:28 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.1.tar.gz
# Wed, 18 May 2022 02:05:28 GMT
ENV REDMINE_DOWNLOAD_SHA256=6916c5fe39d09e56921fe321464e3eb2d206d52075c61da7b8a89247e6908bb7
# Wed, 18 May 2022 02:05:32 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 May 2022 02:06:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 May 2022 02:06:04 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 May 2022 02:06:05 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 May 2022 02:06:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 May 2022 02:06:07 GMT
EXPOSE 3000
# Wed, 18 May 2022 02:06:08 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:dfdd5ffb257742b891ccad9400a77dad2a6260b2451e0f5e48a9ade1d17a87ec`  
		Last Modified: Wed, 11 May 2022 00:53:46 GMT  
		Size: 30.1 MB (30065693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3b67922baafabbc9529545212991accdb17f9797845f3591f85ef205d2fc9f`  
		Last Modified: Wed, 11 May 2022 15:28:37 GMT  
		Size: 9.0 MB (9035226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c0df57f7dd4b85b6a4695e9642aaaff0b0ddd7192bda12ade7cf757d3979fe`  
		Last Modified: Wed, 11 May 2022 15:28:35 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f3915687f386e0ded9ebae7dcbd5b5076693bbe5be125d07d34845c25fb39f`  
		Last Modified: Wed, 11 May 2022 15:30:05 GMT  
		Size: 31.6 MB (31589547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b446e4842c9a31bd7c1b945feb500d204761b7a16188fefd65cc0571880aed`  
		Last Modified: Wed, 11 May 2022 15:30:03 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6fb53f23585d2019b029e6aa772e8ab927671cb9e6434921cd351c54c5fce4`  
		Last Modified: Thu, 12 May 2022 05:22:37 GMT  
		Size: 1.6 KB (1621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e576225710230ed95b67fbc91b6052a14a690923d72b4cab411d31c3b964024f`  
		Last Modified: Thu, 12 May 2022 05:22:52 GMT  
		Size: 99.8 MB (99800048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cb1679cc9eafa09a094fdfb3ba83b54aea6340aa144addd28b518ddaaa13a1`  
		Last Modified: Thu, 12 May 2022 05:22:35 GMT  
		Size: 137.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3eb8da123c7c6a0639fdb782b5a91994be7ebf9b957d42871f8f3bebc49674`  
		Last Modified: Thu, 12 May 2022 05:22:35 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2031a27889ca9d6b44f3c5ba342e5766552ccc7bad27a795ab66c30dd7018b8f`  
		Last Modified: Wed, 18 May 2022 02:13:35 GMT  
		Size: 3.1 MB (3127238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d88f268ec22a2d75f1ff0e032e9ad4c4ccc501f7ca1f1bb5cb88ef4b93714c9`  
		Last Modified: Wed, 18 May 2022 02:13:41 GMT  
		Size: 57.2 MB (57172384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908a0c697ef1eba6bcf94c11ea2ca901168306788a082ecc535a698fc1497e03`  
		Last Modified: Wed, 18 May 2022 02:13:34 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; 386

```console
$ docker pull redmine@sha256:44503ab5308950ddcf7db5a4092182772aef2832366f784eaf720256aaae6fc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **238.6 MB (238597417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31c8be81827c23b611d98502d433747a1055a162eb52822618e13a0dbc48437b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 11 May 2022 01:39:14 GMT
ADD file:9eecb0fd311177f9d226e914c411aef49b5de1930e73019d2ee24afed515b5a2 in / 
# Wed, 11 May 2022 01:39:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 15:01:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:01:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 11 May 2022 15:01:15 GMT
ENV LANG=C.UTF-8
# Wed, 11 May 2022 15:11:03 GMT
ENV RUBY_MAJOR=3.1
# Wed, 11 May 2022 15:11:04 GMT
ENV RUBY_VERSION=3.1.2
# Wed, 11 May 2022 15:11:05 GMT
ENV RUBY_DOWNLOAD_SHA256=ca10d017f8a1b6d247556622c841fc56b90c03b1803f87198da1e4fd3ec3bf2a
# Wed, 11 May 2022 15:13:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 11 May 2022 15:13:19 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 11 May 2022 15:13:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 11 May 2022 15:13:21 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 15:13:22 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 11 May 2022 15:13:23 GMT
CMD ["irb"]
# Wed, 11 May 2022 20:28:29 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 11 May 2022 20:28:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 20:28:59 GMT
ENV RAILS_ENV=production
# Wed, 11 May 2022 20:29:00 GMT
WORKDIR /usr/src/redmine
# Wed, 11 May 2022 20:29:01 GMT
ENV HOME=/home/redmine
# Wed, 11 May 2022 20:29:02 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 18 May 2022 02:21:16 GMT
ENV REDMINE_VERSION=5.0.1
# Wed, 18 May 2022 02:21:17 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.1.tar.gz
# Wed, 18 May 2022 02:21:17 GMT
ENV REDMINE_DOWNLOAD_SHA256=6916c5fe39d09e56921fe321464e3eb2d206d52075c61da7b8a89247e6908bb7
# Wed, 18 May 2022 02:21:21 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 18 May 2022 02:21:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 18 May 2022 02:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 18 May 2022 02:21:55 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 18 May 2022 02:21:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 18 May 2022 02:21:57 GMT
EXPOSE 3000
# Wed, 18 May 2022 02:21:58 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:91c5bdbe4bf9f1970dd54ba71e2523649adce4e5240c2ff8a87711bf389ecba3`  
		Last Modified: Wed, 11 May 2022 01:46:25 GMT  
		Size: 32.4 MB (32389776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a020b71ec599bfb0b119536b160ef416432ad7563df9a6df96e3daa47eb428a5`  
		Last Modified: Wed, 11 May 2022 15:38:34 GMT  
		Size: 11.8 MB (11788800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac8bc3c1327d50a77c927b43839b20ee757c8031b34600d7e2e544df73be66a`  
		Last Modified: Wed, 11 May 2022 15:38:32 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3718714e9c9212b3fb61a865127cb7bbe0dd66a0e32ebfa9cfcdaef99f6a2cd5`  
		Last Modified: Wed, 11 May 2022 15:40:12 GMT  
		Size: 30.8 MB (30788950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7010ee581c5be9f5d968209cf93235b2c478fe0b2540595e6e4fd34e0439f4d`  
		Last Modified: Wed, 11 May 2022 15:40:09 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bd5cb480db7462bac4fb13e3cfff14540418dfc31d9c232cebaf18dd040671`  
		Last Modified: Wed, 11 May 2022 20:32:46 GMT  
		Size: 1.6 KB (1613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5b630d26517bc033d4ff51d4c6b65b2cab8893eb59b11b4c6114cae00131c7c`  
		Last Modified: Wed, 11 May 2022 20:33:01 GMT  
		Size: 103.4 MB (103362302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5b193685f1180f135db2beccd6e4edfe24c0fece5efe458acdaf987b7f6fee3`  
		Last Modified: Wed, 11 May 2022 20:32:44 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50111afdf1269243c9d8e99fc4583d51884e429b8da31761a7f99b9ca212a0f3`  
		Last Modified: Wed, 11 May 2022 20:32:44 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6696ff600f712e8a58a1d9b37de187df35c2ffa97698a3d52d146172b87d269d`  
		Last Modified: Wed, 18 May 2022 02:29:04 GMT  
		Size: 3.1 MB (3127237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e3fe5325199bc31c1dcc03431dadcc898369740225904cad04813a18080584`  
		Last Modified: Wed, 18 May 2022 02:29:11 GMT  
		Size: 57.1 MB (57136334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231e955e23fe5e7e96d1049974f44e6e3794d3cb47a889a2d29fb8ff993af033`  
		Last Modified: Wed, 18 May 2022 02:29:03 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; ppc64le

```console
$ docker pull redmine@sha256:a75b3121f8499cb1e798b8b34be06c2839a08c4e62e6de2fc31bd0342ef2655a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.4 MB (227426703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ada7b0525e5441c17ae136a20abb860d76cf2024ceeb9895ea30d7458f33aa3a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 11:17:54 GMT
ADD file:e8555f1cb439a45786b92e929cfa154b51f668c5b4cd69e4ce98340c5998fe0c in / 
# Thu, 17 Mar 2022 11:18:00 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 08:52:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:53:02 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Fri, 18 Mar 2022 08:53:09 GMT
ENV LANG=C.UTF-8
# Fri, 18 Mar 2022 10:27:30 GMT
ENV RUBY_MAJOR=2.7
# Fri, 18 Mar 2022 10:27:35 GMT
ENV RUBY_VERSION=2.7.5
# Fri, 18 Mar 2022 10:27:41 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Fri, 18 Mar 2022 10:36:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Fri, 18 Mar 2022 10:36:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Fri, 18 Mar 2022 10:36:20 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Fri, 18 Mar 2022 10:36:27 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 10:36:35 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Fri, 18 Mar 2022 10:36:38 GMT
CMD ["irb"]
# Sun, 20 Mar 2022 03:16:13 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 20 Mar 2022 03:20:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 03:20:43 GMT
ENV RAILS_ENV=production
# Sun, 20 Mar 2022 03:20:46 GMT
WORKDIR /usr/src/redmine
# Sun, 20 Mar 2022 03:20:48 GMT
ENV HOME=/home/redmine
# Sun, 20 Mar 2022 03:20:54 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 20 Mar 2022 03:20:57 GMT
ENV REDMINE_VERSION=4.2.4
# Sun, 20 Mar 2022 03:21:00 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Sun, 20 Mar 2022 03:21:02 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Sun, 20 Mar 2022 03:21:12 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 20 Mar 2022 03:25:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 20 Mar 2022 03:26:00 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 20 Mar 2022 03:26:02 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Sun, 20 Mar 2022 03:26:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 20 Mar 2022 03:26:09 GMT
EXPOSE 3000
# Sun, 20 Mar 2022 03:26:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:aec78dc45d7b3df12df0672d13e22005592b453f03ff2580efac2598dddd680b`  
		Last Modified: Thu, 17 Mar 2022 11:28:17 GMT  
		Size: 35.3 MB (35279758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c86c5924edf28293cb4ebc09502f5f8504fc2d95a2b23933f3b629a2bbefb7c`  
		Last Modified: Fri, 18 Mar 2022 11:25:42 GMT  
		Size: 10.5 MB (10472452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20089f9fbec0f2dc204b463c766ab12f80308316ed9ef319ad99b529e2d99a4f`  
		Last Modified: Fri, 18 Mar 2022 11:25:39 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a304d718fc18c12ff21b7d345c21f08dc819a27f611eae3508b4777f8ae10aa`  
		Last Modified: Fri, 18 Mar 2022 11:29:07 GMT  
		Size: 15.0 MB (15049528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfab9e5590637c58b3112e92c45bc7523dbe5fd76e57c45176ee33ca216207ad`  
		Last Modified: Fri, 18 Mar 2022 11:29:04 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa36eb2e41d1f62130333203713ed440057bc23399f1e86897e10d8d4d42c24`  
		Last Modified: Sun, 20 Mar 2022 03:54:36 GMT  
		Size: 1.8 KB (1758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108c199db54921c3a0b2d3d0ad9cd2feca7e0b16de38e1d90f56c2679226bec6`  
		Last Modified: Sun, 20 Mar 2022 03:54:55 GMT  
		Size: 107.5 MB (107488837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaccc4a19cf749a5417eeb2a11796d3d2f68b4e20febd734b5319ddfbaf64b45`  
		Last Modified: Sun, 20 Mar 2022 03:54:33 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd76a7ffba6da9d1c033dcd890ba698f78757e4f79db21649fa9ea88988835b8`  
		Last Modified: Sun, 20 Mar 2022 03:54:33 GMT  
		Size: 160.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1376f496480aec986e9c11a678f1d6484c8f2f0e566b447449a4710d664a3428`  
		Last Modified: Sun, 20 Mar 2022 03:54:34 GMT  
		Size: 3.1 MB (3064429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc68165acff1caa21e4352df5d807a6ccf0a33d931faee33460a03af9c62ac8`  
		Last Modified: Sun, 20 Mar 2022 03:54:41 GMT  
		Size: 56.1 MB (56067442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d786ee07e26ecef1667ca07a51309ee34ad07ce159a481a9955d8d3732cd30`  
		Last Modified: Sun, 20 Mar 2022 03:54:33 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:bullseye` - linux; s390x

```console
$ docker pull redmine@sha256:df1522f7b5941c7bbdf074542f202e1ec37d8946b6ec9e96120ccbf9ccb19336
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210726380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d43e728f1eaba9b5ab6241358f057dfb4f4ad83e0d0a7023a86d1d8e3205e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:58 GMT
ADD file:52f9267b4c57ac585a0d3d47a6f2ae1a71398264173ad4f190332957fa629c67 in / 
# Thu, 17 Mar 2022 03:07:01 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 15:47:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 15:47:31 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 17 Mar 2022 15:47:32 GMT
ENV LANG=C.UTF-8
# Thu, 17 Mar 2022 16:05:24 GMT
ENV RUBY_MAJOR=2.7
# Thu, 17 Mar 2022 16:05:25 GMT
ENV RUBY_VERSION=2.7.5
# Thu, 17 Mar 2022 16:05:25 GMT
ENV RUBY_DOWNLOAD_SHA256=d216d95190eaacf3bf165303747b02ff13f10b6cfab67a9031b502a49512b516
# Thu, 17 Mar 2022 16:06:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 17 Mar 2022 16:06:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 17 Mar 2022 16:06:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 17 Mar 2022 16:06:48 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 17 Mar 2022 16:06:49 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 17 Mar 2022 16:06:49 GMT
CMD ["irb"]
# Fri, 18 Mar 2022 08:04:34 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 18 Mar 2022 08:05:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 08:05:23 GMT
ENV RAILS_ENV=production
# Fri, 18 Mar 2022 08:05:23 GMT
WORKDIR /usr/src/redmine
# Fri, 18 Mar 2022 08:05:24 GMT
ENV HOME=/home/redmine
# Fri, 18 Mar 2022 08:05:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 18 Mar 2022 08:05:24 GMT
ENV REDMINE_VERSION=4.2.4
# Fri, 18 Mar 2022 08:05:24 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.4.tar.gz
# Fri, 18 Mar 2022 08:05:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=cf649f5d4ff783582f82bebd4a5099ef63acb3d5573bbe6b4bf64f293c61c9ce
# Fri, 18 Mar 2022 08:05:27 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 18 Mar 2022 08:06:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 18 Mar 2022 08:06:52 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 18 Mar 2022 08:06:52 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Fri, 18 Mar 2022 08:06:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 18 Mar 2022 08:06:52 GMT
EXPOSE 3000
# Fri, 18 Mar 2022 08:06:52 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:d101968410e5005df630b0572aec03c88de55b8de81f3cf7e6a57e1ce2e5a8e5`  
		Last Modified: Thu, 17 Mar 2022 03:12:46 GMT  
		Size: 29.7 MB (29655795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d22373fdb95e60881955d65541429ef7613c6f6b47adab53cad763afa08eb15`  
		Last Modified: Thu, 17 Mar 2022 16:22:59 GMT  
		Size: 8.9 MB (8856005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:248f006a5a0b6e0eee5c9327fd5e34843eba441b2c731f9fd9dcb9f4e5d7afde`  
		Last Modified: Thu, 17 Mar 2022 16:22:58 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6d859e14e82173b7489f8a174d1dfbc854232374c1cc9b60d879cc62934421d`  
		Last Modified: Thu, 17 Mar 2022 16:26:07 GMT  
		Size: 14.7 MB (14662445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662aae40f54e9f88fe059b7caa3a8dfd58b47bb665f142b6729faad116400d50`  
		Last Modified: Thu, 17 Mar 2022 16:26:06 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebc42ec843144c9673f30c7a48d15aee4313cae9ac895edb81ccecefe62a743`  
		Last Modified: Fri, 18 Mar 2022 08:12:57 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f457638e66375290b61fc0d1629cf6a9f2150280e1d934df89df19efc251d4`  
		Last Modified: Fri, 18 Mar 2022 08:13:10 GMT  
		Size: 99.1 MB (99127551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a419aade13edd85aff0a13e0ba497a7442a900f8b9ac4d45f01dc6f4b734e986`  
		Last Modified: Fri, 18 Mar 2022 08:12:56 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a48f7c3c449104d23733d90501d812bfcda335029b86f3a39cf61724add0f3bc`  
		Last Modified: Fri, 18 Mar 2022 08:12:56 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be765c540b5f7225c40614d9f2fbb78af78c7a98f101135938d676fc48e1821`  
		Last Modified: Fri, 18 Mar 2022 08:12:56 GMT  
		Size: 3.1 MB (3064420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578e2da5ce73fad1aab806790fa52c0a3b76e4dd4a6b75486b13328148efb97b`  
		Last Modified: Fri, 18 Mar 2022 08:13:00 GMT  
		Size: 55.4 MB (55355919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f5a6a1d4d10235dcf6b4f6ea52db4361825113e16f060f169b79ee267925dc`  
		Last Modified: Fri, 18 Mar 2022 08:12:56 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
