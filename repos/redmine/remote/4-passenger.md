## `redmine:4-passenger`

```console
$ docker pull redmine@sha256:f13a94c6e9298f4a0869f773f0a8891ac9a663553a38f8b859264e70de8b7a73
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `redmine:4-passenger` - linux; amd64

```console
$ docker pull redmine@sha256:bfaedbd4737008e106826d87e68882131c8ff8b02b88509a52fd81116c777310
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.7 MB (233662396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:755c651f86ccd870f3e4fb16b3808550c9e9fbcc5a405e5ead6a70304f1cab22`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["passenger","start"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:45:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		libffi-dev 		libgmp-dev 		libssl-dev 		libyaml-dev 		procps 		zlib1g-dev 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:45:45 GMT
RUN set -eux; 	mkdir -p /usr/local/etc; 	{ 		echo 'install: --no-document'; 		echo 'update: --no-document'; 	} >> /usr/local/etc/gemrc
# Thu, 23 Jun 2022 13:45:45 GMT
ENV LANG=C.UTF-8
# Thu, 23 Jun 2022 14:12:58 GMT
ENV RUBY_MAJOR=2.7
# Thu, 23 Jun 2022 14:12:58 GMT
ENV RUBY_VERSION=2.7.6
# Thu, 23 Jun 2022 14:12:58 GMT
ENV RUBY_DOWNLOAD_SHA256=54dcd3044726c4ab75a9d4604720501442b229a3aed6a55fe909567da8807f24
# Thu, 23 Jun 2022 14:14:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bison 		dpkg-dev 		libgdbm-dev 		ruby 		autoconf 		g++ 		gcc 		libbz2-dev 		libgdbm-compat-dev 		libglib2.0-dev 		libncurses-dev 		libreadline-dev 		libxml2-dev 		libxslt-dev 		make 		wget 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O ruby.tar.xz "https://cache.ruby-lang.org/pub/ruby/${RUBY_MAJOR%-rc}/ruby-$RUBY_VERSION.tar.xz"; 	echo "$RUBY_DOWNLOAD_SHA256 *ruby.tar.xz" | sha256sum --check --strict; 		mkdir -p /usr/src/ruby; 	tar -xJf ruby.tar.xz -C /usr/src/ruby --strip-components=1; 	rm ruby.tar.xz; 		cd /usr/src/ruby; 		{ 		echo '#define ENABLE_PATH_CHECK 0'; 		echo; 		cat file.c; 	} > file.c.new; 	mv file.c.new file.c; 		autoconf; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--disable-install-doc 		--enable-shared 	; 	make -j "$(nproc)"; 	make install; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -not \( -name '*tkinter*' \) -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -vE '^/usr/local/lib/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		cd /; 	rm -r /usr/src/ruby; 	if dpkg -l | grep -i ruby; then exit 1; fi; 	[ "$(command -v ruby)" = '/usr/local/bin/ruby' ]; 	ruby --version; 	gem --version; 	bundle --version
# Thu, 23 Jun 2022 14:14:46 GMT
ENV GEM_HOME=/usr/local/bundle
# Thu, 23 Jun 2022 14:14:46 GMT
ENV BUNDLE_SILENCE_ROOT_WARNING=1 BUNDLE_APP_CONFIG=/usr/local/bundle
# Thu, 23 Jun 2022 14:14:46 GMT
ENV PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 23 Jun 2022 14:14:47 GMT
RUN mkdir -p "$GEM_HOME" && chmod 777 "$GEM_HOME"
# Thu, 23 Jun 2022 14:14:47 GMT
CMD ["irb"]
# Fri, 24 Jun 2022 02:59:57 GMT
RUN groupadd -r -g 999 redmine && useradd -r -g redmine -u 999 redmine
# Fri, 24 Jun 2022 03:00:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		wget 				bzr 		git 		mercurial 		openssh-client 		subversion 				ghostscript 		gsfonts 		imagemagick 		gosu 		tini 	; 	sed -ri 's/(rights)="none" (pattern="PDF")/\1="read" \2/' /etc/ImageMagick-6/policy.xml; 	rm -rf /var/lib/apt/lists/*
# Fri, 24 Jun 2022 03:00:23 GMT
ENV RAILS_ENV=production
# Fri, 24 Jun 2022 03:00:23 GMT
WORKDIR /usr/src/redmine
# Fri, 24 Jun 2022 03:00:23 GMT
ENV HOME=/home/redmine
# Fri, 24 Jun 2022 03:00:23 GMT
RUN set -eux; 	[ ! -d "$HOME" ]; 	mkdir -p "$HOME"; 	chown redmine:redmine "$HOME"; 	chmod 1777 "$HOME"
# Fri, 24 Jun 2022 03:00:23 GMT
ENV REDMINE_VERSION=4.2.7
# Fri, 24 Jun 2022 03:00:24 GMT
ENV REDMINE_DOWNLOAD_URL=https://www.redmine.org/releases/redmine-4.2.7.tar.gz
# Fri, 24 Jun 2022 03:00:24 GMT
ENV REDMINE_DOWNLOAD_SHA256=ed4be03b5ab63c2641a87db8978739dd997c0f646bfa1010ac9e5210c343724e
# Fri, 24 Jun 2022 03:00:27 GMT
RUN set -eux; 	curl -fL -o redmine.tar.gz "$REDMINE_DOWNLOAD_URL"; 	echo "$REDMINE_DOWNLOAD_SHA256 *redmine.tar.gz" | sha256sum -c -; 	tar -xf redmine.tar.gz --strip-components=1; 	rm redmine.tar.gz files/delete.me log/delete.me; 	mkdir -p log public/plugin_assets sqlite tmp/pdf tmp/pids; 	chown -R redmine:redmine ./; 	echo 'config.logger = Logger.new(STDOUT)' > config/additional_environment.rb; 	chmod -R ugo=rwX config db sqlite; 	find log tmp -type d -exec chmod 1777 '{}' +
# Fri, 24 Jun 2022 03:01:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		default-libmysqlclient-dev 		freetds-dev 		gcc 		libpq-dev 		libsqlite3-dev 		make 		patch 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*; 		gosu redmine bundle config --local without 'development test'; 	puma="$(grep -E "^[[:space:]]*gem [:'\"]puma['\",[:space:]].*\$" Gemfile)"; 	{ echo; echo "$puma"; } | sed -re 's/^[[:space:]]+//' >> Gemfile; 	echo '# the following entries only exist to force `bundle install` to pre-install all database adapter dependencies -- they can be safely removed/ignored' > ./config/database.yml; 	for adapter in mysql2 postgresql sqlserver sqlite3; do 		echo "$adapter:" >> ./config/database.yml; 		echo "  adapter: $adapter" >> ./config/database.yml; 	done; 	gosu redmine bundle install --jobs "$(nproc)"; 	rm ./config/database.yml; 	chmod -R ugo=rwX Gemfile.lock "$GEM_HOME"; 	rm -rf ~redmine/.bundle; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| grep -v '^/usr/local/' 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 24 Jun 2022 03:01:10 GMT
VOLUME [/usr/src/redmine/files]
# Tue, 12 Jul 2022 02:38:18 GMT
COPY file:5ad924c6f87c91325ac6781766e5ad56444f0bea5780e13e8bed5000ee3cfc38 in / 
# Tue, 12 Jul 2022 02:38:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 12 Jul 2022 02:38:18 GMT
EXPOSE 3000
# Tue, 12 Jul 2022 02:38:18 GMT
CMD ["rails" "server" "-b" "0.0.0.0"]
# Tue, 12 Jul 2022 02:38:22 GMT
ENV PASSENGER_VERSION=6.0.14
# Tue, 12 Jul 2022 02:38:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gcc 		make 	; 	rm -rf /var/lib/apt/lists/*; 		gem install passenger --version "$PASSENGER_VERSION"; 	passenger-config build-native-support; 	if [ -n "$(passenger-config build-native-support 2>&1)" ]; then cat /tmp/passenger_native_support-*.log; false; fi; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jul 2022 02:38:42 GMT
RUN set -eux; 	passenger-config install-agent; 	passenger-config download-nginx-engine
# Tue, 12 Jul 2022 02:38:42 GMT
ENV PASSENGER_PID_FILE=tmp/pids/server.pid
# Tue, 12 Jul 2022 02:38:42 GMT
CMD ["passenger" "start"]
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b32e2eb2b46ed3629fec6dad87afe2b72f9fc1b6537616abee5098d841ed56f`  
		Last Modified: Thu, 23 Jun 2022 14:20:13 GMT  
		Size: 10.0 MB (9992026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1beb6afb9303c279fa4fd7025fbe3350fb3121a8ece1cee8f4c2089ddba78538`  
		Last Modified: Thu, 23 Jun 2022 14:20:11 GMT  
		Size: 200.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90f32716e9e86e73bd2c3f7e8dfd402eeb278de0004ef46205195d6b711d7b8`  
		Last Modified: Thu, 23 Jun 2022 14:24:01 GMT  
		Size: 14.6 MB (14582305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b38c958fd94004aaeaa93936001000585d4dc125e2b8417a65b6e5e2ee1f6ff4`  
		Last Modified: Thu, 23 Jun 2022 14:23:59 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52ac464cb0a80a3e38a7523c573238791251c2b35e235bab8a968bb23d7d289`  
		Last Modified: Fri, 24 Jun 2022 03:03:09 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d5173e4419ed0c78da3d593bc1947c29ff2546a6d8628c659fbf45952f59c4`  
		Last Modified: Fri, 24 Jun 2022 03:03:24 GMT  
		Size: 102.0 MB (101986878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d72df9d9a00f7ade0049950e4a04bf9ee60f24bc7ea66f69ff50d375095a54e`  
		Last Modified: Fri, 24 Jun 2022 03:03:06 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc69208e1b738d36d15baf856c2b2b0d158fde1a25d047b15fb5983e244b1ea0`  
		Last Modified: Fri, 24 Jun 2022 03:03:06 GMT  
		Size: 159.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f5c27c696621731ebeb10cab82ef9a1de130e18f4eb0952383220a7b800fe6a`  
		Last Modified: Fri, 24 Jun 2022 03:03:08 GMT  
		Size: 3.1 MB (3066335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cac5782f197ae88d1b681feb1d454d8b1151994aef8cf1daefcab055a5d4b7f`  
		Last Modified: Fri, 24 Jun 2022 03:03:11 GMT  
		Size: 45.3 MB (45306386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433b189e2a1250f9d5a8dad816907db6ff50cbbd2143319a22e3a92253d806f4`  
		Last Modified: Tue, 12 Jul 2022 02:43:15 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c683b9c530aa2b9f558d90f15357b0077471380a0fc5c908484c7bc4a7e906`  
		Last Modified: Tue, 12 Jul 2022 02:43:40 GMT  
		Size: 21.8 MB (21800334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafc9b824de5e5f45a5407dbd5dd52d7e94491c9690b436a1ef85af62dcc0e4f`  
		Last Modified: Tue, 12 Jul 2022 02:43:38 GMT  
		Size: 5.5 MB (5544419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
