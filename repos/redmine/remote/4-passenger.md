## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:9b780f98151823e0e84e1e41974c548143cae7090cd367eb711d44d3bc8a966b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:a320947c8461cd8bafad0bcfda90b4f5ac840389345003324df81de7b46ad296
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.5 MB (221526742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3049f679e04c98a7643e800733c59f85c960a686a186192d9b12a222bed1592`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:40 GMT
ADD file:4903a19c327468b0e08e4f463cfc162c66b85b4618b5803d71365862f6302e0b in / 
# Wed, 23 Jun 2021 00:20:40 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 17:07:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:07:37 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 23 Jun 2021 17:07:37 GMT
ENV LANG=C.UTF-8
# Wed, 23 Jun 2021 17:14:10 GMT
ENV RUBY_MAJOR=2.7
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_VERSION=2.7.4
# Wed, 07 Jul 2021 19:43:10 GMT
ENV RUBY_DOWNLOAD_SHA256=2a80824e0ad6100826b69b9890bf55cfc4cf2b61a1e1330fccbcb30c46cef8d7
# Thu, 08 Jul 2021 22:11:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 		libgdbm-compat-dev 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 08 Jul 2021 22:11:02 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 08 Jul 2021 22:11:03 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 08 Jul 2021 22:11:05 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 08 Jul 2021 22:11:05 GMT
CMD ["irb"]
# Wed, 14 Jul 2021 20:20:37 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Wed, 14 Jul 2021 20:21:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 20:21:06 GMT
ENV RAILS_ENV=production
# Wed, 14 Jul 2021 20:21:06 GMT
WORKDIR /usr/src/redmine
# Wed, 14 Jul 2021 20:21:06 GMT
ENV HOME=/home/redmine
# Wed, 14 Jul 2021 20:21:07 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_VERSION=4.2.1
# Wed, 14 Jul 2021 20:21:08 GMT
ENV REDMINE_DOWNLOAD_SHA256=ad4109c3425f1cfe4c8961f6ae6494c76e20d81ed946caa1e297d9eda13b41b4
# Wed, 14 Jul 2021 20:21:12 GMT
RUN set -eux; 	wget -O redmine.tar.gz "https://www.redmine.org/releases/redmine-${REDMINE_VERSION}.tar.gz"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Wed, 14 Jul 2021 20:21:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		freetds-dev 		gcc 		libmariadbclient-dev 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:21:54 GMT
VOLUME [/usr/src/redmine/files]
# Wed, 14 Jul 2021 20:21:54 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Wed, 14 Jul 2021 20:21:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 14 Jul 2021 20:21:55 GMT
EXPOSE 3000
# Wed, 14 Jul 2021 20:21:55 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Wed, 14 Jul 2021 20:22:01 GMT
ENV PASSENGER_VERSION=6.0.10
# Wed, 14 Jul 2021 20:22:18 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 14 Jul 2021 20:22:20 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Wed, 14 Jul 2021 20:22:20 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Wed, 14 Jul 2021 20:22:20 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b4d181a07f8025e00e0cb28f1cc14613da2ce26450b80c54aea537fa93cf3bda`  
		Last Modified: Wed, 23 Jun 2021 00:25:39 GMT  
		Size: 27.1 MB (27145851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8edb0654f16a0b0dfa9167e58fdc2d00d20e61f18f10d3e848418baf5bef4ab`  
		Last Modified: Wed, 23 Jun 2021 17:42:38 GMT  
		Size: 12.6 MB (12562685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ba211d3249c13e0f844045a38f32ef8cce47229548262f3503816661e9af`  
		Last Modified: Wed, 23 Jun 2021 17:42:36 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de7400f1f9b6e5d55a83e8b37dd13cf72bdbe0d05934f5c98c4ba06bf4cbf118`  
		Last Modified: Thu, 08 Jul 2021 22:39:29 GMT  
		Size: 14.5 MB (14509548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb40617deac0692ea97ddae53d285e362d757e8808ea3d0242f0f467fbdc83b`  
		Last Modified: Thu, 08 Jul 2021 22:39:27 GMT  
		Size: 175.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5e207773ba291762558574c95425f761b6392afd6e47e33a2ef03ba607a20b`  
		Last Modified: Wed, 14 Jul 2021 20:34:47 GMT  
		Size: 1.7 KB (1744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a0707c83bf4fc7c6a74d7536a44f0769ac86b1f962c1af56accd5e6cd3ba2`  
		Last Modified: Wed, 14 Jul 2021 20:35:01 GMT  
		Size: 94.1 MB (94088231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac5644dd9c4b1b57fc0facc0fef989ab8a63d78d5674817336139f4dbaccb6f`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cba4fc03f4f8b3bb011488d95ba8548ebf98c7c911213769e19fff09ca870`  
		Last Modified: Wed, 14 Jul 2021 20:34:44 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353cee6d422cb4bc36abb65fd6c55a508990ed2f2bf4abfc1ce1535b475d6df3`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 3.1 MB (3058676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b939da848c07b0f5edcd234d2437605bf205006fdb97858805234a356aee26c`  
		Last Modified: Wed, 14 Jul 2021 20:34:50 GMT  
		Size: 44.1 MB (44106524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e500e65c849556d24a3d032e6d73d10c2c207727e62435e93883100e925cce45`  
		Last Modified: Wed, 14 Jul 2021 20:34:45 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca41f4f9e9b7629be3e6e9666279b940b489648484da4e41725e7b22c1c94b1b`  
		Last Modified: Wed, 14 Jul 2021 20:35:22 GMT  
		Size: 21.1 MB (21131700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9436698f0e4aec6d6e7c991fd623ae0d4eab48e62193c564b2fa25de8f4a52e`  
		Last Modified: Wed, 14 Jul 2021 20:35:20 GMT  
		Size: 4.9 MB (4919284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
