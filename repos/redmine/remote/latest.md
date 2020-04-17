## `redmine:latest`

```console
$ docker pull redmine@sha256:a022b780f436f49462c6b78016a5c34227f20e93b5b53d10a507e08a05a192a6
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
$ docker pull redmine@sha256:ac15236e5978bd45008e057f047a3bfe914bfd45930e8cb5de5f279f254b6555
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.2 MB (216235192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:441d51cdf4b91d71e6b9ab55f7ec0fd1e502e82737732b6c9614c76237a2b97e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Mar 2020 01:21:01 GMT
ADD file:d1f1b387a158136fb0f8096c8a8ecf5fc146be4e85c1c3c345d44c927692723a in / 
# Tue, 31 Mar 2020 01:21:01 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 13:56:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 13:56:15 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 31 Mar 2020 14:04:39 GMT
ENV RUBY_MAJOR=2.6
# Wed, 01 Apr 2020 02:53:56 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 01 Apr 2020 02:53:56 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 01 Apr 2020 02:56:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Apr 2020 02:56:45 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Apr 2020 02:56:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Apr 2020 02:56:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Apr 2020 02:56:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Apr 2020 02:56:47 GMT
CMD ["irb"]
# Wed, 01 Apr 2020 03:52:00 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 01 Apr 2020 03:52:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 03:52:55 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Apr 2020 03:52:55 GMT
ENV RAILS_ENV=production
# Wed, 01 Apr 2020 03:52:55 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Apr 2020 03:52:55 GMT
ENV HOME=/home/redmine
# Wed, 01 Apr 2020 03:52:56 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 06 Apr 2020 20:55:22 GMT
ENV REDMINE_VERSION=4.1.1
# Mon, 06 Apr 2020 20:55:22 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Mon, 06 Apr 2020 20:55:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 06 Apr 2020 20:57:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 06 Apr 2020 20:57:55 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 06 Apr 2020 20:57:55 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Mon, 06 Apr 2020 20:57:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:57:56 GMT
EXPOSE 3000
# Mon, 06 Apr 2020 20:57:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:c499e6d256d6d4a546f1c141e04b5b4951983ba7581e39deaf5cc595289ee70f`  
		Last Modified: Tue, 31 Mar 2020 01:26:37 GMT  
		Size: 27.1 MB (27091862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e516c92236d13d90b1c0753be9b2e008c29aa333e89444af60037d29b28912f`  
		Last Modified: Tue, 31 Mar 2020 14:58:49 GMT  
		Size: 12.5 MB (12539789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4698a33c221b13798e4c082d9372980bdf8ee8f8c58cf4af2c5757c10e3ae2c0`  
		Last Modified: Tue, 31 Mar 2020 14:58:45 GMT  
		Size: 201.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617645a7ddaa34752abc3ee2c5586abf98895b004c790d59a3d7ec1f2f718f8a`  
		Last Modified: Wed, 01 Apr 2020 03:49:24 GMT  
		Size: 21.4 MB (21449550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c2e3e89af758929289a94322b5b1bbb637c216dddf54e1d26e418878c80ff7`  
		Last Modified: Wed, 01 Apr 2020 03:49:21 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010fc1e6363f092d0f2e6d1b0ca635d12ccdebe7f82dff00146913ea9b942188`  
		Last Modified: Wed, 01 Apr 2020 04:09:18 GMT  
		Size: 1.8 KB (1750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ecfe61351827ebc4c2f791c243134045a99e8d9e5a9bb4ef339b9860e3f71e`  
		Last Modified: Wed, 01 Apr 2020 04:09:36 GMT  
		Size: 93.1 MB (93059347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fc86fc655c3c7bce52eec063b3b45a7ec8e3a11d6df8040e2a49dad1961949`  
		Last Modified: Wed, 01 Apr 2020 04:09:19 GMT  
		Size: 1.3 MB (1307575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350b7794ab73190852d35513647d43a4003986a470e7532905085e5e84cea7a1`  
		Last Modified: Wed, 01 Apr 2020 04:09:17 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0e4ebba51362a9951a17a614159961816bc17a066999da9bec838d9d24fb60`  
		Last Modified: Wed, 01 Apr 2020 04:09:17 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9ac2f118449659196f70459f85b4391b9dfe6a36e4d98aefd2efd936999789`  
		Last Modified: Mon, 06 Apr 2020 21:10:13 GMT  
		Size: 2.7 MB (2739482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a26abcb82159ee08bbbe02dc148ed0e2fc89263f679f023c29fae17ecba571`  
		Last Modified: Mon, 06 Apr 2020 21:10:20 GMT  
		Size: 58.0 MB (58043173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532b6025d3a5644e41912117e322139b71b5cb21588590ff675bac0744d2b43b`  
		Last Modified: Mon, 06 Apr 2020 21:10:12 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v5

```console
$ docker pull redmine@sha256:902089fed6194c1a0ef1bc78b77eaf56546daae14856235d071187db7e323fa4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204931815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3792e569b3df96dbea898ec39187cd02e12154e71c01abfcb62ce805984027`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 16 Apr 2020 00:50:14 GMT
ADD file:761a556ec2a7d8c742c860e429c9b9ba3f7abfcd9383c6b3767499de6dcad4bc in / 
# Thu, 16 Apr 2020 00:50:15 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 07:08:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 07:08:08 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 16 Apr 2020 07:12:54 GMT
ENV RUBY_MAJOR=2.6
# Thu, 16 Apr 2020 07:12:56 GMT
ENV RUBY_VERSION=2.6.6
# Thu, 16 Apr 2020 07:12:57 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Thu, 16 Apr 2020 07:16:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 16 Apr 2020 07:16:42 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 16 Apr 2020 07:16:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 16 Apr 2020 07:16:43 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 07:16:45 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 16 Apr 2020 07:16:46 GMT
CMD ["irb"]
# Thu, 16 Apr 2020 14:08:22 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 16 Apr 2020 14:09:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 20:26:19 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Apr 2020 20:26:20 GMT
ENV RAILS_ENV=production
# Thu, 16 Apr 2020 20:26:21 GMT
WORKDIR /usr/src/redmine
# Thu, 16 Apr 2020 20:26:21 GMT
ENV HOME=/home/redmine
# Thu, 16 Apr 2020 20:26:24 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 16 Apr 2020 20:26:26 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 16 Apr 2020 20:26:27 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 16 Apr 2020 20:26:36 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 16 Apr 2020 20:31:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Apr 2020 20:31:16 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 16 Apr 2020 20:31:19 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 16 Apr 2020 20:31:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 20:31:25 GMT
EXPOSE 3000
# Thu, 16 Apr 2020 20:31:33 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:600369660a591bc9594fcf333a847fe997901785f7032d3ad2822b2812c13243`  
		Last Modified: Thu, 16 Apr 2020 00:58:26 GMT  
		Size: 24.8 MB (24836437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14b9f33c17decf0c70dba5a4b3b21f31261cca521bd0e0119004bc2b6a05211`  
		Last Modified: Thu, 16 Apr 2020 07:32:59 GMT  
		Size: 10.3 MB (10326015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30429f0a88e73dca727ed9eb0aa9dbb79556ab08e07eb1dc220ca6dbdda041b8`  
		Last Modified: Thu, 16 Apr 2020 07:32:55 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f138e7d1a8a2833e808ac8039c6a476c6d1c8ec692b75a91b510a26832bae6a2`  
		Last Modified: Thu, 16 Apr 2020 07:33:34 GMT  
		Size: 20.7 MB (20713518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51d11bc777a0d834c9caf4e839984f8f5740b5173916d14ec7c7b7de0d94c6c`  
		Last Modified: Thu, 16 Apr 2020 07:33:31 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17104567e8f4cbc8ebba701aa71318050fb9ede87ac59f6794f559912c99b79`  
		Last Modified: Thu, 16 Apr 2020 14:22:04 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698e55f70f5ba9524c4dc125767ba26df636c695bd85c7fa40c319962abae0a3`  
		Last Modified: Thu, 16 Apr 2020 14:22:34 GMT  
		Size: 88.7 MB (88682296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e23a60503d9f514e570ca1c7395655279bcb9fb4c891f4ab857c161483d40d`  
		Last Modified: Thu, 16 Apr 2020 20:38:37 GMT  
		Size: 1.3 MB (1325684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5923cdd7b29b01fbc11f08a648a2cac1518236926917bd4e17e1564da82d072a`  
		Last Modified: Thu, 16 Apr 2020 20:38:35 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c695d1d3225ec28a65720c781d794850611af4bc2cf02782c0504ba28e9f927f`  
		Last Modified: Thu, 16 Apr 2020 20:38:35 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b8ab84cbd2e64ef12854b4b853c43241341638b8c33fbb2fe60212f5e7963d0`  
		Last Modified: Thu, 16 Apr 2020 20:38:37 GMT  
		Size: 2.7 MB (2739765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0829332de8aef55d5db8677b74c878a95618f99376bb4d7f1c9900b6b5e746ba`  
		Last Modified: Thu, 16 Apr 2020 20:38:50 GMT  
		Size: 56.3 MB (56303605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a70d1064e32bcc7aaf28c17f71af75de98edcaed584af7f739456b35fc0247d8`  
		Last Modified: Thu, 16 Apr 2020 20:38:35 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm variant v7

```console
$ docker pull redmine@sha256:cd36c50055512402d6c89219e292e0aaa65509d062e79bff0f50241239f0ea60
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.0 MB (198030884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6daa4c4fc13528920754ba6416265be3c91ec35f9c77135980fcaf6bd73cf11e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 17:31:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 17:31:24 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 16 Apr 2020 17:47:52 GMT
ENV RUBY_MAJOR=2.6
# Thu, 16 Apr 2020 17:47:53 GMT
ENV RUBY_VERSION=2.6.6
# Thu, 16 Apr 2020 17:47:54 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Thu, 16 Apr 2020 17:51:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 16 Apr 2020 17:51:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 16 Apr 2020 17:51:22 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 16 Apr 2020 17:51:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 17:51:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 16 Apr 2020 17:51:26 GMT
CMD ["irb"]
# Fri, 17 Apr 2020 10:11:49 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 17 Apr 2020 10:13:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 10:13:26 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 17 Apr 2020 10:13:27 GMT
ENV RAILS_ENV=production
# Fri, 17 Apr 2020 10:13:29 GMT
WORKDIR /usr/src/redmine
# Fri, 17 Apr 2020 10:13:30 GMT
ENV HOME=/home/redmine
# Fri, 17 Apr 2020 10:13:33 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 17 Apr 2020 10:13:34 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 17 Apr 2020 10:13:36 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 17 Apr 2020 10:13:42 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 17 Apr 2020 10:17:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 17 Apr 2020 10:17:07 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 17 Apr 2020 10:17:08 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 17 Apr 2020 10:17:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Apr 2020 10:17:11 GMT
EXPOSE 3000
# Fri, 17 Apr 2020 10:17:13 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90689245dcf084a6cbe7d0e2eb03ac23596602ca04f8ebeea013edd9163eb36`  
		Last Modified: Thu, 16 Apr 2020 18:12:19 GMT  
		Size: 9.8 MB (9847368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8765a4f122f3e5882a72239acc339fd9c44eb6700bed6b4b33bf6e6a9182cc66`  
		Last Modified: Thu, 16 Apr 2020 18:12:15 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a76519570303f782a281ca6e93a1d7576ddeec65f176c4571a8f749c971f3dc`  
		Last Modified: Thu, 16 Apr 2020 18:12:48 GMT  
		Size: 20.6 MB (20622413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8304cb30692800b6c30c0ee835408b3e4dd68255043f36572f6bbd7d270f0d3d`  
		Last Modified: Thu, 16 Apr 2020 18:12:43 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9eebcef7c068b4f995042e923434c5b1d0e038c8241afa93e6a3d6b0f69d3f7`  
		Last Modified: Fri, 17 Apr 2020 10:25:12 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b373a62954404d71fc105912a2b332a2ef38f999bcffd24890e883f78d6309c`  
		Last Modified: Fri, 17 Apr 2020 10:25:42 GMT  
		Size: 84.7 MB (84732603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c526cc5287f5ad53e90383ed2c7d5e26acbbb86a65fc2ec4253309bec4d8bd81`  
		Last Modified: Fri, 17 Apr 2020 10:25:12 GMT  
		Size: 1.3 MB (1318431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9055d370048a17d0aa3d95b1353e5da15f71e01bb5cc6b480a92c58770e587d5`  
		Last Modified: Fri, 17 Apr 2020 10:25:11 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0432478fdd1aab34050e0163ff016d65a060d051141034ab408508fb75f97d12`  
		Last Modified: Fri, 17 Apr 2020 10:25:11 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:491fedf353351d7618f4e96f95fad2175d2ba5c804798528bdbbfb1aa26d86e6`  
		Last Modified: Fri, 17 Apr 2020 10:25:12 GMT  
		Size: 2.7 MB (2739763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184dd70e5b78c1a20d84f98551f5303302dbb5b8a6a16e49cf08c73c3ffffaf9`  
		Last Modified: Fri, 17 Apr 2020 10:25:24 GMT  
		Size: 56.1 MB (56060587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70309732307501d4360ad8120a4e2a22159dfa9e711155baeaa5bb18c2825a4d`  
		Last Modified: Fri, 17 Apr 2020 10:25:10 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; arm64 variant v8

```console
$ docker pull redmine@sha256:b64fb081b565f2fe63033453cb5577d8d85af63360dd0dcc3b06eac14619fe68
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **211.3 MB (211283317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d94b375f36acfdd79428e9348bb454ba8b9e05989b7d62b0b0f5677e33e88a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:52 GMT
ADD file:1aab17002a9095c31dd6928277a045cb26846ac58c3d2d63316332c99a5f90bd in / 
# Thu, 16 Apr 2020 02:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 19:30:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 19:30:59 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 16 Apr 2020 19:38:08 GMT
ENV RUBY_MAJOR=2.6
# Thu, 16 Apr 2020 19:38:10 GMT
ENV RUBY_VERSION=2.6.6
# Thu, 16 Apr 2020 19:38:12 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Thu, 16 Apr 2020 19:41:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 16 Apr 2020 19:41:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 16 Apr 2020 19:41:38 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 16 Apr 2020 19:41:39 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 19:41:41 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 16 Apr 2020 19:41:42 GMT
CMD ["irb"]
# Fri, 17 Apr 2020 11:07:40 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 17 Apr 2020 11:08:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 11:09:17 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 17 Apr 2020 11:09:18 GMT
ENV RAILS_ENV=production
# Fri, 17 Apr 2020 11:09:19 GMT
WORKDIR /usr/src/redmine
# Fri, 17 Apr 2020 11:09:20 GMT
ENV HOME=/home/redmine
# Fri, 17 Apr 2020 11:09:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 17 Apr 2020 11:09:25 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 17 Apr 2020 11:09:26 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 17 Apr 2020 11:09:51 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 17 Apr 2020 11:13:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 17 Apr 2020 11:13:45 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 17 Apr 2020 11:13:45 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 17 Apr 2020 11:13:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Apr 2020 11:13:47 GMT
EXPOSE 3000
# Fri, 17 Apr 2020 11:13:48 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:3d48095d71a365b5910cea98e5566c152a3f9aa11657560568259bf93ff2f4cb`  
		Last Modified: Thu, 16 Apr 2020 02:48:58 GMT  
		Size: 25.9 MB (25857715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdd33f108215db58bd0e6f140401d93c4b1b536c7ad089a4d0d0edcd2054704`  
		Last Modified: Thu, 16 Apr 2020 20:03:55 GMT  
		Size: 11.2 MB (11244664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b731403e546d6ee4346d854724aeec93f5a7d40b2896f756531171bb5634bf`  
		Last Modified: Thu, 16 Apr 2020 20:03:51 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a07cc279b68bee894882cdb8295d12fba14a21f2759618f21e2e41ec57136dc`  
		Last Modified: Thu, 16 Apr 2020 20:04:26 GMT  
		Size: 21.3 MB (21287940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a03216b543b88961e7600433fc393801a20caacb3e2fa5e42c65bd7e841559`  
		Last Modified: Thu, 16 Apr 2020 20:04:22 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fe0a46bf2a803c3fd66a95c043cf488c5a6d0d59c0ddf82d833ac5ed2b15b4`  
		Last Modified: Fri, 17 Apr 2020 11:20:32 GMT  
		Size: 1.8 KB (1751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac03e1810aaba20fb7f3b6497839bfb48b1f3b2f53d900460f0d97742bf7a7f9`  
		Last Modified: Fri, 17 Apr 2020 11:20:59 GMT  
		Size: 91.7 MB (91684633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c01d159c112132619b23ca43b35b0e26e1ab257f14cb5c308d74f6bcb24a3ff`  
		Last Modified: Fri, 17 Apr 2020 11:20:32 GMT  
		Size: 1.3 MB (1302884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76155cb07831ec6dbbefd622ed0fcf74b3e1a397a25b197037ed15a01f821856`  
		Last Modified: Fri, 17 Apr 2020 11:20:30 GMT  
		Size: 172.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7856e07a6366ee58320c2228be466d029a23324f9a65c9bc0d4e6eda7be31bf`  
		Last Modified: Fri, 17 Apr 2020 11:20:31 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a48ca3a1908ed57c15098eb433718f1ca53963e474e61b9120622ab968e9085`  
		Last Modified: Fri, 17 Apr 2020 11:20:31 GMT  
		Size: 2.7 MB (2739763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f9e538fec9c0ee44722a473f2fc93efb9807c9729ba5d9af4b841f3c3ceb766`  
		Last Modified: Fri, 17 Apr 2020 11:20:42 GMT  
		Size: 57.2 MB (57161207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82797391caa406abe2da293889c23977a4ca90488f8f639b8ac1d62de44799d`  
		Last Modified: Fri, 17 Apr 2020 11:20:31 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; 386

```console
$ docker pull redmine@sha256:9d88c3ec5c8548e0de7acd7ebdfd7a44dca5de568f22d260cf81375c2a19b0d5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.0 MB (220989844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b0a96f1b1d2b1b62d4e78748a05548d3f48ce6105b3d49be75829c63af58b38`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:55 GMT
ADD file:ab0bbfba6c4b56420ffffc6cdddcc4592fff018f0cd07578c7dc0a5faa49df2f in / 
# Thu, 16 Apr 2020 01:39:56 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 18:58:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 18:58:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 16 Apr 2020 19:07:30 GMT
ENV RUBY_MAJOR=2.6
# Thu, 16 Apr 2020 19:07:30 GMT
ENV RUBY_VERSION=2.6.6
# Thu, 16 Apr 2020 19:07:30 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Thu, 16 Apr 2020 19:11:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 16 Apr 2020 19:11:53 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 16 Apr 2020 19:11:53 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 16 Apr 2020 19:11:54 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 19:11:54 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 16 Apr 2020 19:11:55 GMT
CMD ["irb"]
# Fri, 17 Apr 2020 02:42:27 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 17 Apr 2020 02:43:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 17 Apr 2020 02:43:36 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 17 Apr 2020 02:43:36 GMT
ENV RAILS_ENV=production
# Fri, 17 Apr 2020 02:43:37 GMT
WORKDIR /usr/src/redmine
# Fri, 17 Apr 2020 02:43:37 GMT
ENV HOME=/home/redmine
# Fri, 17 Apr 2020 02:43:39 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 17 Apr 2020 02:43:39 GMT
ENV REDMINE_VERSION=4.1.1
# Fri, 17 Apr 2020 02:43:39 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Fri, 17 Apr 2020 02:43:44 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 17 Apr 2020 02:47:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 17 Apr 2020 02:47:17 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 17 Apr 2020 02:47:18 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 17 Apr 2020 02:47:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 17 Apr 2020 02:47:18 GMT
EXPOSE 3000
# Fri, 17 Apr 2020 02:47:19 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:75bc60a98e6523be3fadd9128c1a630cb5cbd2d2d813ee5e99dc146a3de22254`  
		Last Modified: Thu, 16 Apr 2020 01:46:20 GMT  
		Size: 27.8 MB (27753976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:783bdcb00a31ddb1d118dfa8d886b0d2e30c62594fa8361a86e654efd45406e6`  
		Last Modified: Thu, 16 Apr 2020 19:37:48 GMT  
		Size: 17.2 MB (17206366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72053eeb282be50e3047d9cd2ae172aaad371c097382a1077137de3a97a9d3cc`  
		Last Modified: Thu, 16 Apr 2020 19:37:35 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15481f295fd66433885c614bfcf02bfabad0cd62b1c30ec711d6c40aa84c8f81`  
		Last Modified: Thu, 16 Apr 2020 19:38:26 GMT  
		Size: 20.9 MB (20884671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6649bd52b6b678aea81fed1c03dc5d4cee9289a9d1ef4d6cf8ca5daafcb94a`  
		Last Modified: Thu, 16 Apr 2020 19:38:20 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1eed3f86d2c5128fd7016d6d39c2e1495a8f15c582390392680e1e8dce16cd8`  
		Last Modified: Fri, 17 Apr 2020 02:53:47 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d701b7836426872f624dcf7e83de95e4b372025759b3071aecdc7f9065a947`  
		Last Modified: Fri, 17 Apr 2020 02:54:49 GMT  
		Size: 94.7 MB (94730251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ff78856071ab18f5fb53cff019673c5f78a6c84cf37b512f0579d87bcdd50c`  
		Last Modified: Fri, 17 Apr 2020 02:53:46 GMT  
		Size: 1.3 MB (1337913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6e4a6a7eaa82f201646fab9b7bb251d2bd27f0015e79b723959ce3983080e6`  
		Last Modified: Fri, 17 Apr 2020 02:53:44 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf5c3e87a18f79128cde7bb9897641ca122383d9c1f612e8556d5fb70e8285c`  
		Last Modified: Fri, 17 Apr 2020 02:53:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796afd4cba7b50dbf894981643dcb26d1563574712bf546096f60202a8784b8c`  
		Last Modified: Fri, 17 Apr 2020 02:53:49 GMT  
		Size: 2.7 MB (2739483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a79542b68f69bd4acaae54f1bf4d38cf662b2f37b3a3cf9769a24af154171d`  
		Last Modified: Fri, 17 Apr 2020 02:54:39 GMT  
		Size: 56.3 MB (56332787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f688f8c74348142876e3f35ef296578b2a9c8a4fc27c8f56449d44965aa9bdef`  
		Last Modified: Fri, 17 Apr 2020 02:53:44 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; ppc64le

```console
$ docker pull redmine@sha256:d6b09243d49c61f1a491ae402fa53f5d059a9395af89df0da990b7b0e2126e67
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.1 MB (228077305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:566697f6eee4b67ce2aa05995ee56f55a0470bf772b3c13b0b68a237572fb910`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Tue, 31 Mar 2020 01:32:42 GMT
ADD file:36c02e92574faba45b64cfed78a0a0359d65ad175b17128bf554a2a5c0086ff5 in / 
# Tue, 31 Mar 2020 01:32:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 11:00:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 11:00:50 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 31 Mar 2020 11:11:22 GMT
ENV RUBY_MAJOR=2.6
# Wed, 01 Apr 2020 01:52:51 GMT
ENV RUBY_VERSION=2.6.6
# Wed, 01 Apr 2020 01:52:54 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Wed, 01 Apr 2020 01:58:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 01 Apr 2020 01:58:38 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 01 Apr 2020 01:58:42 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 01 Apr 2020 01:58:44 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Apr 2020 01:58:52 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 01 Apr 2020 01:58:55 GMT
CMD ["irb"]
# Wed, 01 Apr 2020 03:29:44 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 01 Apr 2020 03:32:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 03:35:29 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Apr 2020 03:35:32 GMT
ENV RAILS_ENV=production
# Wed, 01 Apr 2020 03:35:36 GMT
WORKDIR /usr/src/redmine
# Wed, 01 Apr 2020 03:35:39 GMT
ENV HOME=/home/redmine
# Wed, 01 Apr 2020 03:35:46 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Mon, 06 Apr 2020 20:28:08 GMT
ENV REDMINE_VERSION=4.1.1
# Mon, 06 Apr 2020 20:28:12 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Mon, 06 Apr 2020 20:28:25 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Mon, 06 Apr 2020 20:33:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 06 Apr 2020 20:33:53 GMT
VOLUME [/usr/src/redmine/files]
# Mon, 06 Apr 2020 20:33:54 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Mon, 06 Apr 2020 20:33:58 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 06 Apr 2020 20:34:02 GMT
EXPOSE 3000
# Mon, 06 Apr 2020 20:34:04 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:9df6bbae5eeb29e9aac2f39cff517c694cce60f01ee477abcdedcd8e8c01c38f`  
		Last Modified: Tue, 31 Mar 2020 01:45:59 GMT  
		Size: 30.5 MB (30518493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1942949d576a4423bb3e9c4d541fdeed116cc0fec657a1421fbac42d0e1aede2`  
		Last Modified: Tue, 31 Mar 2020 12:27:37 GMT  
		Size: 12.7 MB (12688913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184f0edee14fc0769e74017f104f335725ccba17a8b0283ca0d7ff6642a6a525`  
		Last Modified: Tue, 31 Mar 2020 12:27:30 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36bc0c58123b8a5a9085d65aa0ab19094f484cc4bbe7e4532b65e5ea929722f9`  
		Last Modified: Wed, 01 Apr 2020 03:24:44 GMT  
		Size: 22.0 MB (21970057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3be5a81457f4511c88f2bf9052b842ddffe3868be034bed247c4165d93b5bd`  
		Last Modified: Wed, 01 Apr 2020 03:24:41 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe660f40a390266ad449524e335133c86fbb528c05920d6a41282a1f984f4e4`  
		Last Modified: Wed, 01 Apr 2020 04:06:33 GMT  
		Size: 1.8 KB (1756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8fb11c9b4e8d804d940f9bd912efa15a577fa7573c368dd6f7e401e0ef1db`  
		Last Modified: Wed, 01 Apr 2020 04:06:53 GMT  
		Size: 100.3 MB (100281153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e875301b75021ab74fbdd1d9d5f4bf5f2d8e1bdab6973493dd68a64a0f05c35`  
		Last Modified: Wed, 01 Apr 2020 04:06:33 GMT  
		Size: 1.2 MB (1232593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a62fbba2ea1b8dc1e7230e2fc640449ee4e7bd7fa27ce8a62e3b2b82f4aa1ca`  
		Last Modified: Wed, 01 Apr 2020 04:06:29 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59465c970f3aa85dc9e7599328f53f8ad329f8971178655de65fd9d6a3996806`  
		Last Modified: Wed, 01 Apr 2020 04:06:29 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8e090e55c5fcdbf0923fbf03772adf0dd71208d76c3f0a768ef7a08f0345f3`  
		Last Modified: Mon, 06 Apr 2020 20:47:16 GMT  
		Size: 2.7 MB (2739761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75fd7ce2cc3184bd3f44fb9b9c537674910da2191899baec0a1be9c52e1e4a6`  
		Last Modified: Mon, 06 Apr 2020 20:47:25 GMT  
		Size: 58.6 MB (58641823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83e852f4eb78d934deef23d90cebaa87c6b373a752e43a09f207812838b7808`  
		Last Modified: Mon, 06 Apr 2020 20:47:14 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `redmine:latest` - linux; s390x

```console
$ docker pull redmine@sha256:960161b5b7e661664f0172ef53b0d70630499056cd2a07cae50bdf8cbb0642a6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210678057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb7d09e62618a0930df5eef71bf1182b1999f6668d8afa8c07ee82ccfa44c96`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["rails","server","-b","0.0.0.0"]`

```dockerfile
# Thu, 16 Apr 2020 00:42:19 GMT
ADD file:f328b5d6dce2eaf00360542c1e3280958b818268b9150b12ffd1fddf030daf2f in / 
# Thu, 16 Apr 2020 00:42:20 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 08:47:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 08:47:55 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 16 Apr 2020 08:58:22 GMT
ENV RUBY_MAJOR=2.6
# Thu, 16 Apr 2020 08:58:22 GMT
ENV RUBY_VERSION=2.6.6
# Thu, 16 Apr 2020 08:58:23 GMT
ENV RUBY_DOWNLOAD_SHA256=5db187882b7ac34016cd48d7032e197f07e4968f406b0690e20193b9b424841f
# Thu, 16 Apr 2020 08:59:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 16 Apr 2020 08:59:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 16 Apr 2020 08:59:58 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 16 Apr 2020 08:59:58 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 08:59:59 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 16 Apr 2020 08:59:59 GMT
CMD ["irb"]
# Thu, 16 Apr 2020 10:04:09 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 16 Apr 2020 10:04:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 20:11:54 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.12'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Apr 2020 20:11:55 GMT
ENV RAILS_ENV=production
# Thu, 16 Apr 2020 20:11:55 GMT
WORKDIR /usr/src/redmine
# Thu, 16 Apr 2020 20:11:55 GMT
ENV HOME=/home/redmine
# Thu, 16 Apr 2020 20:11:56 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 16 Apr 2020 20:11:56 GMT
ENV REDMINE_VERSION=4.1.1
# Thu, 16 Apr 2020 20:11:56 GMT
ENV REDMINE_DOWNLOAD_MD5=a15a25dec7b866e213bbd4b041f05f17
# Thu, 16 Apr 2020 20:12:03 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 16 Apr 2020 20:13:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Apr 2020 20:13:43 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 16 Apr 2020 20:13:43 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Thu, 16 Apr 2020 20:13:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 20:13:44 GMT
EXPOSE 3000
# Thu, 16 Apr 2020 20:13:44 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
```

-	Layers:
	-	`sha256:043f95f5412a986fb082b0193860bb9c0388c2fbcb5e8bf5bcbbeefb0e45c9c5`  
		Last Modified: Thu, 16 Apr 2020 00:46:19 GMT  
		Size: 25.7 MB (25712234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b75fe3310f9c32d5941f1caa91999b62d997dc4bf0e605396e9afccd42178c4`  
		Last Modified: Thu, 16 Apr 2020 09:11:15 GMT  
		Size: 10.8 MB (10796107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b70f5aaa809370d4906cf147578f4131e840a326a37b79fb926ed50ea4bad7f`  
		Last Modified: Thu, 16 Apr 2020 09:11:13 GMT  
		Size: 199.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d735d9ef922265545cb6cbd6c59664f169d700b71bd1b88c3185f0cdd582e0`  
		Last Modified: Thu, 16 Apr 2020 09:11:42 GMT  
		Size: 21.6 MB (21596699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06be3c628df077c7f2c9a751eabe7edb4552488b561f3a77f960a9e11e50e689`  
		Last Modified: Thu, 16 Apr 2020 09:11:46 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d324f888821702653b8f98f2d3741442258564e43d1d4245fae896534df7b2cb`  
		Last Modified: Thu, 16 Apr 2020 10:09:59 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7927f3237437b49e5ab3ce1ed71ae48e2ff18a06c86194b3d029ef6813a7e2d9`  
		Last Modified: Thu, 16 Apr 2020 10:10:15 GMT  
		Size: 90.8 MB (90834924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d5870bfb18394cc5da2e657ac58da327177a20acbf1f2f76c96509aa9d41ab7`  
		Last Modified: Thu, 16 Apr 2020 20:16:19 GMT  
		Size: 1.4 MB (1355097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cebe76c90a4348fd0a05c54b38728757921993c7d223929c424ea914a8dbf21`  
		Last Modified: Thu, 16 Apr 2020 20:16:17 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17213c8442e74ab10710dc4c6c049df1bd4af6245aaaa99f7d472ae535626c65`  
		Last Modified: Thu, 16 Apr 2020 20:16:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894ad56924b26c3b0dd81387f4ba7899cc3c7232f353f6f8dc2121ca3d8a43b6`  
		Last Modified: Thu, 16 Apr 2020 20:16:18 GMT  
		Size: 2.7 MB (2739763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6253a6e7a36089fd56394ea4b26dab4faf30218cea81ace949c6eb35068a97ba`  
		Last Modified: Thu, 16 Apr 2020 20:16:29 GMT  
		Size: 57.6 MB (57638730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0125fbba96b9bf12701ce52b052a17f2d49c550f164f63f0022a3911c4a24392`  
		Last Modified: Thu, 16 Apr 2020 20:16:33 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
