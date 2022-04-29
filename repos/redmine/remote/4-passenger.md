## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:61a28caeb0352277cbbf12cb27fb1242bccc9bb7506cbbb1b1d942239edc94c1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:88fea582975f27ef80f8acbdbd868030c6b47ea1d86f2f93addfddf84501e0d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.2 MB (232229294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:303e6de1011d725be58932b5d8f8c318078db1ae2f0de1c302417ac2e5c6a6b1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:27 GMT
ADD file:8b1e79f91081eb527b455431af58e823d8b84d9d0c8e5c47cb7bda7507954ae4 in / 
# Wed, 20 Apr 2022 04:43:27 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 13:48:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 13:48:43 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Wed, 20 Apr 2022 13:48:43 GMT
ENV LANG=C.UTF-8
# Wed, 20 Apr 2022 14:15:37 GMT
ENV RUBY_MAJOR=2.7
# Wed, 20 Apr 2022 14:15:37 GMT
ENV RUBY_VERSION=2.7.6
# Wed, 20 Apr 2022 14:15:37 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Wed, 20 Apr 2022 14:17:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Wed, 20 Apr 2022 14:17:25 GMT
ENV GEM_HOME=/usr/local/bundle
# Wed, 20 Apr 2022 14:17:25 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Wed, 20 Apr 2022 14:17:25 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 14:17:26 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Wed, 20 Apr 2022 14:17:26 GMT
CMD ["irb"]
# Thu, 21 Apr 2022 11:26:57 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Thu, 21 Apr 2022 11:27:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Thu, 21 Apr 2022 11:27:21 GMT
ENV RAILS_ENV=production
# Thu, 21 Apr 2022 11:27:21 GMT
WORKDIR /usr/src/redmine
# Thu, 21 Apr 2022 11:27:21 GMT
ENV HOME=/home/redmine
# Thu, 21 Apr 2022 11:27:21 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Thu, 21 Apr 2022 11:27:22 GMT
ENV REDMINE_VERSION=4.2.5
# Thu, 21 Apr 2022 11:27:22 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.5.tar.gz
# Thu, 21 Apr 2022 11:27:22 GMT
ENV REDMINE_DOWNLOAD_SHA256=d97084b0eaad7266056814a0c0aec2737f4d23b8f67ce90c01a79b2eb5605984
# Thu, 21 Apr 2022 11:27:25 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Thu, 21 Apr 2022 11:28:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 21 Apr 2022 11:28:08 GMT
VOLUME [/usr/src/redmine/files]
# Thu, 21 Apr 2022 11:28:08 GMT
COPY file:2c807aca5f34a9ab8acfef3c517816547300ed2b18590f703a1c783bdc707ba8 in / 
# Thu, 21 Apr 2022 11:28:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 21 Apr 2022 11:28:08 GMT
EXPOSE 3000
# Thu, 21 Apr 2022 11:28:08 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Fri, 29 Apr 2022 02:03:39 GMT
ENV PASSENGER_VERSION=6.0.13
# Fri, 29 Apr 2022 02:03:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 29 Apr 2022 02:03:59 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Fri, 29 Apr 2022 02:03:59 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Fri, 29 Apr 2022 02:03:59 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:1fe172e4850f03bb45d41a20174112bc119fbfec42a650edbbd8491aee32e3c3`  
		Last Modified: Wed, 20 Apr 2022 04:48:27 GMT  
		Size: 31.4 MB (31378979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100f29d0fcb2fab0f4d2a795b239feee6df8580994413fe4272b407851faaf3a`  
		Last Modified: Wed, 20 Apr 2022 14:30:59 GMT  
		Size: 10.0 MB (9991861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937a564b41a154323add828d5515056320d68a3f4b485a88b509260e1c231cad`  
		Last Modified: Wed, 20 Apr 2022 14:30:57 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cfeb9c3dee74234ac4b71e2f736ad3f6282a0b4d0195a164ee57443bd00865`  
		Last Modified: Wed, 20 Apr 2022 14:34:47 GMT  
		Size: 14.6 MB (14582235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0572da5ba7d563ae2a6590117a3b5fe2b9d3ef679881596352be9d3fee9cd3f7`  
		Last Modified: Wed, 20 Apr 2022 14:34:46 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aa0e9cbb09c6302807accd36987658e91d1bba5d360ae11c215fa882e1b413e`  
		Last Modified: Thu, 21 Apr 2022 11:32:01 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89575b2f1e5806c2176322805c8b7263d9e95bb3b342219d6838caed7720c0e1`  
		Last Modified: Thu, 21 Apr 2022 11:32:16 GMT  
		Size: 102.0 MB (101987498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e6d7325613a7c9bf219b158d47ce17d6140d0e22102a40b464926ec59b5c5f`  
		Last Modified: Thu, 21 Apr 2022 11:31:59 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51116eea8af952e1428b747835d5ea1b7d66acad56e2f0f493429cfea757c84a`  
		Last Modified: Thu, 21 Apr 2022 11:31:59 GMT  
		Size: 158.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b464156cd6d4234ee9633e1379437f8b578bf9cecf5663d869779e6304806a`  
		Last Modified: Thu, 21 Apr 2022 11:31:59 GMT  
		Size: 3.1 MB (3064905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d792d6585efa5be788ce5ea60bb6d29832b37a2e591278c6c5bf71febe1611f7`  
		Last Modified: Thu, 21 Apr 2022 11:32:04 GMT  
		Size: 43.9 MB (43900360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed95a2e288305ac9a5ee0b1304879d303c79a89218e426ba8374f1ff1087ffd`  
		Last Modified: Thu, 21 Apr 2022 11:31:59 GMT  
		Size: 1.8 KB (1795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c6f42f6e60d5e60eee8193f1b944272523f297fa47a1873f95eb47411ef55b`  
		Last Modified: Fri, 29 Apr 2022 02:04:47 GMT  
		Size: 21.8 MB (21782020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f46c4fdfa24951e209de27b627e6bfbdcc80a058f37c91ea2fe488f7e18646`  
		Last Modified: Fri, 29 Apr 2022 02:04:45 GMT  
		Size: 5.5 MB (5537193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
