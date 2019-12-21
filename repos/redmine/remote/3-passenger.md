## `redmine:3-passenger`

```console
$ docker pull redmine@sha256:68290992ba8f63baf5631e3b911a5a744285e0e68f56fba901b240dc6236766f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:3-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:59178343ac84f524edb87e9fc421ad0ae56eae531a059b18b6c25f5b30e861db
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.2 MB (232150471 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1aa29281c91cd4719280567333e94a8b3e9db32e3d534df31bbaca948284c8c`
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
# Sat, 23 Nov 2019 13:37:33 GMT
ENV RUBY_MAJOR=2.4
# Sat, 23 Nov 2019 13:37:33 GMT
ENV RUBY_VERSION=2.4.9
# Sat, 23 Nov 2019 13:37:33 GMT
ENV RUBY_DOWNLOAD_SHA256=0c4e000253ef7187feeb940a01a1c7594f28d63aa16f978e892a0e2864f58614
# Sat, 23 Nov 2019 13:37:33 GMT
ENV RUBYGEMS_VERSION=3.0.3
# Sat, 23 Nov 2019 13:42:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		bison 		dpkg-dev 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libgdbm-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		ruby 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	ruby -e 'exit(Gem::Version.create(ENV["RUBYGEMS_VERSION"]) > Gem::Version.create(Gem::VERSION))'; 	gem update --system "$RUBYGEMS_VERSION" && rm -r /root/.gem/; 	! dpkg -l | grep -i ruby; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Sat, 23 Nov 2019 13:42:58 GMT
ENV GEM_HOME=/usr/local/bundle
# Sat, 23 Nov 2019 13:42:59 GMT
ENV BUNDLE_PATH=/usr/local/bundle BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Sat, 23 Nov 2019 13:42:59 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/bundle/gems/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 13:43:00 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Sat, 23 Nov 2019 13:43:00 GMT
CMD ["irb"]
# Sun, 24 Nov 2019 00:27:11 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Sun, 24 Nov 2019 00:27:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				gsfonts 		imagemagick 	; 	rm -rf /var/lib/apt/lists/*
# Sun, 24 Nov 2019 00:27:44 GMT
RUN set -eux; 	savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		dirmngr 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		dpkgArch="$(dpkg --print-architecture | awk -F- '{ print $NF }')"; 		export GOSU_VERSION='1.11'; 	wget -O /usr/local/bin/gosu "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch"; 	wget -O /usr/local/bin/gosu.asc "https://github.com/tianon/gosu/releases/download/$GOSU_VERSION/gosu-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys B42F6819007F00F88E364FD4036A9C25BF357DD4; 	gpg --batch --verify /usr/local/bin/gosu.asc /usr/local/bin/gosu; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/gosu.asc; 	chmod +x /usr/local/bin/gosu; 	gosu nobody true; 		export TINI_VERSION='0.18.0'; 	wget -O /usr/local/bin/tini "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch"; 	wget -O /usr/local/bin/tini.asc "https://github.com/krallin/tini/releases/download/v$TINI_VERSION/tini-$dpkgArch.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 6380DC428747F6C393FEACA59A84159D7001A4E5; 	gpg --batch --verify /usr/local/bin/tini.asc /usr/local/bin/tini; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" /usr/local/bin/tini.asc; 	chmod +x /usr/local/bin/tini; 	tini -h; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sun, 24 Nov 2019 00:27:45 GMT
ENV RAILS_ENV=production
# Sun, 24 Nov 2019 00:27:45 GMT
WORKDIR /usr/src/redmine
# Sun, 24 Nov 2019 00:27:45 GMT
ENV HOME=/home/redmine
# Sun, 24 Nov 2019 00:27:46 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 20 Dec 2019 20:47:47 GMT
ENV REDMINE_VERSION=3.4.13
# Fri, 20 Dec 2019 20:47:47 GMT
ENV REDMINE_DOWNLOAD_MD5=5f17b35dfe73118067f63fb535332cfb
# Fri, 20 Dec 2019 20:47:50 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_MD5 *redmine.tar.gz" | md5sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 20 Dec 2019 20:50:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmagickcore-dev 		libmagickwand-dev 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$RAILS_ENV:" > ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 		gosu redmine bundle install --jobs "$(nproc)" --without development test; 		cp Gemfile.lock "Gemfile.lock.${adapter}"; 	done; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Dec 2019 20:50:22 GMT
VOLUME [/usr/src/redmine/files]
# Fri, 20 Dec 2019 20:50:22 GMT
COPY file:df6d0160357b381a47abf010e78172591272c9029cb0436b6b6dfcc71483244e in / 
# Fri, 20 Dec 2019 20:50:22 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 20 Dec 2019 20:50:23 GMT
EXPOSE 3000
# Fri, 20 Dec 2019 20:50:23 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 20 Dec 2019 20:50:31 GMT
ENV PASSENGER_VERSION=6.0.4
# Fri, 20 Dec 2019 20:50:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 20 Dec 2019 20:50:49 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 20 Dec 2019 20:50:49 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 20 Dec 2019 20:50:49 GMT
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
	-	`sha256:d5a90a529446fea058d1f089b08c3d236ab233a2c23ca2fec8dfbf8be256d995`  
		Last Modified: Sat, 23 Nov 2019 13:55:27 GMT  
		Size: 22.0 MB (22006056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527c18adae54a8bc322f695f372990908f0ef80cfca73f3694133c60fba62cb3`  
		Last Modified: Sat, 23 Nov 2019 13:55:24 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0c9d068e5981f7ed592d56ba631985001e364b437036f44f14a369fbcc2a45`  
		Last Modified: Sun, 24 Nov 2019 00:31:34 GMT  
		Size: 1.7 KB (1747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71918dd4b8d0f8ef569b64a14a07e37a97367e173fa1e9f7c8923ecaa9b9d142`  
		Last Modified: Sun, 24 Nov 2019 00:31:49 GMT  
		Size: 80.2 MB (80169926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaef5698d1e9824ec9a1d84c9ea402bafb4000ca36dd3f55f337567cdc88cfb3`  
		Last Modified: Sun, 24 Nov 2019 00:31:34 GMT  
		Size: 1.3 MB (1296412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e0528eacc52aa194413c769753f3d21919ee0ed5ddfd810295de0632d556d9`  
		Last Modified: Sun, 24 Nov 2019 00:31:33 GMT  
		Size: 138.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5cc78f2fef62e7b1c8f6fa50b08953d43e8d20e355cb966606a8485c2cfc2b`  
		Last Modified: Sun, 24 Nov 2019 00:31:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b74b814b21660531d444395fa69069f6971502ee0ba7ff2805e0fcba2f5987`  
		Last Modified: Fri, 20 Dec 2019 20:53:41 GMT  
		Size: 2.5 MB (2463466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8257c464c0cbdeab41a1e4b645bf19031cdbf02201a8577d6518d772333466`  
		Last Modified: Fri, 20 Dec 2019 20:53:49 GMT  
		Size: 61.7 MB (61722707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead6595e66d8654e6334393592bbeccc31aaf4b6ecd6afb45af1b53fc8cd34fe`  
		Last Modified: Fri, 20 Dec 2019 20:53:40 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173b46265165f79ff19bad93f2e5867e3b176f2973c805c846436fc92519d805`  
		Last Modified: Fri, 20 Dec 2019 20:53:57 GMT  
		Size: 19.9 MB (19937280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5849ad667912eb374ac70eaa22bb4d9d9c5cb2862c9d7d74b376a4ad47703c0`  
		Last Modified: Fri, 20 Dec 2019 20:53:56 GMT  
		Size: 4.9 MB (4917846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
