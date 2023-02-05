## `redmine:5-bullseye`

```console
$ docker pull redmine@sha256:df4ff71e736524a7f79a257966e781acf0c58c5053cf6036bec1473838bacc50
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

### `redmine:5-bullseye` - linux; amd64

```console
$ docker pull redmine@sha256:e2f6c8d38aaedd57dd69911dc173ce6334dcbd96b1d0ec7250dc2d969ffc005a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.5 MB (240456497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d70d164cb59c5dc7570563e970417c79b51eff307da72791fd6b4c52cfe90ae1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:41 GMT
ADD file:1d256392bb7afe6942d157db84ca62774ac4114f8a3816fd50bace8d73130b57 in / 
# Sat, 04 Feb 2023 06:51:41 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 20:18:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 20:18:56 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 04 Feb 2023 20:18:56 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 20:29:25 GMT
ENV RUBY_MAJOR=3.1
# Sat, 04 Feb 2023 20:29:25 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 04 Feb 2023 20:29:25 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 04 Feb 2023 20:31:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 04 Feb 2023 20:31:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 04 Feb 2023 20:31:45 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 04 Feb 2023 20:31:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 20:31:46 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 04 Feb 2023 20:31:46 GMT
CMD ["irb"]
# Sun, 05 Feb 2023 04:43:13 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 05 Feb 2023 04:43:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 04:43:48 GMT
ENV RAILS_ENV=production
# Sun, 05 Feb 2023 04:43:48 GMT
WORKDIR /usr/src/redmine
# Sun, 05 Feb 2023 04:43:49 GMT
ENV HOME=/home/redmine
# Sun, 05 Feb 2023 04:43:49 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 05 Feb 2023 04:43:49 GMT
ENV REDMINE_VERSION=5.0.4
# Sun, 05 Feb 2023 04:43:49 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Sun, 05 Feb 2023 04:43:49 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Sun, 05 Feb 2023 04:43:53 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 05 Feb 2023 04:44:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 05 Feb 2023 04:44:27 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 05 Feb 2023 04:44:27 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Sun, 05 Feb 2023 04:44:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 05 Feb 2023 04:44:27 GMT
EXPOSE 3000
# Sun, 05 Feb 2023 04:44:27 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:01b5b2efb836d74b8b49da819514eca52e25290d1688db59420ffb9c6b65a03c`  
		Last Modified: Sat, 04 Feb 2023 06:56:17 GMT  
		Size: 31.4 MB (31396919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a518007828d6d0dc1fa5ee4cd5318885881db3d8a6eeb9720b156c740733e50`  
		Last Modified: Sat, 04 Feb 2023 20:54:21 GMT  
		Size: 10.0 MB (10020328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defb9747fcb73c78c26f4e85993c9791b035f4abe963ba7a0b1cc098fe1f123f`  
		Last Modified: Sat, 04 Feb 2023 20:54:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a219c5ebe5578692e906384f573ad500c1edcacb058873f4ed2b004fa79808`  
		Last Modified: Sat, 04 Feb 2023 20:55:37 GMT  
		Size: 32.6 MB (32613342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639f6a2e57946ced452be7bf967731e82cd87895be40180326feefb36c2ec2df`  
		Last Modified: Sat, 04 Feb 2023 20:55:34 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4b80475c1357b08bb0e7f36a0fc44fdfa3208d1d29073c21df01acb6f4e277`  
		Last Modified: Sun, 05 Feb 2023 04:46:56 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcb18cdee398d136f570e80339dfb0bce6ac04beb5c7ff509214160480aa8dd`  
		Last Modified: Sun, 05 Feb 2023 04:47:11 GMT  
		Size: 102.0 MB (102035430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f81f7150d5baedd6fe42884c8fc44b654321ed43e29e711698aabf552f3f857`  
		Last Modified: Sun, 05 Feb 2023 04:46:54 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6d36a389fd335b64d8cc97e01bac355d1d9d99e944acb37523a6eecba5f800`  
		Last Modified: Sun, 05 Feb 2023 04:46:54 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eef99d509188410d36ef822fd29b4315dc6c02e6e0107d3f39b3010829dc94e`  
		Last Modified: Sun, 05 Feb 2023 04:46:55 GMT  
		Size: 3.1 MB (3143012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679e9e96b698eebbbd73006bcb8bb460f8e8ece3e4f8062edc7b0f187938c5c5`  
		Last Modified: Sun, 05 Feb 2023 04:47:02 GMT  
		Size: 61.2 MB (61243013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:135b4bc780b4f565f970eb76f90e9e2963367dd4b79522884b4330776edacae0`  
		Last Modified: Sun, 05 Feb 2023 04:46:54 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm variant v5

```console
$ docker pull redmine@sha256:6cb676d3a68eb474f3ae47f1d9dae8ac079c7d662d4529a7c163e1f5be34aabc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.3 MB (239262134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:046781a5326e0ccbcfa60d13a7f435e166749fa394c22d1d0d1a9c20b62c8590`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 04 Feb 2023 02:46:38 GMT
ADD file:ce468627e54d8d1c839cea8ab62e505f612298fd97d50e189293fcfcc6af03a5 in / 
# Sat, 04 Feb 2023 02:46:38 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 09:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 09:33:41 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 04 Feb 2023 09:33:41 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 09:38:56 GMT
ENV RUBY_MAJOR=3.1
# Sat, 04 Feb 2023 09:38:56 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 04 Feb 2023 09:38:57 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 04 Feb 2023 09:41:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 04 Feb 2023 09:41:28 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 04 Feb 2023 09:41:28 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 04 Feb 2023 09:41:28 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 09:41:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 04 Feb 2023 09:41:29 GMT
CMD ["irb"]
# Sat, 04 Feb 2023 16:16:26 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Feb 2023 16:17:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 16:17:05 GMT
ENV RAILS_ENV=production
# Sat, 04 Feb 2023 16:17:05 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Feb 2023 16:17:05 GMT
ENV HOME=/home/redmine
# Sat, 04 Feb 2023 16:17:05 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Feb 2023 16:17:06 GMT
ENV REDMINE_VERSION=5.0.4
# Sat, 04 Feb 2023 16:17:06 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Sat, 04 Feb 2023 16:17:06 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Sat, 04 Feb 2023 16:17:09 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Feb 2023 16:19:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 16:19:15 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Feb 2023 16:19:15 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Sat, 04 Feb 2023 16:19:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 16:19:15 GMT
EXPOSE 3000
# Sat, 04 Feb 2023 16:19:15 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:83735a64f458d40820e4310d632e8bb1dc888f6c25114496be3ce431b5f21d5d`  
		Last Modified: Sat, 04 Feb 2023 02:51:43 GMT  
		Size: 28.9 MB (28898637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11840acf7524c8615792233e0aa865a39fcfec82fd12f1d56dcdeafa27377e7`  
		Last Modified: Sat, 04 Feb 2023 09:53:09 GMT  
		Size: 8.6 MB (8633880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7f9f67c68be3b740ba8f9e275da3d27631b9dd6231fbae67e61ac82fa18145e`  
		Last Modified: Sat, 04 Feb 2023 09:53:07 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d40c62ccc9597509afd2114ce7375a7f3d269ad3dd297c18c5c7d519ab521a4c`  
		Last Modified: Sat, 04 Feb 2023 09:54:06 GMT  
		Size: 31.2 MB (31161662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfaa70a6a99e4a31051442a405e1dd5217faa6d0a5ab5dec2392a8e9259b5248`  
		Last Modified: Sat, 04 Feb 2023 09:54:02 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9759af3e818961e97027c0a61aa517fff88673cc083bb033ac4499c202a95f7`  
		Last Modified: Sat, 04 Feb 2023 16:23:16 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0197730af3ca9291fe873abf8d9cf220f80fbf03881c76b582b7a3c8e912bb64`  
		Last Modified: Sat, 04 Feb 2023 16:23:37 GMT  
		Size: 97.0 MB (96992190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d492012e7ccf7b6cc80adfdad32c39a8810b851b760362bc578f10180c41deb5`  
		Last Modified: Sat, 04 Feb 2023 16:23:14 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e0a34281a3ba607829a814505b9452cfbba7a67b43a25d84692c4718724b0b`  
		Last Modified: Sat, 04 Feb 2023 16:23:14 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac847cdcf40f99ee76d22e463c4e43505af71a05f984cded4d322094afd35f1d`  
		Last Modified: Sat, 04 Feb 2023 16:23:16 GMT  
		Size: 3.1 MB (3142680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816d1fbaac01392382d2807cfb53ab5b281c5bfc6ccf881eecbd47998c5df47c`  
		Last Modified: Sat, 04 Feb 2023 16:23:25 GMT  
		Size: 70.4 MB (70428729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08a870c2786a28788bd1c6d67449427a6f96cd548b2d631cb73c69ede013eb7`  
		Last Modified: Sat, 04 Feb 2023 16:23:14 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm variant v7

```console
$ docker pull redmine@sha256:02eea70c47dbefb392ee8a8254e33dc531ae25ae79ab483d7495a369b2d0e796
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.2 MB (232171301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:813d00988b99b105c9437baa608dd894153e714959f797cef74ee6eb494a9b95`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 11 Jan 2023 04:00:36 GMT
ADD file:3fb94bfd628f3ebd91db74501bd297a817977cc066664f0fa342442b3352e0be in / 
# Wed, 11 Jan 2023 04:00:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 18:29:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 18:29:41 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 11 Jan 2023 18:29:41 GMT
ENV LANG=C.UTF-8
# Wed, 11 Jan 2023 18:39:14 GMT
ENV RUBY_MAJOR=3.1
# Wed, 11 Jan 2023 18:39:15 GMT
ENV RUBY_VERSION=3.1.3
# Wed, 11 Jan 2023 18:39:15 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Wed, 11 Jan 2023 18:41:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 11 Jan 2023 18:41:29 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 11 Jan 2023 18:41:29 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 11 Jan 2023 18:41:29 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 Jan 2023 18:41:29 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 11 Jan 2023 18:41:29 GMT
CMD ["irb"]
# Thu, 12 Jan 2023 05:52:17 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 12 Jan 2023 05:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 Jan 2023 05:52:50 GMT
ENV RAILS_ENV=production
# Thu, 12 Jan 2023 05:52:50 GMT
WORKDIR /usr/src/redmine
# Thu, 12 Jan 2023 05:52:51 GMT
ENV HOME=/home/redmine
# Thu, 12 Jan 2023 05:52:51 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 12 Jan 2023 05:52:51 GMT
ENV REDMINE_VERSION=5.0.4
# Thu, 12 Jan 2023 05:52:51 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Thu, 12 Jan 2023 05:52:51 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Thu, 12 Jan 2023 05:52:55 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 12 Jan 2023 05:54:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 12 Jan 2023 05:54:35 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 12 Jan 2023 05:54:35 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Thu, 12 Jan 2023 05:54:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 12 Jan 2023 05:54:35 GMT
EXPOSE 3000
# Thu, 12 Jan 2023 05:54:35 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:330ad28688ae3fa5f3b241fef3efd076299bec9874e0597b1c16dcf8a165a53d`  
		Last Modified: Wed, 11 Jan 2023 04:07:49 GMT  
		Size: 26.6 MB (26559488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c4329f115ccb62a523184a59f6677da5453b0d310a49802471adda6a5f696b`  
		Last Modified: Wed, 11 Jan 2023 19:06:44 GMT  
		Size: 8.1 MB (8142228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2f88bb9c79099195b3a20ab2c1514dbb503f0bcc31d9dd770d3b661343def6`  
		Last Modified: Wed, 11 Jan 2023 19:06:42 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15754fb0e7143626e8f37f3f553f347a931ccc393f46a91a67fdc7bab863610b`  
		Last Modified: Wed, 11 Jan 2023 19:08:34 GMT  
		Size: 31.0 MB (31025384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2160666b2d6f262dc0a75a00e8f29acda7b1d739333cd38d57baef295106c2`  
		Last Modified: Wed, 11 Jan 2023 19:08:31 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7844b68c9de9fa85d05a8e0c08a67ae214fb498dde4bc5a52a81c729f7e420`  
		Last Modified: Thu, 12 Jan 2023 05:58:48 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e1ba50c08b1fa1e079823bc968bc6ef6793d57eb59a995c714b75e511fd2d6`  
		Last Modified: Thu, 12 Jan 2023 05:59:05 GMT  
		Size: 93.1 MB (93133645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfdd5bdabc01063607f2d83af446510f438271dacdbf0582bd6915791b8a52c7`  
		Last Modified: Thu, 12 Jan 2023 05:58:46 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2506c9bcd3fca9888a59834fbe90aad6d8c2ffd70270546d95f41918af94f9fb`  
		Last Modified: Thu, 12 Jan 2023 05:58:46 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187f25098855f70adbe9f074e38e00bb423fae50dc444e07e013788032aa10bf`  
		Last Modified: Thu, 12 Jan 2023 05:58:47 GMT  
		Size: 3.1 MB (3142681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0148a404996ff5fb9b7fb5b6a9a4128e5d727d36ed5645401f773d2c7380c34d`  
		Last Modified: Thu, 12 Jan 2023 05:58:56 GMT  
		Size: 70.2 MB (70163522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a791140a398ea3789da3a9e2f413f6225ebfadcc75eb4e162585a24770a6ab`  
		Last Modified: Thu, 12 Jan 2023 05:58:46 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:c16a7c1ac99604ef52485daab56e31fa9c42600da19076d59978830795f88e70
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.9 MB (234948474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:708d8d54a2b68820a7e07fb8ef8b8eb0b4108dfea1e300f0f98888a2a1fd0957`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:37 GMT
ADD file:f613775c59ebd3ca219dc6bbad83115eb74bbbc1980ca4b63e7cb8ab3fa364e4 in / 
# Sat, 04 Feb 2023 06:17:37 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 16:28:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 16:28:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 04 Feb 2023 16:28:58 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 16:37:26 GMT
ENV RUBY_MAJOR=3.1
# Sat, 04 Feb 2023 16:37:26 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 04 Feb 2023 16:37:27 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 04 Feb 2023 16:39:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 04 Feb 2023 16:39:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 04 Feb 2023 16:39:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 04 Feb 2023 16:39:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 16:39:15 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 04 Feb 2023 16:39:15 GMT
CMD ["irb"]
# Sun, 05 Feb 2023 00:35:56 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 05 Feb 2023 00:36:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:36:23 GMT
ENV RAILS_ENV=production
# Sun, 05 Feb 2023 00:36:23 GMT
WORKDIR /usr/src/redmine
# Sun, 05 Feb 2023 00:36:24 GMT
ENV HOME=/home/redmine
# Sun, 05 Feb 2023 00:36:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 05 Feb 2023 00:36:24 GMT
ENV REDMINE_VERSION=5.0.4
# Sun, 05 Feb 2023 00:36:24 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Sun, 05 Feb 2023 00:36:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Sun, 05 Feb 2023 00:36:27 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 05 Feb 2023 00:36:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 05 Feb 2023 00:36:52 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 05 Feb 2023 00:36:52 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Sun, 05 Feb 2023 00:36:52 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 05 Feb 2023 00:36:52 GMT
EXPOSE 3000
# Sun, 05 Feb 2023 00:36:53 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:f79f8cc5c20d534298dd6317333f38b7691da6d66e063ff10699727982c852be`  
		Last Modified: Sat, 04 Feb 2023 06:21:25 GMT  
		Size: 30.0 MB (30044792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4815cea4ccc92deb5768f1c409807f717772a2991fd01107c6acb13067969972`  
		Last Modified: Sat, 04 Feb 2023 16:57:57 GMT  
		Size: 9.2 MB (9242937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7cf6c53b2ebd778e263c408d13f39e38a6dd33c8cb44cc6f96a74bd9c42cd7`  
		Last Modified: Sat, 04 Feb 2023 16:57:56 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f55aa3ed5adccf6964f7d9abcfa49d7441d8036bef50ce6604d7c45a9c0c52`  
		Last Modified: Sat, 04 Feb 2023 16:59:14 GMT  
		Size: 32.0 MB (31982624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71a8ab94c1c7949514bffa486d8eceaca945ad7e15247b7c6efbf2f58fc09dd`  
		Last Modified: Sat, 04 Feb 2023 16:59:11 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:259c3f74389678634a140fd1d20b08376b89d396d082724a14147ba15c46d00c`  
		Last Modified: Sun, 05 Feb 2023 00:38:48 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd16a2ec0127e8131edc4f53a840d49e6a7df236de3a8fd4475cf0d2dff7140`  
		Last Modified: Sun, 05 Feb 2023 00:39:00 GMT  
		Size: 99.8 MB (99807832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0e47294ad01c7c6ce6c812a21746c5e451e9466e138d48183ca333c481a2b4`  
		Last Modified: Sun, 05 Feb 2023 00:38:46 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245dbdc16bd7484225acca32084d6d5934ff7d7968da29b609ded497ace3f029`  
		Last Modified: Sun, 05 Feb 2023 00:38:46 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37f9ed8ba8f4244d6a7014c01c7cea3c07fa72f76a1f4bfe04cf548b02b60eb`  
		Last Modified: Sun, 05 Feb 2023 00:38:47 GMT  
		Size: 3.1 MB (3143016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2904ed9e25f0410054cf5e4ad46f59721850aa53af2937f4fec9aa2de2da870`  
		Last Modified: Sun, 05 Feb 2023 00:38:51 GMT  
		Size: 60.7 MB (60722817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0afc2de3f5d7a9bfa6ba45f93c7eb2253cd5fa21c91e1037d03416f168c76c97`  
		Last Modified: Sun, 05 Feb 2023 00:38:46 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; 386

```console
$ docker pull redmine@sha256:2cf58b9c64b320843d2035fd7bd3fbfe087549fe1f36a492cfc0fba5ec0982a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.1 MB (242142543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d5541e8c67943e993d517b5a18e81b5a91691ea8a883055b157499fc069f996`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 04 Feb 2023 07:49:22 GMT
ADD file:82af884aad6a87f5b309a7418aa1df69f92180a39818ae6d77d37d072cb6fecb in / 
# Sat, 04 Feb 2023 07:49:22 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 20:55:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 20:55:18 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 04 Feb 2023 20:55:19 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 21:05:06 GMT
ENV RUBY_MAJOR=3.1
# Sat, 04 Feb 2023 21:05:07 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 04 Feb 2023 21:05:08 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 04 Feb 2023 21:07:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 04 Feb 2023 21:07:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 04 Feb 2023 21:07:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 04 Feb 2023 21:07:26 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 21:07:27 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 04 Feb 2023 21:07:28 GMT
CMD ["irb"]
# Sun, 05 Feb 2023 02:41:51 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 05 Feb 2023 02:42:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 02:42:24 GMT
ENV RAILS_ENV=production
# Sun, 05 Feb 2023 02:42:24 GMT
WORKDIR /usr/src/redmine
# Sun, 05 Feb 2023 02:42:25 GMT
ENV HOME=/home/redmine
# Sun, 05 Feb 2023 02:42:27 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 05 Feb 2023 02:42:27 GMT
ENV REDMINE_VERSION=5.0.4
# Sun, 05 Feb 2023 02:42:28 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Sun, 05 Feb 2023 02:42:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Sun, 05 Feb 2023 02:42:33 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 05 Feb 2023 02:43:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 05 Feb 2023 02:43:08 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 05 Feb 2023 02:43:09 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Sun, 05 Feb 2023 02:43:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 05 Feb 2023 02:43:10 GMT
EXPOSE 3000
# Sun, 05 Feb 2023 02:43:11 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:fb99e0a97d653ef9acb2bdac0d1d10a8655b789bd4e8924c4a1c4a2af8adbb4a`  
		Last Modified: Sat, 04 Feb 2023 07:55:04 GMT  
		Size: 32.4 MB (32375772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a3ffbbaa63b01e2cf819a55818eea1eb46db3b3aafaf5784db252606400ae58`  
		Last Modified: Sat, 04 Feb 2023 21:32:10 GMT  
		Size: 12.0 MB (11992883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dd325b91bebd8537cd4104c8d5811ee15d0d093387c94329a18c33aabcc967`  
		Last Modified: Sat, 04 Feb 2023 21:32:08 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:490635fff5bce5b8bfdfccd05abf37031cf71711f9a60ef1c92bcaef350fad3a`  
		Last Modified: Sat, 04 Feb 2023 21:33:48 GMT  
		Size: 31.0 MB (30956717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c7d2c63f828c9f5480a5d9385d8c54ac11005c15f1a7fc3be1cf5e5c3a6873`  
		Last Modified: Sat, 04 Feb 2023 21:33:44 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9002655c708b5cb1d5afde5a4f18f6e4f9bc6fab568b90e31f5af30927e4fa`  
		Last Modified: Sun, 05 Feb 2023 02:46:02 GMT  
		Size: 1.6 KB (1613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c80cd5bdcf60a7c31db76872e3075e3e380b00d3411463f220049670e48ae6`  
		Last Modified: Sun, 05 Feb 2023 02:46:17 GMT  
		Size: 103.4 MB (103357271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96a2ed6a16435fd7c010661896c3b2c4747902c63adcc4658011ac5cdf5ecd5`  
		Last Modified: Sun, 05 Feb 2023 02:46:00 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5235a10343a37ee20d2ca0bb26af71b3f4d31675bb2e0132e79246e91e5c6be2`  
		Last Modified: Sun, 05 Feb 2023 02:46:00 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5b83509de68165cc4edfc6c2106f2cf936bb8b966593a4da8e798c49abb04d`  
		Last Modified: Sun, 05 Feb 2023 02:46:01 GMT  
		Size: 3.1 MB (3142886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37a04381073f5ef4fc7d8036a57615bb4e072793f8c36d3e96d5bf87cdfbd5a`  
		Last Modified: Sun, 05 Feb 2023 02:46:06 GMT  
		Size: 60.3 MB (60312780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c949b85c6d1e56ce01c45699b3750f77c325bbff12beb16e469cc973350a4dff`  
		Last Modified: Sun, 05 Feb 2023 02:46:00 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; ppc64le

```console
$ docker pull redmine@sha256:b9b9f8a48003053bb61789db73a5b9337d2029c0785107fc550cffeb69bb3cdf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.6 MB (262601889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a0e4334d59321252fd332bc77adbeccb3b15c2e9cb413b44379875dabdd8e51`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 04 Feb 2023 12:25:55 GMT
ADD file:2c82cc89d7ac2efeaf54e7589e28644e3e8436d66f6909bf295a2b030116ac58 in / 
# Sat, 04 Feb 2023 12:25:58 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 16:50:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 16:50:35 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 04 Feb 2023 16:50:35 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 16:55:39 GMT
ENV RUBY_MAJOR=3.1
# Sat, 04 Feb 2023 16:55:39 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 04 Feb 2023 16:55:39 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 04 Feb 2023 17:00:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 04 Feb 2023 17:00:09 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 04 Feb 2023 17:00:09 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 04 Feb 2023 17:00:10 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 17:00:11 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 04 Feb 2023 17:00:12 GMT
CMD ["irb"]
# Sun, 05 Feb 2023 02:17:09 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 05 Feb 2023 02:18:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 02:18:37 GMT
ENV RAILS_ENV=production
# Sun, 05 Feb 2023 02:18:37 GMT
WORKDIR /usr/src/redmine
# Sun, 05 Feb 2023 02:18:38 GMT
ENV HOME=/home/redmine
# Sun, 05 Feb 2023 02:18:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sun, 05 Feb 2023 02:18:40 GMT
ENV REDMINE_VERSION=5.0.4
# Sun, 05 Feb 2023 02:18:40 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Sun, 05 Feb 2023 02:18:40 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Sun, 05 Feb 2023 02:18:46 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sun, 05 Feb 2023 02:22:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 05 Feb 2023 02:22:03 GMT
VOLUME [/usr/src/redmine/files]
# Sun, 05 Feb 2023 02:22:04 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Sun, 05 Feb 2023 02:22:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sun, 05 Feb 2023 02:22:05 GMT
EXPOSE 3000
# Sun, 05 Feb 2023 02:22:05 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:0604364135762a6c4b3503dd7f0396a51396443bf6052b34b8df7f67679b42c0`  
		Last Modified: Sat, 04 Feb 2023 12:32:12 GMT  
		Size: 35.3 MB (35268795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e992b80b310ac18fdf8e607400274d8448c18f75bc01ac3f69850a0c8a27ce`  
		Last Modified: Sat, 04 Feb 2023 17:12:37 GMT  
		Size: 10.5 MB (10477875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f2b9156337f87996a62dbec8ea14b353cfe8ba10f062eb48f83ed22507dc1e`  
		Last Modified: Sat, 04 Feb 2023 17:12:33 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8999b5bc90abf8884ec64fa8b0a7093cd243a4bb1a26ef5ac8b7f422f948db`  
		Last Modified: Sat, 04 Feb 2023 17:13:29 GMT  
		Size: 32.8 MB (32793370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b3adea8540a375dcf440764f9fca12ace4e4d0e7a8826c16fdba8f0238946a`  
		Last Modified: Sat, 04 Feb 2023 17:13:23 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de2c0aab041844b3f74ce1b692c08b8c98dff72fd3f4b7ac96a5b5db58c7c281`  
		Last Modified: Sun, 05 Feb 2023 02:29:09 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e816bf5d31f219b26545626bfa2e562865841df07c434720260a46aa7b2117d7`  
		Last Modified: Sun, 05 Feb 2023 02:29:37 GMT  
		Size: 107.5 MB (107516352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401249fac494d7ce585fef13f49d50c8b7d174706214e1afd24a455363b0d996`  
		Last Modified: Sun, 05 Feb 2023 02:29:07 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13429fd08454d5894b5453ca8041b6db55d68e1f902bf3cc0bb947cfd74bd161`  
		Last Modified: Sun, 05 Feb 2023 02:29:07 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d27a4296d609c0cf57b71b6898ff76ddd2e6aa2107eb838c177f2112a88dca6`  
		Last Modified: Sun, 05 Feb 2023 02:29:08 GMT  
		Size: 3.1 MB (3143016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01abe9a217c1fc94a3ac934551719e955f3ee904e07f794c440fbb9e7952bfe`  
		Last Modified: Sun, 05 Feb 2023 02:29:20 GMT  
		Size: 73.4 MB (73398025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05a4bd8c37a59ff4ddbb1475d3061eebf475120e88dae3280b85135702370e3`  
		Last Modified: Sun, 05 Feb 2023 02:29:07 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; s390x

```console
$ docker pull redmine@sha256:5a1b558130a873654a3935ed8f1f97a90bcebdd00fb1b5a4de7a6feed745e974
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.3 MB (246268578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b353bd3afc49bf5229a7b38b9606e8451b24152bc75c688dc7e524d1c38b9f5c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Sat, 04 Feb 2023 04:06:15 GMT
ADD file:29a3ecb38611dbbb6f45b2d10ad3cee60c0198429376f999e9a397f9c405820e in / 
# Sat, 04 Feb 2023 04:06:17 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:51:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:51:14 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 04 Feb 2023 10:51:14 GMT
ENV LANG=C.UTF-8
# Sat, 04 Feb 2023 10:55:41 GMT
ENV RUBY_MAJOR=3.1
# Sat, 04 Feb 2023 10:55:41 GMT
ENV RUBY_VERSION=3.1.3
# Sat, 04 Feb 2023 10:55:41 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Sat, 04 Feb 2023 10:57:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 04 Feb 2023 10:57:55 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 04 Feb 2023 10:57:55 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 04 Feb 2023 10:57:55 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 10:57:56 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 04 Feb 2023 10:57:56 GMT
CMD ["irb"]
# Sat, 04 Feb 2023 16:41:54 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sat, 04 Feb 2023 16:42:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 16:42:24 GMT
ENV RAILS_ENV=production
# Sat, 04 Feb 2023 16:42:24 GMT
WORKDIR /usr/src/redmine
# Sat, 04 Feb 2023 16:42:24 GMT
ENV HOME=/home/redmine
# Sat, 04 Feb 2023 16:42:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Sat, 04 Feb 2023 16:42:24 GMT
ENV REDMINE_VERSION=5.0.4
# Sat, 04 Feb 2023 16:42:25 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Sat, 04 Feb 2023 16:42:25 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Sat, 04 Feb 2023 16:42:27 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Sat, 04 Feb 2023 16:43:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 16:43:50 GMT
VOLUME [/usr/src/redmine/files]
# Sat, 04 Feb 2023 16:43:50 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Sat, 04 Feb 2023 16:43:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 04 Feb 2023 16:43:50 GMT
EXPOSE 3000
# Sat, 04 Feb 2023 16:43:50 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:7c6fe4d1ef15da79055e0a71952e1a38f799d4f36e9acebdb1ec1512651b39f1`  
		Last Modified: Sat, 04 Feb 2023 04:10:27 GMT  
		Size: 29.6 MB (29629678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe7607a7a328d85c5c480afaf63c416b114c5ee8361a3f20c3a7599e18054a4`  
		Last Modified: Sat, 04 Feb 2023 11:08:38 GMT  
		Size: 8.9 MB (8861196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9b129a75dbec0241ae1ab81941ca557646f6f5fe1212e910cab77f60b91d76`  
		Last Modified: Sat, 04 Feb 2023 11:08:37 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad7ead632992731bc66d721a3a2433934d7f9150c193616092866d535d37f83`  
		Last Modified: Sat, 04 Feb 2023 11:09:19 GMT  
		Size: 32.4 MB (32435706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4daecfbb7aebf7eaa68c8fd4b27b40f9f9232c51dd9b85f96a9d5965c57aee`  
		Last Modified: Sat, 04 Feb 2023 11:09:16 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5482e680666578af1bc4580087a4d8081b60275585f071762963fad44bdb70`  
		Last Modified: Sat, 04 Feb 2023 16:47:18 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b7404ac653d71f0d875e91e8558e8c0efb1e0d2775d455a42169933d483d3f`  
		Last Modified: Sat, 04 Feb 2023 16:47:32 GMT  
		Size: 99.2 MB (99176300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8fc6b6390fe5aee7ade0d8ca86ee79d98c6e3739521aceacccdb3866cc5c05`  
		Last Modified: Sat, 04 Feb 2023 16:47:17 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:223ee172f425bbecd3b653fdb312f02ddeed47a792268532b035800936df2acb`  
		Last Modified: Sat, 04 Feb 2023 16:47:17 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778438c041bdb2b1e2cb15f33f76b0f10de13df942f2ea40e7792f3fd9c0e3c7`  
		Last Modified: Sat, 04 Feb 2023 16:47:18 GMT  
		Size: 3.1 MB (3143016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a9f7a5f67f328999f54e13addc600248d9cb06cebc357ef7b3dbd79317053ca`  
		Last Modified: Sat, 04 Feb 2023 16:47:24 GMT  
		Size: 73.0 MB (73018220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713a58c470e60c4b0efe6167aa6ce5d05687e8418baf8879cdc685efd2998e7e`  
		Last Modified: Sat, 04 Feb 2023 16:47:17 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
