## `redmine:passenger`

```console
$ docker pull redmine@sha256:20978a415feb616600255f4c53e3509d43bda37e3d4eed95565700c729a886ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:passenger` - linux; amd64

```console
$ docker pull redmine@sha256:ca7a0f5ebc117c2ded52061c9e9b586460299e6c913a2d8924deb67cfcb0f6ae
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.0 MB (230993959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19b910b4099c7da0258d7cb4dbeb87280b8aedad9fa4683be5ff506a5ec406ea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 12:48:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 12:48:57 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Sat, 23 Nov 2019 12:58:18 GMT
ENV RUBY_MAJOR=2.6
# Sat, 23 Nov 2019 12:58:18 GMT
ENV RUBY_VERSION=2.6.5
# Sat, 23 Nov 2019 12:58:18 GMT
ENV RUBY_DOWNLOAD_SHA256=d5d6da717fd48524596f9b78ac5a2eeb9691753da5c06923a6c31190abe01a62
# Sat, 23 Nov 2019 13:03:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 23 Nov 2019 13:03:22 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 23 Nov 2019 13:03:22 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 23 Nov 2019 13:03:23 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 13:03:24 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 23 Nov 2019 13:03:24 GMT
CMD ["irb"]
# Sun, 24 Nov 2019 00:22:55 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 24 Nov 2019 00:23:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 24 Nov 2019 00:23:40 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 24 Nov 2019 00:23:40 GMT
ENV RAILS_ENV=production
# Sun, 24 Nov 2019 00:23:41 GMT
WORKDIR /usr/src/redmine
# Sun, 24 Nov 2019 00:23:41 GMT
ENV HOME=/home/redmine
# Sun, 24 Nov 2019 00:23:41 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 20 Dec 2019 20:42:04 GMT
ENV REDMINE_VERSION=4.0.6
# Fri, 20 Dec 2019 20:42:04 GMT
ENV REDMINE_DOWNLOAD_MD5=897bfcaa4a49539b10d0529ce103f919
# Fri, 20 Dec 2019 20:42:08 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 20 Dec 2019 20:44:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmagickcore-dev 		libmagickwand-dev 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Dec 2019 20:44:55 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 20 Dec 2019 20:44:55 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 20 Dec 2019 20:44:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 20 Dec 2019 20:44:56 GMT
EXPOSE 3000
# Fri, 20 Dec 2019 20:44:56 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 20 Dec 2019 20:45:04 GMT
ENV PASSENGER_VERSION=6.0.4
# Fri, 20 Dec 2019 20:45:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Dec 2019 20:45:25 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 20 Dec 2019 20:45:25 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 20 Dec 2019 20:45:25 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb775c9947bd15329b240cace20af8c8a27f2a0307b3a70afa4fc4d1fc48bca8`  
		Last Modified: Sat, 23 Nov 2019 13:53:45 GMT  
		Size: 12.5 MB (12539717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4023dfa48cbbce1634b98375fc7fd67949fb44a3364f32d3b5c26f67ac6f62`  
		Last Modified: Sat, 23 Nov 2019 13:53:41 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aa32dfe0a3dadee59ef8220a23c940764e0c1450b57c9b41d8bf0596bb3283d`  
		Last Modified: Sat, 23 Nov 2019 13:54:08 GMT  
		Size: 21.4 MB (21445730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f36e70241367a9fc6c3b6bbae1d582c4f43099aa80c2ca3ab6743fcf0c3cc4`  
		Last Modified: Sat, 23 Nov 2019 13:54:05 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e316cc0e245707fcafa3b1c6d506668d13ac7dfbf77040df5ab41aab0ada50`  
		Last Modified: Sun, 24 Nov 2019 00:31:04 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f6d36d788e308adcea936c951724825e77ab0466824a776ade7e7b408d447f`  
		Last Modified: Sun, 24 Nov 2019 00:31:19 GMT  
		Size: 80.2 MB (80165276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff1349f123720a9525d0a2e874f55f15582dda75542fa425155c9392ef24bcf3`  
		Last Modified: Sun, 24 Nov 2019 00:31:04 GMT  
		Size: 1.3 MB (1296492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4b74160ec7bd63cffa3503f12599ff87c076b29a469eb209c855a0186d7444`  
		Last Modified: Sun, 24 Nov 2019 00:31:03 GMT  
		Size: 139.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b166162149d6fe6f7f848ae136911e8b3ac804c02af0fa2739f7c1b87dcad0d`  
		Last Modified: Sun, 24 Nov 2019 00:31:03 GMT  
		Size: 128.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc6f82a10a70a3de00d2cad8fc4b5bf2a9fd7f1fb9ca2c0ed351416c3958c48`  
		Last Modified: Fri, 20 Dec 2019 20:53:02 GMT  
		Size: 2.5 MB (2534052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b62507d95f7205850449651c428e59f16a89d5601ccee64b4e75c42a57bd5ab`  
		Last Modified: Fri, 20 Dec 2019 20:53:11 GMT  
		Size: 61.1 MB (61057991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884a461b2f9f807622508f0cf099e20a77ea7e1611dfbc26b6d0934754edae91`  
		Last Modified: Fri, 20 Dec 2019 20:53:01 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2242aa8c4191caa2dd9fa025dfe6191583e6e9444e82555df7c1482b91e8492`  
		Last Modified: Fri, 20 Dec 2019 20:53:19 GMT  
		Size: 19.9 MB (19939798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4d6ccb7d5d0d7987882c56c8064eb69a1365219096e8b4af29d48efa078cff`  
		Last Modified: Fri, 20 Dec 2019 20:53:17 GMT  
		Size: 4.9 MB (4917839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
