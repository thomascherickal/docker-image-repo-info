## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:99d7c1bcbc334638e6c938d3ddfae8914892cd76685db5a6e99e8712bd13a6d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:d93b0c68b001c8b9418a7faabcba477d3ff5cfbb7b1729f5500a7250117fcfba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.7 MB (233737788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28696fefa19d6c60b1985a8aa27df7bfe80198d0f505d20ed6c428a220344441`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Tue, 13 Sep 2022 00:56:29 GMT
ADD file:5bd53bff884e470b3c12425132975ab9c6f99002c62c43bca1ff5cde9d863b92 in / 
# Tue, 13 Sep 2022 00:56:29 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:07:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:07:20 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Tue, 13 Sep 2022 03:07:20 GMT
ENV LANG=C.UTF-8
# Tue, 13 Sep 2022 03:22:30 GMT
ENV RUBY_MAJOR=2.7
# Tue, 13 Sep 2022 03:22:30 GMT
ENV RUBY_VERSION=2.7.6
# Tue, 13 Sep 2022 03:22:30 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Tue, 13 Sep 2022 03:24:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Tue, 13 Sep 2022 03:24:16 GMT
ENV GEM_HOME=/usr/local/bundle
# Tue, 13 Sep 2022 03:24:16 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Tue, 13 Sep 2022 03:24:17 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Sep 2022 03:24:17 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Tue, 13 Sep 2022 03:24:17 GMT
CMD ["irb"]
# Tue, 13 Sep 2022 03:33:03 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Tue, 13 Sep 2022 03:33:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:33:28 GMT
ENV RAILS_ENV=production
# Tue, 13 Sep 2022 03:33:28 GMT
WORKDIR /usr/src/redmine
# Tue, 13 Sep 2022 03:33:28 GMT
ENV HOME=/home/redmine
# Tue, 13 Sep 2022 03:33:28 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Tue, 13 Sep 2022 03:33:28 GMT
ENV REDMINE_VERSION=4.2.7
# Tue, 13 Sep 2022 03:33:28 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Tue, 13 Sep 2022 03:33:29 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Tue, 13 Sep 2022 03:33:32 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Tue, 13 Sep 2022 03:34:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 03:34:16 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 13 Sep 2022 03:34:16 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 13 Sep 2022 03:34:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 13 Sep 2022 03:34:16 GMT
EXPOSE 3000
# Tue, 13 Sep 2022 03:34:16 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 13 Sep 2022 03:34:25 GMT
ENV PASSENGER_VERSION=6.0.14
# Tue, 13 Sep 2022 03:34:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 13 Sep 2022 03:34:43 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 13 Sep 2022 03:34:43 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 13 Sep 2022 03:34:43 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:31b3f1ad4ce1f369084d0f959813c51df0ca17d9877d5ee88c2db6ff88341430`  
		Last Modified: Tue, 13 Sep 2022 01:00:29 GMT  
		Size: 31.4 MB (31404121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecf19185ffb5ca2c21464d14f921ab167270fcd17601222a3a5ceaf893d96ca`  
		Last Modified: Tue, 13 Sep 2022 03:27:57 GMT  
		Size: 10.0 MB (10019057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7201eddc3a4c46c660962e898a98aa99c0e7574e66983029dfd9503904208e69`  
		Last Modified: Tue, 13 Sep 2022 03:27:55 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bfda2aa8c298d17baadeb3e5f9eb944f96424b3521b361474a31cd87db36fe3`  
		Last Modified: Tue, 13 Sep 2022 03:30:13 GMT  
		Size: 14.6 MB (14582325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c3d9b4dd8289368878436477f79ced8f721101511534979d35576f92265b82`  
		Last Modified: Tue, 13 Sep 2022 03:30:13 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf37b28c407a881ccdde912b4680ab465af243eee5cded1359a1b6241550922`  
		Last Modified: Tue, 13 Sep 2022 03:36:20 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd20a333d732f2a6603d61d4b7919d5d92b65f3a2f0a2b70b7e10ccd20dd6187`  
		Last Modified: Tue, 13 Sep 2022 03:36:35 GMT  
		Size: 102.0 MB (101992235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c90b1b609858319681f1e36774f3e48ad4fc7869c3870be6e534159b29a405c`  
		Last Modified: Tue, 13 Sep 2022 03:36:18 GMT  
		Size: 171.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178524822ef5bed85914c866cf3978a3ce675e4f3b306da65ae7ad4905078ebe`  
		Last Modified: Tue, 13 Sep 2022 03:36:18 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eabe12014e37bd0478e5d51900a85f1270ba8d40256826de2614f341d10fcab6`  
		Last Modified: Tue, 13 Sep 2022 03:36:19 GMT  
		Size: 3.1 MB (3066342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d20da6f1d63bd044b557be6eef3b89d4f55dad41f49b48246091783865ab040`  
		Last Modified: Tue, 13 Sep 2022 03:36:23 GMT  
		Size: 45.3 MB (45324465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bad295eb2b97e4b1406d470cb1048c062b06c518cab48e484789297f0c78e5`  
		Last Modified: Tue, 13 Sep 2022 03:36:18 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fe702009f53ae3c4dc4bc9ba8a8de00014c8852a91b0ef9bda0ab9200d9f1d`  
		Last Modified: Tue, 13 Sep 2022 03:37:07 GMT  
		Size: 21.8 MB (21800525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d52e6923b61680cd73211fab6138399e0b5321cebd227332ed232ac6a7e6a21`  
		Last Modified: Tue, 13 Sep 2022 03:37:05 GMT  
		Size: 5.5 MB (5544417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
