## `redmine:5-bullseye`

```console
$ docker pull redmine@sha256:0c9c6b9b018ccc173cf484597a9cdcc55b203862052ff92b85fbd0c1f4a37083
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
$ docker pull redmine@sha256:47a669deee43b5bf9881a6ee9b35185cd710b68bfaec59ea34485a2bf86d6975
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.5 MB (240507024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28dddd6f45f3bcb56cdcba446b3c0b4ae2a052de832e64db90016cba1cc350fa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 21 Dec 2022 01:20:32 GMT
ADD file:73e68ae6852c9afbb2989dc9c5b7c6668843f454b1bdcfb48658bfbc6c4af69e in / 
# Wed, 21 Dec 2022 01:20:33 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 10:08:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 10:08:10 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 21 Dec 2022 10:08:10 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 10:14:25 GMT
ENV RUBY_MAJOR=3.1
# Wed, 21 Dec 2022 10:14:25 GMT
ENV RUBY_VERSION=3.1.3
# Wed, 21 Dec 2022 10:14:25 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Wed, 21 Dec 2022 10:16:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 21 Dec 2022 10:16:50 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 21 Dec 2022 10:16:50 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 21 Dec 2022 10:16:50 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 10:16:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 21 Dec 2022 10:16:50 GMT
CMD ["irb"]
# Wed, 21 Dec 2022 16:01:11 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 21 Dec 2022 16:01:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 16:01:42 GMT
ENV RAILS_ENV=production
# Wed, 21 Dec 2022 16:01:42 GMT
WORKDIR /usr/src/redmine
# Wed, 21 Dec 2022 16:01:42 GMT
ENV HOME=/home/redmine
# Wed, 21 Dec 2022 16:01:43 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 21 Dec 2022 16:01:43 GMT
ENV REDMINE_VERSION=5.0.4
# Wed, 21 Dec 2022 16:01:43 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Wed, 21 Dec 2022 16:01:43 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Wed, 21 Dec 2022 16:01:46 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 21 Dec 2022 16:02:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 16:02:19 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 21 Dec 2022 16:02:19 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Wed, 21 Dec 2022 16:02:19 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 16:02:19 GMT
EXPOSE 3000
# Wed, 21 Dec 2022 16:02:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3f4ca61aafcd4fc07267a105067db35c0f0ac630e1970f3cd0c7bf552780e985`  
		Last Modified: Wed, 21 Dec 2022 01:24:36 GMT  
		Size: 31.4 MB (31396943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c1347bf51c53a765c0fe4414697505ac758faa26c11a340f06b6dfeaa1934be`  
		Last Modified: Wed, 21 Dec 2022 10:30:23 GMT  
		Size: 10.0 MB (10019713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a72f1f78ce7686ff2bbaa353683b7a65bba6686dfcf86046f9a6de8069858de`  
		Last Modified: Wed, 21 Dec 2022 10:30:21 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf4af2fbbcead5e76a1e429563c3589ebe5ec711392714b989a68b8a7fc4ce8`  
		Last Modified: Wed, 21 Dec 2022 10:30:57 GMT  
		Size: 32.6 MB (32613396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b09efec1139fa4324b73b5a6881221c41ec5c3fc332fa451860c2a002bafa8de`  
		Last Modified: Wed, 21 Dec 2022 10:30:54 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ac28e99d170aa1ac38c96fae22079b3a692d70f39c34d12b4395c2f82ae7cc`  
		Last Modified: Wed, 21 Dec 2022 16:04:53 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae003e9ee1e312094f3c4f2dae169a34e01b9f2de12f7e3cd03adddddb3ef26`  
		Last Modified: Wed, 21 Dec 2022 16:05:09 GMT  
		Size: 102.0 MB (102020933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314400fb7f257f98fdc81ef12d36760a3e97ba3c72b6082648441f638dfb5bef`  
		Last Modified: Wed, 21 Dec 2022 16:04:51 GMT  
		Size: 173.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8703e3aa5633279a198bdd2ee2c1f3396ff69de98b78cea02f0214262ef15c`  
		Last Modified: Wed, 21 Dec 2022 16:04:51 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0340060639f7a32b27bc95aa21c61c52a025d04a5f735a880524ddf5e617b90`  
		Last Modified: Wed, 21 Dec 2022 16:04:52 GMT  
		Size: 3.1 MB (3143019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f11f0e2bf77a81c3045eb4c4a86af5ca15472468cfbe5d67ded3cd9599ae38`  
		Last Modified: Wed, 21 Dec 2022 16:04:58 GMT  
		Size: 61.3 MB (61308554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9006439316439481f223ed4396a5666ae9a40e95845a0bac47e70bd7b290a684`  
		Last Modified: Wed, 21 Dec 2022 16:04:51 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm variant v5

```console
$ docker pull redmine@sha256:877637b1f30cd46e63ff05b34e34468ab18a3d5062309cb34a33877a1a2d5d39
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **239.3 MB (239293528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b030c303e7fa36216545a77c42dcb823761a88ad6a958f16380f5c51bc87a285`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 21 Dec 2022 01:49:08 GMT
ADD file:89f7788ae38bc6c172614b734ff10cba90c89ee09ca0f1acccc185c1bec630a1 in / 
# Wed, 21 Dec 2022 01:49:09 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 09:20:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:20:46 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 21 Dec 2022 09:20:46 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 09:26:31 GMT
ENV RUBY_MAJOR=3.1
# Wed, 21 Dec 2022 09:26:31 GMT
ENV RUBY_VERSION=3.1.3
# Wed, 21 Dec 2022 09:26:31 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Wed, 21 Dec 2022 09:29:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 21 Dec 2022 09:29:03 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 21 Dec 2022 09:29:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 21 Dec 2022 09:29:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 09:29:04 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 21 Dec 2022 09:29:04 GMT
CMD ["irb"]
# Wed, 21 Dec 2022 15:39:05 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 21 Dec 2022 15:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 15:39:40 GMT
ENV RAILS_ENV=production
# Wed, 21 Dec 2022 15:39:40 GMT
WORKDIR /usr/src/redmine
# Wed, 21 Dec 2022 15:39:40 GMT
ENV HOME=/home/redmine
# Wed, 21 Dec 2022 15:39:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 21 Dec 2022 15:39:41 GMT
ENV REDMINE_VERSION=5.0.4
# Wed, 21 Dec 2022 15:39:41 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Wed, 21 Dec 2022 15:39:41 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Wed, 21 Dec 2022 15:39:44 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 21 Dec 2022 15:41:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 15:41:38 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 21 Dec 2022 15:41:38 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Wed, 21 Dec 2022 15:41:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 15:41:38 GMT
EXPOSE 3000
# Wed, 21 Dec 2022 15:41:39 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6addfee759f2774f92392906ab5b50ba2f4a14314858c502e856f7d7de2a7e07`  
		Last Modified: Wed, 21 Dec 2022 01:54:03 GMT  
		Size: 28.9 MB (28898607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dd7fa9668cbd75861f2451bd50e3e30e0fe4837c5f34395f7db5e503ba698a`  
		Last Modified: Wed, 21 Dec 2022 09:40:55 GMT  
		Size: 8.6 MB (8633589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa75426820dd8f9cdb65138218c0c09d571c75c7cea6680b483384938939bd6`  
		Last Modified: Wed, 21 Dec 2022 09:40:53 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db469348094a12c79a9fb8f5dc8eaddb671fc6e5a54b71423ab2f3008648e95`  
		Last Modified: Wed, 21 Dec 2022 09:41:50 GMT  
		Size: 31.2 MB (31161485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b86167e1b110a8852893c5ccc0b4faa1a72eaee8b44744137836b8808e3bb5`  
		Last Modified: Wed, 21 Dec 2022 09:41:46 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735cd35b175ad3f27c20cf91ed36beb3639e8ebd45ca032e79b8403c54c70fdd`  
		Last Modified: Wed, 21 Dec 2022 15:45:25 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977150fbef417ead22ca30e1d8b4c43bfd54a0d0f9e084d8eb0671c3143a5bd2`  
		Last Modified: Wed, 21 Dec 2022 15:45:45 GMT  
		Size: 97.0 MB (96986513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69d1cd5fa895618a3c5e3ada84297420378fcd237c1779d62cb08ba9cf03860`  
		Last Modified: Wed, 21 Dec 2022 15:45:23 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0abc2a854040c7ca3a53662d14bffcecf308fac08212161393deaccfbcc5e53`  
		Last Modified: Wed, 21 Dec 2022 15:45:23 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9fd9f0055bfabaa5b29ca45e2d6d18e3cb48eb1db9d68f48083615b2b1bf27`  
		Last Modified: Wed, 21 Dec 2022 15:45:25 GMT  
		Size: 3.1 MB (3142674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6704f9f3e005dff82095cf3c4f59b6d321a1f5ae4d7f68a2147a513a98e6fe7`  
		Last Modified: Wed, 21 Dec 2022 15:45:33 GMT  
		Size: 70.5 MB (70466304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1dc7a7320529d67e7db1781543a65b86ec30ac8f7cb8e45780f6ba0ae808968`  
		Last Modified: Wed, 21 Dec 2022 15:45:23 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm variant v7

```console
$ docker pull redmine@sha256:d59d0f122c850ca98bb51ef82ed628f1cee2bfc2fb11ff173f8eb61b96e530b4
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.0 MB (232033768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a7c1116f34d48f38de8f75186766d0621905539944770a6cf48d158c539bc9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 06 Dec 2022 00:58:51 GMT
ADD file:cb354f875d5631d5d4542ab57d0b9b323a261f5c631d5917127504d6eb54d85a in / 
# Tue, 06 Dec 2022 00:58:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 12:50:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 12:50:11 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 06 Dec 2022 12:50:12 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 13:00:05 GMT
ENV RUBY_MAJOR=3.1
# Tue, 06 Dec 2022 13:00:05 GMT
ENV RUBY_VERSION=3.1.3
# Tue, 06 Dec 2022 13:00:05 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Tue, 06 Dec 2022 13:02:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 06 Dec 2022 13:02:24 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 06 Dec 2022 13:02:24 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 06 Dec 2022 13:02:24 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 13:02:25 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 06 Dec 2022 13:02:25 GMT
CMD ["irb"]
# Wed, 07 Dec 2022 03:18:50 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 07 Dec 2022 03:19:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 07 Dec 2022 03:19:19 GMT
ENV RAILS_ENV=production
# Wed, 07 Dec 2022 03:19:20 GMT
WORKDIR /usr/src/redmine
# Wed, 07 Dec 2022 03:19:20 GMT
ENV HOME=/home/redmine
# Wed, 07 Dec 2022 03:19:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 07 Dec 2022 03:19:20 GMT
ENV REDMINE_VERSION=5.0.4
# Wed, 07 Dec 2022 03:19:20 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Wed, 07 Dec 2022 03:19:20 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Wed, 07 Dec 2022 03:19:24 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 07 Dec 2022 03:21:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 07 Dec 2022 03:21:03 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 07 Dec 2022 03:21:03 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Wed, 07 Dec 2022 03:21:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 07 Dec 2022 03:21:03 GMT
EXPOSE 3000
# Wed, 07 Dec 2022 03:21:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:4f32a98d14d26603bb8e8cf9bda992e24606d2fe00101767049a01d5176929e1`  
		Last Modified: Tue, 06 Dec 2022 01:06:05 GMT  
		Size: 26.6 MB (26576348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1829ddfbb7412785849a7bc642891c9941e4405c63bce3ed75b5baf09db48e53`  
		Last Modified: Tue, 06 Dec 2022 13:28:43 GMT  
		Size: 8.1 MB (8142816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d76deae3c66382a31903668fef3c6d6d1eec2332c431b39a892e65c133c4d3`  
		Last Modified: Tue, 06 Dec 2022 13:28:40 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e61666cd5577e332b7b95673f6a9e4c1866afff94adddb6956c4fe5502435a`  
		Last Modified: Tue, 06 Dec 2022 13:30:23 GMT  
		Size: 31.0 MB (31019743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c80fa884adb20fae43157bd05c90caed0703e3a8bef3787880ec7d8122b6eb`  
		Last Modified: Tue, 06 Dec 2022 13:30:18 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9077a0dd78afd5320c8bcf2fc2fa7f01a4fe1a1279b005c7c4cd96acf1e412d8`  
		Last Modified: Wed, 07 Dec 2022 03:25:32 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:849d2229cb99ffe6efe212e44389bccb47ead639a68f778a2a55d87183f348eb`  
		Last Modified: Wed, 07 Dec 2022 03:25:49 GMT  
		Size: 93.1 MB (93134401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1950ea8d10c2d2f096d0a6bc598ba73f74a47dd5b9c7a81384b8518e5a79e6aa`  
		Last Modified: Wed, 07 Dec 2022 03:25:30 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e59dc87265380526ab749be540148c26a7ef0619dd328e2108298aff2266582`  
		Last Modified: Wed, 07 Dec 2022 03:25:30 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32c87b0f6d808de766286cd4a14e0148123e4cb40eda565effb2276f1119a53`  
		Last Modified: Wed, 07 Dec 2022 03:25:31 GMT  
		Size: 3.1 MB (3142673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3b3964271680aaf857b2c2e167603175927bab69d72c09891650ab8318f23d`  
		Last Modified: Wed, 07 Dec 2022 03:25:39 GMT  
		Size: 70.0 MB (70013435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:235f08e4a54bdb91ea87e17c9c3ee4b51ac870a5d2191f9ec0e8cf02e9ae0167`  
		Last Modified: Wed, 07 Dec 2022 03:25:30 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:8e9448f64ffc1eb46e5d7397ec48e4fbabf02a0ad856c2684701441afd85d8ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.8 MB (234801759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a786b88f21fba00c3b19759e707a390ba16210a2639c7782824e54e2b11a3475`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 06 Dec 2022 01:40:17 GMT
ADD file:379d6ac56afdb6e02d71fa0faebc13b8a2554fc6ae76c5f5bbdb5b8e475135d6 in / 
# Tue, 06 Dec 2022 01:40:17 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 13:00:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 13:00:27 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 06 Dec 2022 13:00:27 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 13:07:41 GMT
ENV RUBY_MAJOR=3.1
# Tue, 06 Dec 2022 13:07:41 GMT
ENV RUBY_VERSION=3.1.3
# Tue, 06 Dec 2022 13:07:41 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Tue, 06 Dec 2022 13:09:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 06 Dec 2022 13:09:23 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 06 Dec 2022 13:09:23 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 06 Dec 2022 13:09:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 13:09:24 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 06 Dec 2022 13:09:24 GMT
CMD ["irb"]
# Tue, 06 Dec 2022 20:04:30 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 06 Dec 2022 20:04:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 20:04:57 GMT
ENV RAILS_ENV=production
# Tue, 06 Dec 2022 20:04:58 GMT
WORKDIR /usr/src/redmine
# Tue, 06 Dec 2022 20:04:58 GMT
ENV HOME=/home/redmine
# Tue, 06 Dec 2022 20:04:58 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 06 Dec 2022 20:04:58 GMT
ENV REDMINE_VERSION=5.0.4
# Tue, 06 Dec 2022 20:04:58 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Tue, 06 Dec 2022 20:04:58 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Tue, 06 Dec 2022 20:05:01 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 06 Dec 2022 20:05:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 20:05:29 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 06 Dec 2022 20:05:29 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 06 Dec 2022 20:05:29 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 20:05:29 GMT
EXPOSE 3000
# Tue, 06 Dec 2022 20:05:29 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:6064e7e5b6afa4dc711228eddfd250aebac271830dc184c400ce640020bc2cb0`  
		Last Modified: Tue, 06 Dec 2022 01:43:56 GMT  
		Size: 30.1 MB (30060320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b35d881fa3be42425d38e36b65b32fe285d7d74b7a772e62b932aa139d3f0c`  
		Last Modified: Tue, 06 Dec 2022 13:26:45 GMT  
		Size: 9.2 MB (9242670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb3dfae78a18073ac38d4f8ef7719f44ea19e4e38b67d02f68c496b097fc41e`  
		Last Modified: Tue, 06 Dec 2022 13:26:43 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c67fe65949c57d7e42409c0e5da28aea12c8021cf8506d234fe260ea6d7872`  
		Last Modified: Tue, 06 Dec 2022 13:27:50 GMT  
		Size: 32.0 MB (31963442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7080b7370f3c7baf1e114a3951d2fd1998f680024fdd1d1f1479b5f6452698cd`  
		Last Modified: Tue, 06 Dec 2022 13:27:47 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0adbab555d84235c7c2699a97180122f3fd672adf3772052b6e75870bfa539`  
		Last Modified: Tue, 06 Dec 2022 20:07:24 GMT  
		Size: 1.7 KB (1745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77801468ec03ce995a5c9f70f8cffe5a133ff589cb4fd83a52fb81d805ee041d`  
		Last Modified: Tue, 06 Dec 2022 20:07:36 GMT  
		Size: 99.8 MB (99798545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a7d88bb496cb749628db3f2ed708ecc9cb5afe6c0f5e9f286dbb69cafb1545`  
		Last Modified: Tue, 06 Dec 2022 20:07:22 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe6d0bfaf823003cdd2d7dcfc2272ec13f767882fee83f9ffc08c4949316aa5`  
		Last Modified: Tue, 06 Dec 2022 20:07:22 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462b9756cb274b5257905310c85e767515b82c4e4267c24fbc62b17886556700`  
		Last Modified: Tue, 06 Dec 2022 20:07:23 GMT  
		Size: 3.1 MB (3143007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13409e8ec5ee248dec816809cf9f4dfccddd8f8cb622a10ab603ba848775634e`  
		Last Modified: Tue, 06 Dec 2022 20:07:28 GMT  
		Size: 60.6 MB (60589314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04d0c5213a1e7598c6bea8d7eaf6700b6f48beaa6a602cf1283687363e0e85af`  
		Last Modified: Tue, 06 Dec 2022 20:07:22 GMT  
		Size: 2.0 KB (2014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; 386

```console
$ docker pull redmine@sha256:d5089ba1b36aa5edd1b57addea7bcda0df9feba74274e77653aff71c79375517
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.9 MB (241861247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7e69a8fa513e4c76caa29063efc5cc1330a6833463f40b045fa0d5810e2c8cd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 16:10:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 16:10:42 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 06 Dec 2022 16:10:42 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 16:20:30 GMT
ENV RUBY_MAJOR=3.1
# Tue, 06 Dec 2022 16:20:31 GMT
ENV RUBY_VERSION=3.1.3
# Tue, 06 Dec 2022 16:20:32 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Tue, 06 Dec 2022 16:22:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 06 Dec 2022 16:22:48 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 06 Dec 2022 16:22:48 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 06 Dec 2022 16:22:49 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 16:22:50 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 06 Dec 2022 16:22:51 GMT
CMD ["irb"]
# Tue, 06 Dec 2022 22:08:41 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 06 Dec 2022 22:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 22:09:13 GMT
ENV RAILS_ENV=production
# Tue, 06 Dec 2022 22:09:13 GMT
WORKDIR /usr/src/redmine
# Tue, 06 Dec 2022 22:09:14 GMT
ENV HOME=/home/redmine
# Tue, 06 Dec 2022 22:09:15 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 06 Dec 2022 22:09:16 GMT
ENV REDMINE_VERSION=5.0.4
# Tue, 06 Dec 2022 22:09:17 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Tue, 06 Dec 2022 22:09:18 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Tue, 06 Dec 2022 22:09:22 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 06 Dec 2022 22:09:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 22:09:56 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 06 Dec 2022 22:09:58 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 06 Dec 2022 22:09:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 22:09:59 GMT
EXPOSE 3000
# Tue, 06 Dec 2022 22:10:00 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca384dd6a73eee035883553041cebb38bc84a3d2d5c9843f7b1f933863fcb5f7`  
		Last Modified: Tue, 06 Dec 2022 16:47:37 GMT  
		Size: 11.8 MB (11788280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc77a7a274ce31f64644ada4ab011a7a40ec1276d0618cd07871bb859c2046db`  
		Last Modified: Tue, 06 Dec 2022 16:47:35 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c074e75f3a0d9af5df34dc5884935d2b5e01692efe51298e3b5fdbdd27b1fa32`  
		Last Modified: Tue, 06 Dec 2022 16:49:09 GMT  
		Size: 30.9 MB (30948964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b29fd04593371ba0c12c006c1ea55b74a1c3acb2ad1034d27d8c53de019065`  
		Last Modified: Tue, 06 Dec 2022 16:49:07 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71cc7ac01b94e0ae8db375fc19e49b54bd5722d004c931beb3d2dc409b0659`  
		Last Modified: Tue, 06 Dec 2022 22:12:58 GMT  
		Size: 1.6 KB (1615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526afdd343f2eac5f7b6978457172be64bfee4ef4b03d40ca45f2efbe39469f1`  
		Last Modified: Tue, 06 Dec 2022 22:13:14 GMT  
		Size: 103.4 MB (103355413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c7776070d5a33f9fdc9a337780ee783245e7a3a61ae506b05510a6eb2e8cda`  
		Last Modified: Tue, 06 Dec 2022 22:12:56 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48126cd9e6089b247491c308fe12212144e20e3ad21e73b36488e9720945252`  
		Last Modified: Tue, 06 Dec 2022 22:12:56 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d9dd36b0bd4d6b10975554b24b884ac49d5cde5e7cbe19bd40f873094205d`  
		Last Modified: Tue, 06 Dec 2022 22:12:57 GMT  
		Size: 3.1 MB (3142887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc1812ac77bd6d7ee543915f5ab061a743c7dc9aa68a043ad7d12d49814df25`  
		Last Modified: Tue, 06 Dec 2022 22:13:04 GMT  
		Size: 60.2 MB (60228423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e931e04b12fc4f438a76c21d54e043ae839a505248ecf68dbcba62912fb56f55`  
		Last Modified: Tue, 06 Dec 2022 22:12:56 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; ppc64le

```console
$ docker pull redmine@sha256:2482abc38eb11bab99f598472dc2bd449738701b0edca518fee1a17130086a9c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.5 MB (262485274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc07e4fcae77c019ec2c7f0f03364d81653a35607c2da3ad9504d214dadeb112`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 06 Dec 2022 01:18:04 GMT
ADD file:2231a44ea52d93df58e23883ba6b6911d4c554f4c1d172d80fb21c751ddcbbfc in / 
# Tue, 06 Dec 2022 01:18:06 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 09:35:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 09:35:48 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 06 Dec 2022 09:35:48 GMT
ENV LANG=C.UTF-8
# Tue, 06 Dec 2022 09:43:01 GMT
ENV RUBY_MAJOR=3.1
# Tue, 06 Dec 2022 09:43:01 GMT
ENV RUBY_VERSION=3.1.3
# Tue, 06 Dec 2022 09:43:02 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Tue, 06 Dec 2022 09:47:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 06 Dec 2022 09:47:14 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 06 Dec 2022 09:47:14 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 06 Dec 2022 09:47:14 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Dec 2022 09:47:16 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 06 Dec 2022 09:47:16 GMT
CMD ["irb"]
# Tue, 06 Dec 2022 21:39:07 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 06 Dec 2022 21:40:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 21:40:17 GMT
ENV RAILS_ENV=production
# Tue, 06 Dec 2022 21:40:18 GMT
WORKDIR /usr/src/redmine
# Tue, 06 Dec 2022 21:40:18 GMT
ENV HOME=/home/redmine
# Tue, 06 Dec 2022 21:40:20 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 06 Dec 2022 21:40:20 GMT
ENV REDMINE_VERSION=5.0.4
# Tue, 06 Dec 2022 21:40:21 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Tue, 06 Dec 2022 21:40:21 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Tue, 06 Dec 2022 21:40:26 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 06 Dec 2022 21:43:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 21:43:32 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 06 Dec 2022 21:43:32 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Tue, 06 Dec 2022 21:43:32 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 06 Dec 2022 21:43:32 GMT
EXPOSE 3000
# Tue, 06 Dec 2022 21:43:33 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:1f72e1168976861c676bf86a6c149129baba7e13200e8b70e6f24dc2ac2797df`  
		Last Modified: Tue, 06 Dec 2022 01:24:18 GMT  
		Size: 35.3 MB (35285293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcb5a302d4619db0220eecbb90cb7cf33297235cdec6cae64a7cb030cdeae4c`  
		Last Modified: Tue, 06 Dec 2022 10:03:35 GMT  
		Size: 10.5 MB (10478730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf885d002681bd6d3d6e8d2f966f5c691791a7ea93fa44205582b2fd53eb3a89`  
		Last Modified: Tue, 06 Dec 2022 10:03:31 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8309f6fcca41caa6d19a2210dac23646c13a8306fb49dabdaf33c547d089f6e0`  
		Last Modified: Tue, 06 Dec 2022 10:04:39 GMT  
		Size: 32.8 MB (32774673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78754ffb6dba7787a1ab454ece614e1ee04be6e99862c1fca7195b66c22c691a`  
		Last Modified: Tue, 06 Dec 2022 10:04:33 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c16a5d8936f1e673cf8547cb1c4baf0fc39cbd96cdac5567f4ea52c3b40a84`  
		Last Modified: Tue, 06 Dec 2022 21:49:54 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54a8c73385d689bd6f9265b121ac8bbaccf89e7a867d2a0762e7440a663a08d`  
		Last Modified: Tue, 06 Dec 2022 21:50:22 GMT  
		Size: 107.5 MB (107520345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b69a2626807f536f6bb2a1b3617e75e7eb185089bedb829f314c9e0377679c`  
		Last Modified: Tue, 06 Dec 2022 21:49:52 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26abf6bc0af9bf5bcc6ac871c9efeae696c1aeeabfc136f869dae1c9b7d2bd47`  
		Last Modified: Tue, 06 Dec 2022 21:49:52 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c28f9b95279e4e5f738dae4971b843228899f9630cc57a9d5ff40738d9d025bc`  
		Last Modified: Tue, 06 Dec 2022 21:49:53 GMT  
		Size: 3.1 MB (3143009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ab6829e044a34a703663609aeae8ee36105d036ebe151283c7da4023b3d5dd`  
		Last Modified: Tue, 06 Dec 2022 21:50:05 GMT  
		Size: 73.3 MB (73278767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccaa9a4bdcaf2c22c809cfd36a78a893806c7bf22786f285ddd8257276a96c8`  
		Last Modified: Tue, 06 Dec 2022 21:49:51 GMT  
		Size: 2.0 KB (2013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:5-bullseye` - linux; s390x

```console
$ docker pull redmine@sha256:eaa4c559d8d6c37650e96e05b9ce6488422a64969b988b72697818579605b66e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.3 MB (246293264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f278ba6fd2e710a1e48f0671f9002a335c55d2e45e7fb0d8f0f1c4b8dc3088ad`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Wed, 21 Dec 2022 01:43:11 GMT
ADD file:c1d41928e802c0b63beb07130c33bcc6dbdeb380a7f47510163cb176891e682a in / 
# Wed, 21 Dec 2022 01:43:14 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:46:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:46:58 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 21 Dec 2022 04:46:59 GMT
ENV LANG=C.UTF-8
# Wed, 21 Dec 2022 04:52:17 GMT
ENV RUBY_MAJOR=3.1
# Wed, 21 Dec 2022 04:52:18 GMT
ENV RUBY_VERSION=3.1.3
# Wed, 21 Dec 2022 04:52:19 GMT
ENV RUBY_DOWNLOAD_SHA256=4ee161939826bcdfdafa757cf8e293a7f14e357f62be7144f040335cc8c7371a
# Wed, 21 Dec 2022 04:56:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 21 Dec 2022 04:56:06 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 21 Dec 2022 04:56:07 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 21 Dec 2022 04:56:07 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 21 Dec 2022 04:56:09 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 21 Dec 2022 04:56:09 GMT
CMD ["irb"]
# Wed, 21 Dec 2022 11:22:28 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 21 Dec 2022 11:23:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 11:24:05 GMT
ENV RAILS_ENV=production
# Wed, 21 Dec 2022 11:24:05 GMT
WORKDIR /usr/src/redmine
# Wed, 21 Dec 2022 11:24:06 GMT
ENV HOME=/home/redmine
# Wed, 21 Dec 2022 11:24:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 21 Dec 2022 11:24:08 GMT
ENV REDMINE_VERSION=5.0.4
# Wed, 21 Dec 2022 11:24:09 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-5.0.4.tar.gz
# Wed, 21 Dec 2022 11:24:09 GMT
ENV REDMINE_DOWNLOAD_SHA256=39436f5f8d26f5b7ce17e79903a3112e556e924da4f51c05b57f5defbe6f2924
# Wed, 21 Dec 2022 11:24:16 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 21 Dec 2022 11:26:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 21 Dec 2022 11:26:49 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 21 Dec 2022 11:26:50 GMT
COPY file:f61e8718e722eba56748d9a7e58011159861fb49784b1ad721746c1fc5735b6d in / 
# Wed, 21 Dec 2022 11:26:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 21 Dec 2022 11:26:50 GMT
EXPOSE 3000
# Wed, 21 Dec 2022 11:26:51 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:197dcf20f55386b4c3f5fbace4720b64b5b0b606658b4ea9925121b9dbe7d638`  
		Last Modified: Wed, 21 Dec 2022 01:49:12 GMT  
		Size: 29.6 MB (29629760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd387a7ef8d2520ba9db31762bad0c6bf601a26c45891a0d4a7c9f454efba8d`  
		Last Modified: Wed, 21 Dec 2022 05:07:21 GMT  
		Size: 8.9 MB (8860201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9e40ac5a3d42e87a8535e1acc0d1bc0cb04466cc663868cd2a7b539ad491a5`  
		Last Modified: Wed, 21 Dec 2022 05:07:20 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13b4ecc6d7a3e32af4c54233e35f8d12f858cd52e82c912c67a6bce057334cc`  
		Last Modified: Wed, 21 Dec 2022 05:07:49 GMT  
		Size: 32.4 MB (32435843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e78e9d6a4141da288a1965fad026fbb95b82c6da8f93331323f199e52b0b54`  
		Last Modified: Wed, 21 Dec 2022 05:07:46 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7842b2377fa8cee173f8723b654183d99a404a6a8bcc73c539623178cc395ca`  
		Last Modified: Wed, 21 Dec 2022 11:32:31 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:610f1bd36631c9acccaa34f47700d2ae830e8c4f29f2234fbb33813665aca901`  
		Last Modified: Wed, 21 Dec 2022 11:32:46 GMT  
		Size: 99.2 MB (99156741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c297809891258dd22d02cd2e00d82e1827628739fc9781c636360bdca6a8edb0`  
		Last Modified: Wed, 21 Dec 2022 11:32:32 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694b762a1c21368ccd215a0e8e10036e3a8a2bab74d0f0e09a9342a2d4311323`  
		Last Modified: Wed, 21 Dec 2022 11:32:30 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9954373ecc6af6fa8566c393c7d15fde8cd82829a8f358e72bf64033cce958b7`  
		Last Modified: Wed, 21 Dec 2022 11:32:31 GMT  
		Size: 3.1 MB (3143015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830f5c41a63f958d72407ea4dcd1d5041c10088f6ffb3dc2217ab1bce0366975`  
		Last Modified: Wed, 21 Dec 2022 11:32:38 GMT  
		Size: 73.1 MB (73063238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce697572ae90bc459682b8382aff285c3e1544a472d768772dbd31c94864f83`  
		Last Modified: Wed, 21 Dec 2022 11:32:30 GMT  
		Size: 2.0 KB (2012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
